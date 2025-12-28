# ShaderPlay

![Program Screen Recording](./assets/screen-recording.webp)

ShaderPlay is a dirt simple alternative to Shadertoy. It's primarily built for personal use, with a minimal feature set. Additional features will be added as needed.

## Dependences

- Required
    - C Compiler
        - **GCC**: For Linux
        - **MSVC**: For Windows
    - **Linux only:** XCB libraries (for GUI/windowing)
- Optional
    - **MinGW**: For cross-compiling Windows binaries on Linux
    - **Wine**: For running Windows builds on Linux during development/testing

## Building

- Compile the build tool:
```sh
cc build.c -o build
```
- Build the project:
```sh
./build build     # For Linux
./build.exe build # For Windows
```
- For more build system options/help:
```sh
./build --help     # For Linux
./build.exe --help # For Windows
```

## Running

- Running example shader:
```sh
./build/shaderpaly shaders/circles.frag     # For Linux
./build/shaderpaly.exe shaders/circles.frag # For Windows
```
- Run your own shader:
```sh
./build/shaderplay <shader_location>     # For Linux
./build/shaderplay.exe <shader_location> # For Windows
```
- For more options/help:
```sh
./build/shaderpaly --help       # For Linux
./build/shaderpaly.exe --help   # For Windows
```
