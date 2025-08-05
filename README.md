# mpv-dark-box

Minimalistic dark theme for mpv.

![Preview](preview.webp)

## Installation

* Download the [dark-box.lua](https://raw.githubusercontent.com/Mayurifag/mpv-dark-box/refs/heads/main/dark-box.lua) file from this repository.

* Place the `dark-box.lua` file into your mpv `scripts` directory:

**Windows:** `%APPDATA%/mpv/scripts/`

**Linux/macOS:** `~/.config/mpv/scripts/`

* Add the following lines to your `mpv.conf`:

```conf
# Required change. This disables the default OSC for script. Seems not needed in newer versions of mpv, but just in case.
osc=no
# Optional yet recommended changes:
[Auto.Idle]
profile-cond=p["idle-active"]
profile-restore=copy-equal
# When you start playing a video, mpv briefly shows a message like Playing: my_video.mkv. Following setting prevents that
osd-playing-msg=' '
# When mpv launched without file, do not show title (keep things minimal)
title=' '
# The idle window will start with a width of 640 pixels, giving you a consistent window size every time you launch the app
geometry=640
```

## Description

This is a fork of the original [maoiscat/mpv-dark-box](https://github.com/maoiscat/mpv-dark-box) with following changes:

| Change                     | Description                                                                                                   |
| :------------------------- | :------------------------------------------------------------------------------------------------------------ |
| Get back volume button     | Was hidden by original author. You can scroll on it to change volume!                                         |
| mpv v0.37.0+ compatibility | Thanks to @Samillion in [this issue comment](https://github.com/0dist/oscc/issues/6#issuecomment-2387559031). |
| README rewrite             | Translated to English and *opinionatedly* cleaned up.                                                         |

There is no active development here, things are working, yet any new vibecoded PRs are welcome!
