# Atlas MapGenerator
A C++ Map Generator.
This project uses [Core framework](https://github.com/izkeas/Core) 

![Map generator Image](./MapGenerator.png "Map Generator Image")

## NOTE
This repository has been archived because I'm not working on it anymore, maybe I'll remake this project into a website form in the future

## Features
- Generate Pixel Art maps of a World
- set biomes with temperature, humidity and height
- save and load settings with world templates

## Build
this project uses meson as build system, to build do the following:

### Linux

        meson setup build
        meson compile -C build

Meson will download all required libraries and compile, then run the example with:

        ./build/src/Map\ Generator

### Windows

windows needs mingw, download and install [mingw](https://github.com/niXman/mingw-builds-binaries/releases), select the x86_64 posix sjlj

        meson setup build-mingw --cross-file mingw_cross.txt
        meson compile -C build-mingw
        ./build/src/Map Generator.exe

## Atlas Uses the following libraries
- Core framework
- fastnoiselite
- nlohmann_json
- magic_enum
