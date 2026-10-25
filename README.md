# ROLLING THUNDER — release feed

Public release feed for **ROLLING THUNDER**, the Vietnam 1968 real-time strategy
game (US Army vs NVA/VC). The game polls this repository's latest release and
offers a one-click "Update & restart" on its start screen.

## Players

Download the newest `RollingThunder-vX.Y.Z-win-x64.zip` from
[Releases](https://github.com/lupulbraydon-ops/rolling-thunder-releases/releases),
unzip the whole folder, run `Rolling Thunder.exe`. `READ ME FIRST.txt` inside
the zip has the controls and the online-play instructions.

For LAN or online games every PC must run the same version — update both.

## Publishing (maintainer)

From the private source repo `lupulbraydon-ops/rolling-thunder`:

```
.\publish.ps1 -Version 0.19.0 -Release -Notes "what changed"
```

The script runs the sim + relay test gates, packages with electron-builder,
boots the packaged exe once, zips it and creates the GitHub release here.
