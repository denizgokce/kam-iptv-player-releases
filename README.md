<p align="center">
  <img src="assets/icon.png" width="120" alt="KAM IPTV Player">
</p>

<h1 align="center">KAM IPTV Player</h1>

<p align="center">
  A desktop IPTV player for macOS and Windows.<br>
  <b><a href="../../releases/latest">Download the latest release</a></b>
</p>

<p align="center">
  English · <a href="README.tr.md">Türkçe</a> · <a href="README.de.md">Deutsch</a>
</p>

---

> **Bring your own playlist.** KAM IPTV Player is only a player. It ships with
> no channels, films, series, playlists or provider of any kind — you add your
> own. See the [disclaimer](DISCLAIMER.md).

This repository holds **installers only**. The source code is not public.
For phones, tablets and Android TV, see [KAM IPTV for Android](https://github.com/denizgokce/kam-iptv-android-releases).

## Download

Open the [latest release](../../releases/latest) and pick the file for your computer:

| File | For |
|---|---|
| `KAM.IPTV.Player-<version>-mac-arm64.dmg` | Mac with Apple silicon (M1 or later) |
| `KAM.IPTV.Player-<version>-mac-x64.dmg` | Mac with an Intel processor (when published) |
| `KAM.IPTV.Player-<version>-win-x64.exe` | Windows 10 / 11, 64-bit |

Each release lists the SHA-256 checksum of every file in `SHA256SUMS.txt`.

## Installing

### macOS

1. Open the `.dmg` and drag **KAM IPTV Player** into **Applications**.
2. The first time, **right-click the app → Open → Open**.

The app is not notarised by Apple, so a plain double-click the first time is
refused with *"cannot be opened because Apple cannot check it"*. Right-click →
Open only has to be done once. If macOS still refuses, run this once in
Terminal:

```sh
xattr -dr com.apple.quarantine "/Applications/KAM IPTV Player.app"
```

### Windows

1. Run the `.exe` installer.
2. If SmartScreen says *"Windows protected your PC"*, choose **More info → Run anyway**.

The installer is not code-signed, which is why SmartScreen asks.

## What it does

**Playlists**
- Sign in with your provider's account details (server, username, password),
  or load an M3U / M3U8 file or URL.
- Lists are stored on your computer and refreshed only when you ask.
- **Recently Added** shows what arrived and when, grouped by day.

**Browsing**
- Live channels, films and series in separate sections, series grouped into
  seasons automatically.
- Search across everything, tolerant of typos — and a film is found under any
  of its names (*Akıl Oyunları* finds *A Beautiful Mind*).
- Your own **folder groups** and saved **filter chips** (*HD but not FHD*).
- **Playlists** of your own — a whole franchise in the order you want to
  watch it, rearranged by drag and drop.
- **Watched** and **Favourites**, resume points, and *Continue Watching* with
  the frame you left on.

**Details**
- Posters, plots, ratings and cast from the free Stremio Cinemeta service.
  You can switch this off completely in Settings; then nothing is requested
  from any outside service.

**Playback**
- Several playback engines tried in turn, with an FFmpeg fallback built in for
  files the others cannot play (MKV, AVI, unusual codecs).
- Audio and subtitle track selection, playback speed, ±10 s.
- Picture-in-picture in a floating window that stays on top while you work.
- A title is marked as watched when the end credits start.

## Privacy

- No account, no telemetry, no analytics.
- Your playlists, provider details, favourites and history stay on your
  computer.
- The only outside service contacted on its own is Cinemeta, with title names
  only, and it can be switched off.

## Reporting a problem

Open an [issue](../../issues) with your operating system, the app version
(Settings) and what happened. **Never post your playlist, provider address,
username or password** — stream addresses contain them.

---

Copyright © 2026 the KAM IPTV authors. All rights reserved. See [LICENSE](LICENSE)
and the [disclaimer](DISCLAIMER.md).
