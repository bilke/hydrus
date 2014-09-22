# Hydrus-1D for CMake

This is [Hydrus-1D](http://www.pc-progress.com/en/Default.aspx?hydrus-1d) adapted for CMake and GFortran. See the [Hydrus-1D technical manual](http://www.pc-progress.com/Downloads/Pgm_hydrus1D/HYDRUS1D-4.08.pdf) for more information.

It was tested on

- Linux with gcc 4.8.1 and [CMake](http://cmake.org) 2.8.12.
- Windows with MinGW and MSYS and CMake 3.0.2

## Instructions

```bash
git clone https://github.com/bilke/hydrus.git
mkdir build
cd build
cmake ../hydrus [-G "MSYS Makefiles"]
make
./h1d_calc
```

## MinGW setup

- Install MinGW as [described here](http://www.mingw.org/wiki/Getting_Started)
  - In the *MinGW Installation Manager* choose the packages `mingw-developer-tools`, `mingw32-base`, `mingw32-gcc-g++` and `msys-base`
- On the msys-shell run `mingw-get install fortran`
