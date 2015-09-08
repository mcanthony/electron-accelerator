# Electron-accelerator

Get up and running with a customisable electron build process!

This tool will request some configuration for your new electron project and the:

- Unpack a template to the current working directory.
- Apply your custom configuration

The end result is a project scaffold that supports building, debugging and releasing for Windows, Linux and Mac platforms.

### Installation

```
npm i electron-accelerator -g
```

### Usage

In your project directory.

```

Usage: electron-accelerator

This will prompt you to input options.
You can also supply these at the command line

Example: electron-accelerator --authors-name=Amy --application-name=Foo --platform=all --architecture=x64

Required options:

authors-name               any string
application-name           any string
platform                   all, linux, win32 or darwin
architecture               all, ia32 or x64
application-description    the description of your application
repository-url             the url of the repository for your application
setup-windows-releases     yes, no

Optional arguments:

squirrel-s3-bucket           the bucket name where a windows installer can be uploaded
squirrel-s3-bucket-prefix    the bucket prefix
squirrel-windows-update-url  the url that the windows installer will update from

```

This will:


- Unpack a template to the current working directory.
- Apply your custom configuration
- Write a ``readme.md`` to your project. The read me will describe how to build and release your electron app.
- Your new project will support
  - ``script/bootstrap`` - quickly and easily set up everything you need to get started with electron development
  - ``script/build`` - create custom builds for your required platforms
  - ``script/server`` - quickly run up your electron build to test
  - ``script/server-debug`` - quickly run up your electron build with node-inspector debugging


### Related projects and reading
This project stands on the shoulders of giants. It uses the following packages:

- [electron-packager](https://github.com/maxogden/electron-packager)
- [electron-prebuilt](https://github.com/mafintosh/electron-prebuilt)
- [grunt-electron-installer](https://github.com/atom/grunt-electron-installer)
