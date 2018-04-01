[![npm (scoped)](https://img.shields.io/npm/v/@gnu-mcu-eclipse/arm-none-eabi-gcc.svg)](https://www.npmjs.com/package/@gnu-mcu-eclipse/arm-none-eabi-gcc) 
[![license](https://img.shields.io/github/license/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack.svg)](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack/blob/xpack/LICENSE) 
[![Standard](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com/)


## GNU MCU Eclipse ARM Embedded GCC binaries

This xPack installs the platform specific binaries for the ARM Embedded toolchain.

This project is open source and it is publicly available from [GitHub](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack).

## Prerequisites

A recent [Node.js](https://nodejs.org) (>7.7), since the ECMAScript 6 class syntax and `async`/`await` are used.

If this is your first encounter with `npm`, you need to install the [node.js](https://nodejs.org/) JavScript run-time. The process is straightforward and does not pollute the system locations significantly; just pick the current version, download the package suitable for your platform and install it as usual. The result is a binary program called `node` that can be used to execute JavaScript code from the terminal, and a link called `npm`, pointing to the `npm-cli.js` script, which is part of the node module that implements the npm functionality. On Windows, it is recommended to first install the [Git for Windows](https://git-scm.com/download/win) package.

With `npm` available, the next step is to install `xpm`, the xPack package manager:

```console
$ sudo npm install xpm --global
```

On Windows, global `npm` packages are installed in the user home folder, and do not require `sudo`.

## Easy install

The module is available as [**gnu-mcu-eclipse/arm-none-eabi-gcc**](https://www.npmjs.com/package/gnu-mcu-eclipse/arm-none-eabi-gcc) from the public repository; with `npm` already available, installing the toolchain is quite easy:

```console
$ xpm install @gnu-mcu-eclipse/arm-none-eabi-gcc --global
```

Global `xpm` packages are installed in the user home folder, and do not require `sudo`.

To remove the installed xPack, the command is similar:

```console
$ xpm uninstall @gnu-mcu-eclipse/arm-none-eabi-gcc --global
```

(Note: not yet implemented)

## Developer info

### Git repo

```console
$ git clone https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc-xpack.git arm-none-eabi-gcc-xpack.git
```

### Toolchain binaries

The binaries are downloaded from the [gnu-mcu-eclipse/arm-none-eabi-gcc](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc) [releases](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases) project.

### Code standard compliance

The module currently does not include any JavaScript code.

### Code documentation metadata

The module currently does not include any documentation metadata

### How to publish

* open [releases](https://github.com/gnu-mcu-eclipse/arm-none-eabi-gcc/releases) and select the latest release
* update the `baseUrl:` with the file URLs (including the tag/version)
* from the blog post, copy the SHA & file names
* commit all changes, use a message like `7.2.0-1.2` (without `v`)
* `npm version 7.2.0-1.2`
* push all changes to GitHub
* `npm publish`

## License

The original content is released under the [MIT License](https://opensource.org/licenses/MIT), with all rights reserved to [Liviu Ionescu](https://github.com/ilg-ul).