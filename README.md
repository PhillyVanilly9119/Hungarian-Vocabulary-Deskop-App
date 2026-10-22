# Hungarian Vocabulary Trainer

Qt 6 desktop app for practicing English and Hungarian vocabulary, built with C++20 and CMake for macOS.

## Build

Requirements: Qt 6 (macOS), CMake 3.21+, Ninja or Make, Xcode command line tools.

```sh
cmake -S . -B build -G Ninja -DCMAKE_PREFIX_PATH="<path-to-Qt>/macos"
cmake --build build
open build/HungarianVocabulary.app
```
