# dtc-7.0
DragonTC 7.0 prebuilt :V

# How I compiled on Ubuntu 18.04
---------------------------
It's simple! Run the following commands in bash to get set up:
```
$ mkdir dtc
$ cd dtc
$ repo init -u https://github.com/dragon-tc/DragonTC -b master
$ repo sync -j(# of cores) -c -f
```
For Debian and Ubuntu:
```
sudo apt-get install clang build-essential git git-svn bc binfmt-support llvm-6.0 llvm-6.0-dev llvm-6.0-runtime cmake automake autogen autoconf autotools-dev libtool shtool python m4 gcc libtool zlib1g-dev libomp-dev
```

And run the following to build your desired toolchain:
```
$ cd build
$ ./version
```
Where "version" is 5.0 6.0 or 7.0
To optimize the toolchain for your local system, run with the 'opt' argument. Example:
```
$ ./7.0 opt
```
