# Growtopia Proxy
[![Github Action](https://img.shields.io/github/actions/workflow/status/ZTzTopia/GTProxy/cmake_ci.yml?branch=dev&logo=github&logoColor=white)](https://github.com/ZTzTopia/GTProxy/actions?query=workflow%3ACI)
[![GitHub Release](https://img.shields.io/github/v/release/ZTzTopia/GTProxy.svg?color=orange&logo=docusign&logoColor=orange)](https://github.com/ZTzTopia/GTProxy/releases/latest) 

This is a proxy for [Growtopia](https://growtopiagame.com/), which makes it possible to debug incoming and outgoing packets and even modify them.

## Supported Platforms
- [Windows](https://www.microsoft.com/en-us/windows). Tested with Windows 7, 8, 10 and 11.
- [GNU/Linux](https://www.gnu.org/gnu/linux-and-gnu.en.html). Tested with Ubuntu and Arch Linux. (but who use GNU/Linux to play growtopia?)

## Features
- Free and open source.
- Print incoming and outgoing packets (text, variant list, etc).
- Support for [Growtopia](https://growtopiagame.com/) 3.92 and up.
- Built-in http server with metadata from [Growtopia](https://growtopiagame.com/) client.
- ~~Works well with sub-server redirection.~~ ([#22](https://github.com/ZTzTopia/GTProxy/issues/22))
- Config file.

## Download
The latest application executable can be found on the [releases page](https://github.com/ZTzTopia/GTProxy/releases).

## Build
The following dependencies are required to build from source.
- [CMake](https://cmake.org/).
- [Conan, the C/C++ Package Manager](https://conan.io) (v2.0+).

The following steps are for building from source.
1. First you need to clone the source code of this project. `git clone https://github.com/ZTzTopia/GTProxy.git --recurse-submodules`
2. Install Python 3.5+ (Windows only: select 'Add Python to PATH' in installer)
3. CMake will install needed package with [Conan, the C/C++ Package Manager](https://conan.io). `pip install "conan>2.0"`
```shell
$ mkdir build
$ cd build
$ cmake .. -DCMAKE_BUILD_TYPE=Debug
$ cmake --build .
```

## Credits
- Thanks to my two friends who helped a lot with this project.
- [Conan, the C/C++ Package Manager](https://conan.io/): The open source, decentralized and multi-platform package manager to create and share all your native binaries
- [LibreSSL](https://www.libressl.org/) is a version of the TLS/crypto stack forked from OpenSSL in 2014, with goals of modernizing the codebase, improving security, and applying best practice development processes
- [magic_enum](https://github.com/Neargye/magic_enum): Static reflection for enums (to string, from string, iteration)
- [nlohmann_json](https://github.com/nlohmann/json): JSON for Modern C++
- [pcg-cpp](https://github.com/imneme/pcg-cpp): Random number generator
- [randutils.hpp](https://gist.github.com/imneme/540829265469e673d045): Random utilities
- [spdlog](https://github.com/gabime/spdlog): Fast C++ logging library

## License
This project is licensed under the MIT License. See the [LICENSE](https://github.com/ZTzTopia/GTProxy/blob/main/LICENSE) file for details.
