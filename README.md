# Min - Nord Theme

This is my attempt at reskinning [the Min browser](https://minbrowser.org/) to wear the mighty [Nord color theme](https://www.nordtheme.com/).

This project is a fork of Min, the minimal browser. See the original repository [here](https://github.com/minbrowser/min).

## Installing

- Install [Node](https://nodejs.org).
- Run `npm install` to install dependencies.

### Building binaries

In order to build Min from source, follow the installation instructions above, then use one of the following commands to create binaries:

- `npm run buildWindows`
- `npm run buildMacIntel`
- `npm run buildMacArm`
- `npm run buildDebian`
- `npm run buildRaspi` (for Raspberry Pi, Raspberry Pi OS)
- `npm run buildLinuxArm64`
- `npm run buildRedhat`

Depending on the platform you are building for, you may need to install additional dependencies:

- If you are using macOS and building a package for Linux, install [Homebrew](http://brew.sh), then run `brew install fakeroot dpkg` first.
- If you are using macOS or Linux and building a package for Windows, you will need to install [Mono](https://www.mono-project.com/) and [Wine](https://www.winehq.org/).
- If you are building a macOS package, you'll need to install Xcode and the associated command-line tools. You may also need to set your default SDK to macOS 11.0 or higher, which you can do by running `export SDKROOT=/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX11.1.sdk`. The exact command will depend on where Xcode is installed and which SDK version you're using.
- To build on Windows, you'll need to install Visual Studio. Once it's installed, you may also need to run `npm config set msvs_version 2019` (or the appropriate version).
