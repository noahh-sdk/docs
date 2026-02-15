---
title: Installation
icon: download
description: Instructions for installing Noahh
order: 0
---

# Installing Noahh

## For Users

> :warning: Please note that Noahh is **incompatible with all other mod loaders and mods**. We're porting stuff like Mega Hack and BetterEdit over, but don't expect their old releases to work.

Noahh is installed using **its own installer**. You can find the latest version [on the Noahh homepage](https://noahh-sdk.org) or [on GitHub](https://github.com/noahh-sdk/installer/releases/latest).

Noahh is currently available on **Windows** and **MacOS**; Android and iOS support is planned in the future.

## Installing Noahh SDK (for Developers)

### Prerequisites

 * [CMake](https://cmake.org/download/) (minimum v3.13.4, prefer latest)
 * A supported C++ compiler ([MSVC](https://visualstudio.microsoft.com/downloads/) for Windows, [clang](https://releases.llvm.org/) for MacOS)
 * [git](https://git-scm.com/downloads)

1. Install [Noahh CLI](https://github.com/noahh-sdk/cli/releases/latest) [(Instructions)](/info/installcli.md)
    * Unzip the download file somewhere, and [add the directory with noahh.exe to your user's PATH variable](/info/installcli.md#adding-cli-to-path-on-windows). You may need to restart your command line after adding the directory to your path.

2. [Install Noahh to GD](#for-users)

3. Run `noahh sdk install` to install the SDK (You can provide an argument to `noahh sdk install <path>` if you want to install somewhere other than the default path)
    * The installation should automatically set the `NOAHH_SDK` environment variable to point to the SDK on Windows. You might need to restart your terminal or IDE, or even have to restart your computer. If it still doesn't work then you'll have to set it manually, as it is required.

4. Run `noahh config setup` from the command line to set up a profile

5. Run `noahh sdk install-binaries` to install prebuilt binaries, or [build Noahh yourself](/source/building.md)
    * You can pick whether you want the `nightly` or `stable` branch of Noahh. `nightly` is the latest commit of the `main` branch, and contains all of the latest and greatest features but may also feature crashes and possibly not even compile, whereas `stable` is the latest released version. Use `noahh sdk update nightly` or `noahh sdk update stable` to switch between the two branches.

6. All done :) See the [instructions for creating a mod](/info/creating.md).
