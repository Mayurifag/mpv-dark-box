# mpv-dark-box

This is an mpv-osc script using mpv's native [osc.lua](https://github.com/mpv-player/mpv/blob/master/player/lua/osc.lua) based [MPV-EASY-Player project](https://github.com/422658476/MPV-EASY-Player/blob/master/mpv-easy-data/osc-style/osc-potplayer-box-knob-or-bar-0.lua)

## Preview

Preview 1

![Preview 1](assets/preview1.png)

Preview 2

![Preview 2](assets/preview2.png)

## How to use

1. Download and add dark-box.lua in the scripts directory.
2. Add `osc=no` in mpv.conf
3. Use mpv as usual

## Configuration Instructions

Like the built-in skin, edit osc.conf in script-opts to set the parameters, most of which are common to the built-in skin, with a few changes:

1. font     -- configure font used in OSC
2. layout   -- The script only has default style
3. logotext -- text is displayed under the logo at startup and supports ASS subtitle code.
4. Christmas hat has been removed

## Configuration options for the preview image

### mpv.conf

```conf
osc=no
[Auto.Idle]
profile-cond=p["idle-active"]
profile-restore=copy-equal
osd-playing-msg=' '
title=' '
background=1.0
geometry=640
```

### osc.conf

```conf
font=Consolas
logotext={\\1c&H00\\bord0\\fs30\\fn微软雅黑 light\\fscx125}MPV{\\fscx100} player
```

Also replace the icon of mpv.exe with a blank icon by yourself to achieve the same effect.
