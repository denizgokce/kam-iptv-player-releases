<p align="center">
  <img src="assets/icon.png" width="120" alt="KAM IPTV Player">
</p>

<h1 align="center">KAM IPTV Player</h1>

<p align="center">
  Ein IPTV-Player für macOS und Windows.<br>
  <b><a href="../../releases/latest">Neueste Version herunterladen</a></b>
</p>

<p align="center">
  <a href="README.md">English</a> · <a href="README.tr.md">Türkçe</a> · Deutsch
</p>

---

> **Bring deine eigene Playlist mit.** KAM IPTV Player ist nur ein Player. Er
> enthält keine Sender, Filme, Serien, Playlists oder Anbieter – du fügst deine
> eigenen hinzu. Siehe [Haftungsausschluss](DISCLAIMER.de.md).

Dieses Repository enthält **nur Installationsdateien**. Der Quellcode ist nicht öffentlich.

## Download

Öffne die [neueste Version](../../releases/latest) und wähle die Datei für deinen Rechner:

| Datei | Für |
|---|---|
| `KAM IPTV Player-<Version>-mac-arm64.dmg` | Mac mit Apple-Chip (M1 oder neuer) |
| `KAM IPTV Player-<Version>-mac-x64.dmg` | Mac mit Intel-Prozessor (sofern veröffentlicht) |
| `KAM IPTV Player-<Version>-win-x64.exe` | Windows 10 / 11, 64 Bit |

Zu jeder Version stehen die SHA-256-Prüfsummen aller Dateien in `SHA256SUMS.txt`.

## Installation

### macOS

1. Öffne die `.dmg` und ziehe **KAM IPTV Player** in **Programme**.
2. Beim ersten Mal: **Rechtsklick auf die App → Öffnen → Öffnen**.

Die App ist nicht von Apple notarisiert; ein einfacher Doppelklick wird beim
ersten Mal mit *„kann nicht geöffnet werden, da Apple sie nicht überprüfen
kann"* abgelehnt. Rechtsklick → Öffnen ist nur einmal nötig. Lehnt macOS
weiterhin ab, führe einmal im Terminal aus:

```sh
xattr -dr com.apple.quarantine "/Applications/KAM IPTV Player.app"
```

### Windows

1. Starte die `.exe`-Installationsdatei.
2. Meldet SmartScreen *„Der Computer wurde durch Windows geschützt"*, wähle **Weitere Informationen → Trotzdem ausführen**.

Die Installationsdatei ist nicht codesigniert; deshalb fragt SmartScreen nach.

## Was er kann

**Playlists**
- Anmeldung mit den Zugangsdaten deines Anbieters (Server, Benutzername,
  Passwort) oder eine M3U-/M3U8-Datei bzw. -Adresse laden.
- Listen bleiben auf deinem Rechner und werden nur aktualisiert, wenn du es willst.
- **Neu hinzugefügt** zeigt nach Tagen, was wann dazugekommen ist.

**Stöbern**
- Live-Sender, Filme und Serien in eigenen Bereichen, Serien automatisch nach Staffeln.
- Suche über alles, fehlertolerant – und ein Film wird unter jedem seiner
  Namen gefunden (*Akıl Oyunları* findet *A Beautiful Mind*).
- Eigene **Ordnergruppen** und gespeicherte **Filter-Chips** (*HD, aber nicht FHD*).
- Eigene **Playlists** – eine ganze Filmreihe in deiner Reihenfolge, per Drag & Drop sortiert.
- **Gesehen** und **Favoriten**, Fortsetzungspunkte und *Weiterschauen* mit dem
  Bild, bei dem du aufgehört hast.

**Details**
- Poster, Handlung, Bewertungen und Besetzung vom kostenlosen Dienst Stremio
  Cinemeta. Lässt sich in den Einstellungen komplett abschalten; dann wird kein
  externer Dienst angefragt.

**Wiedergabe**
- Mehrere Wiedergabe-Engines werden nacheinander versucht, mit eingebautem
  FFmpeg für Dateien, die die anderen nicht abspielen (MKV, AVI, ungewöhnliche Codecs).
- Audio- und Untertitelauswahl, Wiedergabegeschwindigkeit, ±10 s.
- Bild-in-Bild in einem schwebenden Fenster, das beim Arbeiten im Vordergrund bleibt.
- Ein Titel gilt als gesehen, sobald der Abspann beginnt.

## Datenschutz

- Kein Konto, keine Telemetrie, keine Analyse.
- Deine Playlists, Anbieterdaten, Favoriten und dein Verlauf bleiben auf deinem Rechner.
- Der einzige externe Dienst, der von selbst kontaktiert wird, ist Cinemeta –
  nur mit Titelnamen, und abschaltbar.

## Ein Problem melden

Eröffne ein [Issue](../../issues) mit Betriebssystem, App-Version
(Einstellungen) und was passiert ist. **Poste niemals deine Playlist,
Anbieteradresse, deinen Benutzernamen oder dein Passwort** – Streamadressen enthalten sie.

---

Copyright © 2026 die KAM-IPTV-Autoren. Alle Rechte vorbehalten. Siehe
[LICENSE](LICENSE) und den [Haftungsausschluss](DISCLAIMER.de.md).
