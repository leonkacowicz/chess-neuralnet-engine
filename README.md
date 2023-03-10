# What is this?
This package is a one of a series packages intended to
support the development of general purpose [chess engines and tools](
https://github.com/leonkacowicz/chess-tools).

This package extends the basic minimax-tree-searching 
[chess engine](https://github.com/leonkacowicz/chess-engine), by experimentally using
neuralnets as position evaluation function at the leave nodes of the [minimax-tree](
https://www.chessprogramming.org/Search_Tree).

# How do I build it?

This package uses CMake as a build-tool. In theory, it requires CMake 3.5,
but I haven't tested it with previous versions of CMake. If you manage to
build it with an older version of CMake, let me know or send a pull request
decreasing the required version on line 1 of `/CMakeLists.txt`

To build it:
```sh
mkdir build
cd build
cmake ..
make
```

# Testing
After building, an executable at `build/test/engine/engine_test` should be generated.
All tests specified in `/tests/` should be invoked by this executable.