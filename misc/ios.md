---
title: iOS Development Setup
---

# iOS Development Setup

Something something preamble

You will have to edit your `CMakeLists.txt` on your exiting mods. Newer created mods will already have this change
```cmake
# At the beginning of your CMakeLists.txt, change this:
#  set(CMAKE_OSX_ARCHITECTURES "arm64;x86_64")
# into:
if ("${CMAKE_SYSTEM_NAME}" STREQUAL "iOS" OR IOS)
    set(CMAKE_OSX_ARCHITECTURES "arm64")
else()
    set(CMAKE_OSX_ARCHITECTURES "arm64;x86_64")
endif()
```

## Build

To build mods for iOS, you must have Mac OS with the iPhone SDK installed from Xcode.

You must also get the Noahh binaries for iOS, you can do this using the CLI:
```bash
noahh sdk update nightly
noahh sdk install-binaries --platform ios
```

Nightly is required, as iOS is currently not on the stable release for Noahh.

Now you can build your mod for iOS via:
```bash
noahh build -p ios
```
Or if you want to build manually:
```bash
cmake -B build -DCMAKE_SYSTEM_NAME=iOS -DNOAHH_TARGET_PLATFORM=iOS -DCMAKE_BUILD_TYPE=RelWithDebInfo -G Ninja
cmake --build build
```

## Github Actions
To build your mod for iOS using `noahh-sdk/build-noahh-mod`, you have to add iOS to the build matrix, like so:
```yml
- name: iOS
  os: macos-latest
  target: iOS
```

As of writing this, iOS support is only available on nightly Noahh, so make sure to add this to the options of the `build-noahh-mod` step
```yml
sdk: nightly
```