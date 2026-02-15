---
title: Installation
icon: download
description: Instructions for installing Noahh
order: 0
---

# Installing Noahh

## For Users

Noahh is currently available on **Windows** and **MacOS**; Android and iOS support is planned in the future.

Noahh is installed using **its own installer**. You can find the latest version [on the Noahh homepage](https://noahh-sdk.org) or [on GitHub](https://github.com/noahh-sdk/installer/releases/latest). 

You can also [install the files manually](#installing-noahh-manually), should the installer not work.

> :warning: Please note that Noahh is **incompatible with all other mod loaders and mods**. We're porting stuff like Mega Hack and BetterEdit over, but don't expect their old releases to work.

## Installing Noahh Manually

In most cases, you should be fine by using the installer for installing Noahh. However, timeouts and other WiFi shenanigans can make it difficult at times for the installer to do it's job properly as of writing this. To get around it, you can simply drop the Noahh files into the Geometry Dash folder following the instructions below.

1. Download the most recent .zip release of Noahh [from here](https://github.com/noahh-sdk/noahh/releases). It should contain several files, the v1.0.0-beta.18 release being shown below for example: 

![Image of the files in the .zip, listed in this order: 1. Noahh.dll, 2. Noahh.lib, 3. Noahh.pdb, 4. NoahhBootstrapper.dll, 5. XInput9_1_0.dll.](/assets/(Jarten)NoahhFilesExample.png)

2. Find your Geometry Dash folder. For Windows, it should be stored in `C:\Program Files (x86)\Steam\steamapps\common\Geometry Dash`. For MacOS, it should be stored in `<User>/Library/Application Support/Steam/steamapps/common/Geometry Dash`. The `Library` directory is usually hidden, so using the Finder is ideal.

3. Extract all of the files from the Noahh .zip folder into the Geometry Dash folder so that all the files from the .zip are on the same level as the Geometry Dash executable.

Then launch the game. If it didn't work, go yell at Jarten#4513 on Discord because he was the one who wrote this. Including this last bit. Please yell at me if it goes wrong since I have almost zero experience with Noahh as of yet and still decided to do this anyway.

## Installing Noahh SDK (for Developers)

### Prerequisites

 * [CMake](https://cmake.org/download/) (minimum v3.13.4, prefer latest)
 * A supported C++ compiler ([MSVC](https://visualstudio.microsoft.com/downloads/) for Windows, [clang](https://releases.llvm.org/) for MacOS)
 * [git](https://git-scm.com/downloads)

1. Install [Noahh CLI](https://github.com/noahh-sdk/cli/releases/latest) [(Instructions)](/noahh/installcli)
    * Unzip the download file somewhere, and [add the directory with noahh.exe to your user's PATH variable](/noahh/installcli#adding-cli-to-path-on-windows). You may need to restart your command line after adding the directory to your path.

2. Install Noahh to GD. This means using [the installer](#installing-noahh) or [installing it manually](#installing-noahh-manually) 

3. Run `noahh sdk install` to install the SDK (You can provide an argument to `noahh sdk install <path>` if you want to install somewhere other than the default path)
    * The installation should automatically set the `NOAHH_SDK` environment variable to point to the SDK on Windows. You might need to restart your terminal or IDE, or even have to restart your computer. If it still doesn't work then you'll have to set it manually, as it is required.

4. Run `noahh config setup` from the command line to set up a profile

5. Run `noahh sdk install-binaries` to install prebuilt binaries, or [build Noahh yourself](/source/building.md)
    * You can pick whether you want the `nightly` or `stable` branch of Noahh. `nightly` is the latest commit of the `main` branch, and contains all of the latest and greatest features but may also feature crashes and possibly not even compile, whereas `stable` is the latest released version. Use `noahh sdk update nightly` or `noahh sdk update stable` to switch between the two branches.

6. All done :) See the [instructions for creating a mod](/noahh/creating.md).
