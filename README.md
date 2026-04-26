# Project README

## Overview
The project is a Brainfuck interpreter written in C. It includes support for compiling and running Brainfuck code on different operating systems (Linux, Windows, Wine, and WebAssembly).

## Features
- **Brainfuck Execution**: The core feature is the ability to run Brainfuck code.
- **Platform Support**: The project supports building and running on Linux, Windows using WINE, and WebAssembly.

## Project Structure

### Prerequisites
- **C/C++ Compiler and Debugger**: GCC, Clang (for Linux), MSVC or MinGW-w64 for Windows.
- **Make utility**: Required for building the project.
- **Standard Development Tools**: Typically installed with the C/C++ development environment.
- **Libraries Needed**:
  - None specific to this project.

## Build & Run

### Building on Linux
To build and run the Brainfuck interpreter on Linux, follow these steps:

```bash
cd /home/codeleaded/Hecke/C/Cmd_BrainFck
make -f Makefile.linux all  # Build the project
make -f Makefile.linux exe   # Run the built executable
```

### Building on Windows using WINE
To build and run the Brainfuck interpreter on Windows using WINE, follow these steps:

```bash
cd /home/codeleaded/Hecke/C/Cmd_BrainFck
make -f Makefile.wine all  # Build the project
make -f Makefile.wine exe   # Run the built executable in a WINE environment
```

### Building on WebAssembly (using Emscripten)
To build and run the Brainfuck interpreter for the web using WebAssembly, follow these steps:

```bash
cd /home/codeleaded/Hecke/C/Cmd_BrainFck
make -f Makefile.web all  # Build the project
make -f Makefile.web exe   # Run the built Wasm file with wasmtime
```

### General Build Options
- `make -f Makefile.(os) all`: Builds the project.
- `make -f Makefile.(os) do`: Builds and runs the executable.
- `make -f Makefile.(os) clean`: Cleans up build artifacts.

These instructions provide a comprehensive overview of building and running the Brainfuck interpreter on different platforms.