# Noahh Docs

### [Visit the Docs site](https://docs.noahh-sdk.org)

This is the source code for Noahh's docs, containing all the hand-written tutorials.

Class & function documentation is built automatically from [the Noahh source code](https://github.com/noahh-sdk/noahh).

## Building

The docs are built using [Flash](https://github.com/nipfswd/flash). To build the docs, you need Flash, along with [CMake](https://cmake.org/install/) and [Clang](https://clang.llvm.org/).

To build the docs, you first need to clone Noahh, and then clone the docs inside the Noahh root, for a folder structure like this:

```
noahh/
    docs/
        <docs files>
    <noahh files>
```

For example, you can do this with the following commands:

```
git clone https://github.com/noahh-sdk/noahh
cd noahh
git clone https://github.com/noahh-sdk/docs
```

Alternatively, you can symlink your local copy of the docs folder to your local copy of the Noahh folder.

After building Flash from source using Cargo or installing the latest release, you can build the docs with the following command:

```
flash -i <path/to/noahh> -o <relative_output_dir> --overwrite
```

Afterwards, start up a local HTTP server in the folder where you ran Flash.

You should run Flash in the directory you want to build the docs in and use `-o .`, or run it in the parent directory and do `-o <output_dir_name>`.