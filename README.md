[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc) [![npm](https://img.shields.io/npm/dw/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc/) [![npm](https://img.shields.io/npm/dt/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc/)

## The GNU MCU Eclipse ARM Embedded GCC binary xPack

This binary xPack installs the platform specific binaries for the [GNU MCU Eclipse 
ARM Embedded GCC](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc) toolchain.

The source files of the xPack project are publicly available from 
[GitHub](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack).

## Prerequisites

On all platforms, all is needed is a recent [`xpm`](https://www.npmjs.com/package/xpm), which is a portable 
[Node.js](https://nodejs.org) command line application.

## Easy install

The xPack is available as 
[`@gnu-mcu-eclipse/arm-none-eabi-gcc`](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc) 
from the public `npmjs.com` repository; with `xpm` available, installing 
the latest version of the toolchain is quite easy:

```console
$ xpm install @gnu-mcu-eclipse/arm-none-eabi-gcc --global
```

Global xPacks are installed in the user home folder, and do not require `sudo`.

To remove the installed xPack, the command is similar:

```console
$ xpm uninstall @gnu-mcu-eclipse/arm-none-eabi-gcc --global
```

(Note: not yet implemented)

## Developer info

### xPack git repo

The few xPack source files are available from GitHub:

```console
$ git clone https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack.git arm-none-eabi-gcc-xpack.git
```

### Toolchain binaries

The binaries are not stored on the `npmjs.com` server, but are downloaded from the 
[releases](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases) 
section of the `gnu-mcu-eclipse/arm-none-eabi-gcc` GitHub project.

### How to publish

* open [releases](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases) 
and select the latest release
* update the `baseUrl:` with the file URLs (including the tag/version)
* from the blog post, copy the SHA & file names
* commit all changes, use a message like `package.json: 7.2.0-1.2` (without `v`)
* `npm version 7.2.0-1.2`
* push all changes to GitHub
* `npm publish`

Multiple xPack releases referring to the same GitHub release have an extra 
digit in the version field, like `7.2.0-1.2.3`.

## License

The original content is released under the 
[MIT License](https://opensource.org/licenses/MIT), with all rights 
reserved to [Liviu Ionescu](https://github.com/ilg-ul).

The binary distributions include several open-source components; the
corresponding licenses are available in the `gnu-mcu-eclipse/licenses`
folder.
