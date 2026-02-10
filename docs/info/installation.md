# Installing Noahh

## Using the installer

The official Noahh installer is currently under heavy remodelling. It will be brought back here when it's ready :) For now, you will have to install the SDK manually.

## Manually (on Windows)

### Prerequisites

 * [CMake](https://cmake.org/download/) (minimum v3.13.4, prefer latest)
 * A supported C++ compiler ([clang](https://releases.llvm.org/)/[MSVC](https://visualstudio.microsoft.com/downloads/))
 * [git](https://git-scm.com/downloads)

1. Install [Noahh CLI](https://github.com/noahh-sdk/cli/releases/latest)

  * Unzip the download file somewhere, and [add the directory with noahh.exe to your user's PATH variable](https://helpdeskgeek.com/windows-10/add-windows-path-environment-variable/). You may need to restart your command line after adding the directory to your path.

2. Navigate somewhere on your computer using the command line and do `git clone https://github.com/noahh-sdk/noahh --recursive`

  * You may want to switch to the `ui` branch **if you're reading this document _before_ 2022/10/10**. Do this with `git checkout ui`

3. Build Noahh yourself or ask HJfod for prebuilt binaries

4. [Create a new System Environment Variable](https://www.wikihow.com/Create-an-Environment-Variable-in-Windows-10) `NOAHH_SDK` and make its value be the path to the `noahh` repository on your computer (Example: `C:\Users\Steve\Documents\noahh`)

5. All done :) See the [instructions for creating a mod](/docs/tutorial/creating.md) next  



## Manually (on MacOS)

### Prerequisites

 * CMake, can be installed with [brew](https://formulae.brew.sh/formula/cmake#default) (minimum v3.13.4, prefer latest)
 * A supported C++ compiler (Apple Clang/[LLVM Clang](https://releases.llvm.org/), can be installed with [brew](https://formulae.brew.sh/formula/llvm#default))
 * git, preinstalled

1. Install [Noahh CLI](https://github.com/noahh-sdk/cli/releases/latest)

  * Unzip the download file somewhere, and [add the directory with noahh file to your user's PATH variable with .zshenv](https://stackoverflow.com/a/18077919). You need to restart your terminal after adding the directory to your path.
  * run `chmod +x path_to_noahh_executable` to make the file executable

2. Run `noahh profile add --name ProfileName "/path/to/Geometry Dash.app/Contents"`, then `noahh sdk install "/path/to/install/noahh"`, or leave the path blank to install to default path `/Users/Shared/Noahh/sdk`

3. Run `git submodule update --init --recursive` to pull th submodules

  * You may want to switch to the `ui` branch **if you're reading this document _before_ 2022/10/10**. Do this with `git checkout ui`

4. Build Noahh yourself after missing MacOS addresses are added

5. All done :) See the [instructions for creating a mod](/docs/tutorial/creating.md) next