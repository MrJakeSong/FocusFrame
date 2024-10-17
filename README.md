<div align="center">
  <h1>FocusFrame</h1>
</div>

<p align="center">
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT">
  </a>

  <a href="https://goreportcard.com/report/github.com/skryvvara/focusframe">
    <img src="https://goreportcard.com/badge/github.com/skryvvara/focusframe" alt="Go Report Card">
  </a>

  <a href="https://github.com/skryvvara/focusframe/actions/workflows/build.yml">
    <img src="https://github.com/skryvvara/focusframe/actions/workflows/build.yml/badge.svg" alt="Pipeline Status">
  </a>
</p>

## About

FocusFrame is a window management tool designed to run applications in a borderless window just like the "Fake Fullscreen"-Mode many games offer while not filling the entire screen.

<img src="./.github/images/example_screenshot.png" src="Screenshot of running Baldur's Gate 3 in a 16:9 2560x1440 window on 49 inch monitor">

This is an open source alternative to the closed source variant [Windowed Borderless Gaming](https://westechsolutions.net/sites/WindowedBorderlessGaming/home) developed by [Gameplay Crush](https://steamcommunity.com/id/GameplayCRUSH/).

As FocusFrame is in early development, consider using his software for a more feature-complete and stable state.

## Usage

> Please note that the usage of this application can change multiple times during the early stage of development. The current approach using the `toggle`key will **not be** the final solution.

Press the `toggle`-Key (default `F4`) to manage/unmanage an application. Managed application will be moved to the configured position and size when receiving focus.

## Installation

### Binary Releases

Download and unpack from https://github.com/skryvvara/focusframe/releases.

## Build

To build the application from source use the steps listed below.

### Windows

```sh
make

# or

GOOS=windows \
GOARCH=amd64 \
go build \
-ldflags '-H=windowsgui -X main.Version=v1.0.0'
-o ./bin/focusframe.exe \
./cmd
```

The executable is then found in the `bin` directory (e.g) `bin/focusframe.exe`.

## Compatibility

Compatiblity is currently limited to Windows 11 and Windows 10 (although Windows 8 and Windows 7 should work as well but are not actively tested).

To learn more about topics that are currently blocking support for other operating systems, refer to this [wiki article](https://github.com/Skryvvara/FocusFrame/wiki/Operating-System-Support#what-issues-are-currently-blocking-support-for-different-operating-systems).

## Contributors

<a href="https://github.com/skryvvara/focusframe/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=skryvvara/focusframe" alt="Contributors">
</a>

## Contributing

We welcome contributions! Please refer to our [contributing guide](/CONTRIBUTING.md).

## Special thanks

A big thanks to [Gameplay Crush](https://steamcommunity.com/id/GameplayCRUSH/), the developer of [Windowed Borderless Gaming](https://westechsolutions.net/sites/WindowedBorderlessGaming/home) which is the software that inspired this project.

## License

FocusFrame is released under the [MIT](https://opensource.org/licenses/MIT) License.
