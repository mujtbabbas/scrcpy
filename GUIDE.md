# Reader's Guide — scrcpy

## What this project is

**scrcpy** (pronounced "screen copy", by Genymobile) **mirrors an Android
device — video and audio — to your computer over USB or TCP/IP, and lets you
control it with your keyboard and mouse**. It needs no root access and
installs nothing on the device. It is built for lightness and speed: native
code, 30–120 fps, 1920×1080 or better, ~35–70 ms latency, ~1 second startup,
no account, no ads, free and open source. It runs on Linux, Windows and macOS.

## How the content is organised

- `app/` — the desktop client (C code, icons and data files): the window you
  see and interact with.
- `server/` — the small server component pushed to the Android device at
  runtime (Java, built with the Gradle files at the root); nothing stays
  installed on the device afterwards.
- [`README.md`](README.md) — the front page: what scrcpy is, its headline
  properties, the feature list (audio forwarding, recording, virtual
  display, screen-off mirroring, copy-paste both ways, configurable quality,
  camera mirroring, webcam (V4L2) mode on Linux, HID keyboard/mouse,
  gamepads, OTG mode), and the per-OS download pages.
- `doc/` — **the real manual, one file per topic**: `connection.md`,
  `control.md`, `audio.md`, `video.md`, `recording.md`, `camera.md`,
  `keyboard.md`, `mouse.md`, `gamepad.md`, `otg.md`, `v4l2.md`,
  `virtual-display.md`, `window.md`, `device.md`, `tunnels.md`,
  `shortcuts.md`, the install guides `linux.md` / `windows.md` / `macos.md`,
  and the developer docs `build.md`, `develop.md`, `verify-release.md`.
- [`FAQ.md`](FAQ.md) — the frequently asked questions; `assets/` — README
  screenshots.

## How to use it

1. Follow your OS page in `doc/` (`linux.md`, `windows.md` or `macos.md`) to
   install, connect the device by USB (or see `doc/connection.md` for
   wireless TCP/IP), and run `scrcpy`.
2. Learn the controls from `doc/control.md` and `doc/shortcuts.md`.
3. Dive into the topic docs for the features you need — recording, camera,
   virtual display, gamepad — and check `FAQ.md` before filing an issue.

## About this standalone edition

This repository is a standalone edition of
[Genymobile/scrcpy](https://github.com/Genymobile/scrcpy), converted from a
fork into its own repository and enhanced in place. (The upstream warning
stands: the official source of scrcpy is the Genymobile repository.) See
[`ENHANCEMENTS.md`](ENHANCEMENTS.md) for what this edition adds and
[`CHANGELOG.md`](CHANGELOG.md) for its version history (v1.0.0 upstream
baseline, v1.1.0 enhancements). All original work belongs to Genymobile and
the upstream contributors; licence Apache-2.0 (see `LICENSE`).
