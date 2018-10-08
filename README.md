pmdk-convert: PMDK pool conversion tool
=======================================

[![Build Status](https://travis-ci.org/pmem/pmdk-convert.svg?branch=master)](https://travis-ci.org/pmem/pmdk-convert)
[![Build status](https://ci.appveyor.com/api/projects/status/github/pmem/pmdk-convert?branch/master?svg=true&pr=false)](https://ci.appveyor.com/project/pmem/pmdk-convert/branch/master)
[![Coverage Status](https://codecov.io/github/pmem/pmdk-convert/coverage.svg?branch=master)](https://codecov.io/gh/pmem/pmdk-convert/branch/master)

# Building The Source #

Requirements:
- libpmem-dev(el) >= 1.3 (http://pmem.io/pmdk/)
- cmake >= 3.3
- git
On Windows:
- [Windows SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk) >= 10.0.16299

### On Linux ###
```sh
$ git clone https://github.com/pmem/pmdk-convert.git
$ cd pmdk-convert
$ mkdir build
$ cd build
$ cmake .. -DCMAKE_INSTALL_PREFIX=/home/user/pmdk-convert-bin
$ make
$ make install
```
### On Windows ###

```sh
PS> git clone https://github.com/pmem/pmdk-convert.git
PS> cd pmdk-convert
PS> mkdir build
PS> cd build
PS> cmake .. -G "Visual Studio 14 2015 Win64"
PS> msbuild build/ALL_BUILD.vcxproj
```

To build pmdk-convert on Windows 8 you have to specify your SDK version in the cmake command i.e.
```sh
PS> cmake .. -G "Visual Studio 14 2015 Win64" -DCMAKE_SYSTEM_VERSION="10.0.26624"
```
