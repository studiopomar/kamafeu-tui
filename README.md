# Kamafeu TUI

Standalone terminal dashboard for Kamafeu Studio. It is an optional companion and is not required by the graphical Studio.

## Build

```sh
cmake -S . -B build -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
```

FTXUI 7.0.3 is fetched by CMake at configure time. On Unix, enable CTest to run the terminal transport smoke test:

```sh
ctest --test-dir build --output-on-failure
```

Prebuilt archives are published for Windows x64, macOS Apple Silicon, macOS Intel, and Linux x64. The Studio's optional component manager can install these releases.

## License

Kamafeu TUI is distributed under the MIT License. FTXUI is a separate dependency with its own license and notices.
