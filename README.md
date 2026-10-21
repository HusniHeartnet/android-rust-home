# Android Rust Home

A light home screen (launcher) for Android, written in Rust.

Uses little memory, starts fast, asks for as few permissions as it can, and keeps everything on the
phone. See [PRIVACY.md](PRIVACY.md).

## Features

- App grid with search, a dock, and a clock
- Long-press menu to pin to the dock, hide or open app info
- Starts fast and stays small

## Install

Download the APK from the releases page and follow [docs/INSTALL.md](docs/INSTALL.md).

## Build

Needs Rust with the `aarch64-linux-android` target, `cargo-ndk`, the Android SDK (build-tools 34,
platform 34), NDK r27c and a JDK 17. Then, from `apps/home` (Windows PowerShell):

```
cargo test
powershell -File build-apk.ps1
```

APKs are signed with your own key, see [docs/SIGNING.md](docs/SIGNING.md).

## Layout

- `apps/home/` the app
- `tools/build/` the shared APK build script

## More apps

- [Android Rust Gallery](https://github.com/HusniHeartnet/android-rust-gallery)
- [Android Rust Files](https://github.com/HusniHeartnet/android-rust-files)
- [Android Rust Notes](https://github.com/HusniHeartnet/android-rust-notes)

## Licence

Copyright (C) heartnetapps. Licensed under the GNU General Public License, version 3 or (at your
option) any later version. See [LICENSE](LICENSE). The names and logos are not covered by the licence.
