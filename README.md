# clangwrapper

Wrapper for `clang` enforcing toolchain/libstdc++ includes/libraries to use.

Written as a hack for [scala-native](https://github.com/scala-native/scala-native)
so that compilation is possible also if libstdc++ in default path is too old.

Allows for compilation of [scala-native](https://github.com/scala-native/scala-native)
code with `g++` instead of `clang`.


## Installation
Copy `clang` to folder in `PATH` ahead of folder containing real `clang` and `clang++`.
Link `clang` to `clang++` (or create copy).

For compilation of `scala-native` code, `clang-major.minor` should not be wrapped,
i.e. the first `clang-major.minor` in `PATH` should be the real one.
