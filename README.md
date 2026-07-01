<div align="center">
    <p>
    <h3>
      <b>
        Twoyi Platform
      </b>
    </h3>
  </p>
  <p>
    <b>
      A lightweight Android container
    </b>
    <br/>
  </p>
  <p>

[![Build APK](https://github.com/costaOSS/twoyi/actions/workflows/build.yml/badge.svg)](https://github.com/costaOSS/twoyi/actions/workflows/build.yml)
  </p>
  <p>
    <sub>
      Fork maintained by
      <a href="https://github.com/costaOSS">costaOSS</a>
    </sub>
  </p>
  <br />
  <p>
    <a href="https://twoyi.io">
      <img
        src="https://github.com/twoyi/twoyi/blob/main/assets/twoyi_screen.jpg?raw=true"
        alt="Screenshot"
        width="25%"
      />
    </a>
  </p>
</div>

## About

**Twoyi** is a lightweight Android container that runs a secondary Android environment on your device, powered by a Rust native library and an OpenGL ES renderer.

This is a maintained fork with dependency updates, security fixes, and modernized build toolchain.

## Build

You can trigger a build manually from the [Actions tab](https://github.com/costaOSS/twoyi/actions/workflows/build.yml) using the **Run workflow** button.

### Prerequisites

- JDK 17+
- Android SDK (platforms 27-36)
- Android NDK r27c+
- Rust with `aarch64-linux-android` target
- [cargo-xdk](https://github.com/tiann/cargo-xdk)

### Build locally

```bash
git clone https://github.com/costaOSS/twoyi
cd twoyi
./gradlew assembleRelease
```

The APK will be at `app/build/outputs/apk/release/`.

### Notes

- The build requires a valid `rootfs.7z` in `app/src/main/assets/` for a functional ROM.
- The app targets API 27+ with compileSdk 36.
- All dependencies are updated to their latest stable versions.
- JCenter repository has been removed (no longer available).

## License

This project is licensed under the Mozilla Public License, v. 2.0.
