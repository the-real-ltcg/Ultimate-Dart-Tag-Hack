# Ultimate-Dart-Tag-Hack
Hack(s) for Ultimate Dart Tag

## Currently works for game Versions 1.0.0-1.0.2

## Fly Hack

A standalone, prebuilt copy of [Ultimate Dart Tag](https://github.com/the-real-ltcg/Ultimate-Dart-tag) with a free-fly cheat baked in. It's a full fork of the game's source, not an external injector — the fly toggle lives directly in `ThirdPersonController.cs`, gated so it never changes anything about the base game unless you actually use it.

### Controls
- **F7** — toggle fly mode on/off
- While flying: **WASD** to move (camera-relative, full 3D — you fly toward wherever you're looking), **Space** to rise, **Left Ctrl** to descend, hold **Shift** to go faster
- Gravity and ground collision are ignored entirely while flying; toggling off drops you back into normal movement wherever you are

### Building it yourself
Same process as the base game:
1. Open in Unity `6000.0.79f1`
2. `File > Build Settings > Windows` to produce an exe, or
3. Run `Installer/installer.iss` through Inno Setup for a proper installer

### Notes
- This is a separate build from the real game (different product name, install path, and installer AppId) so installing it won't overwrite or conflict with a real Ultimate Dart Tag install.
- Only affects the local client using it — it doesn't touch server-side/network state beyond normal movement, since the underlying game already treats client movement as authoritative.
- For private/friendly use only, same as the base game (LAN multiplayer, no ranked/competitive mode to worry about).
