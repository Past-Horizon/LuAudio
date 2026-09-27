# LuAudio — Cross-Platform C++ Audio Engine

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-lightgrey)](CMakePresets.json)
[![C++](https://img.shields.io/badge/C%2B%2B-20-blue)](CMakeLists.txt)

LuAudio is a cross-platform C++ audio engine built with performance in mind.

It supports real-time playback, offline rendering, audio effects, plugins, and multiple platform audio backends.

## Features

* Real-time audio playback
* Offline audio rendering
* WAV support
* Ogg/Vorbis read and write
* MP3 support
* Audio effect chaining
* Plugin support
* Platform audio backends
* Cross-platform C++20 API

## Platform Support

| Platform | Status        | Notes    |
| -------- | ------------- | -------- |
| Windows  | ✅ Most mature | WASAPI   |
| Android  | ✅ Tested      | Oboe     |
| Linux    | 🟡 Supported  | PipeWire |

## Is it stable?

LuAudio has gone through stress testing across its supported platforms, including a lot of testing on Android.

It's still a project under development though, so issues can happen. Feel free to open an issue if you find one.

## Documentation

LuAudio does not currently have a documentation website.

The public headers are fully documented and are currently the main source of API documentation.

## Building

LuAudio uses CMake.

### Windows

You'll need Visual Studio with C++ tools, the Windows SDK, CMake, and Ninja.

Available presets:

```
x64-debug
x64-release
x86-debug
x86-release
```

Open the project in Visual Studio, select a preset, and build normally.

### Android

You'll need the Android NDK 29.0.14206865, CMake, and Ninja.

Available presets:

```
android-arm64-debug
android-arm64-release
```

### Hardcoded paths

Some paths in `CMakePresets.json` currently point to my own setup, so you may need to change them for your machine.

## History

LuAudio started as a small C++ audio project and slowly grew into a proper cross-platform audio engine.

As I kept working on it, I added more formats, platform backends, effects, plugins, offline rendering, and in-memory audio support.

## Vision

I want LuAudio to stay relatively lightweight while still being capable enough for real applications that need an audio engine without dragging in a huge framework.

## License

LuAudio uses the Apache 2.0 license. See [LICENSE](LICENSE) for details.
