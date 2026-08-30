# Phantasy Star III: Generations of Doom — German Translation

**Version 1.1** · Release Date: 30.08.2026 · Author: **Karlhungus**
Platform: Sega Mega Drive / Genesis

> This is an unofficial fan translation. It is not affiliated with or endorsed by SEGA.
> No ROM is included — you must supply your own copy of the game. This project
> distributes a patch file only, never a pre-patched ROM.

---

## What's new in 1.1

- **Real German umlauts and ß** (ä ö ü Ä Ö Ü) throughout all dialogue and menu text,
  replacing the ae/oe/ue/ss transcription used in 1.0
- **Fixed:** a dialogue box in the wedding scene that was cut off (two dialogue boxes
  had been incorrectly merged into a single script block)
- Revised phrasing on the bride-selection screen ("Ich heirate …" instead of the
  earlier "Ich nehme …")

Full history: see [CHANGELOG.md](CHANGELOG.md).

---

## 1. About this patch (English)

This patch translates Phantasy Star III: Generations of Doom for the Sega Mega Drive /
Genesis into German.

| | |
|---|---|
| Dialogue | translated |
| Menus / system text | translated |
| Item names | **not** translated — left in the original English |
| Proper names | **not** translated — characters, places, techniques and enemies keep their original English names |

This was a deliberate decision. Item and proper names are deeply embedded in the
series' identity and are widely recognised by fans in their English form. Keeping them
intact also avoids space and pointer problems in the menu system.

**A note on umlauts:** as of version 1.1, the font has been extended to include proper
German umlauts (ä ö ü Ä Ö Ü) and ß, so these are used throughout instead of the ae/oe/
ue/ss transcription from version 1.0. Double-s ("ss") is still used where standard
German spelling actually calls for it after a short vowel (*muss, dass, Schloss,
lassen, Prinzessin, wissen, Schlüssel*, …) — that's correct orthography, not a font
limitation.

This is my first ROM hacking project. I worked on it entirely on my own, using AI both
for the translation itself and as technical support for script extraction, alignment
of the German and English text blocks, the font/character-set work for version 1.1,
and parts of the assembly work.

To check the result, I did not rely on spot tests: I recorded a complete Let's Play of
the German version on my YouTube channel and played it through from start to finish
for version 1.0. Version 1.1 was verified by rebuilding the ROM from source and
comparing it against the fully reviewed 1.0 text base — see
[Verifying the result](#4-verifying-the-result).

https://www.youtube.com/@rgbretrogaming

## 2. Required ROM

| | |
|---|---|
| Game | Phantasy Star III – Generations of Doom |
| Region code | UE (USA / Europe combined release) |
| Serial | GM 1303-01 |
| Copyright | (C)SEGA 1991.APL |
| Size | 786,432 bytes (768 KB / 6 Mbit) |
| Header | none — plain headerless .bin / .md dump |
| CRC32 | `C6B42B0F` |
| MD5 | `82c7bc027685cc8fc6c9e077beb1a75a` |
| SHA-1 | `59d4914e652672fd1e453c76b8250d17e8ca154e` |

The patch applies to this exact ROM only. If your file has a different size or
checksum, the patching tool will refuse it. No ROM is included with this patch and
none will be provided. You must supply your own copy of the game.

## 3. How to patch

- **Patch format:** BPS
- **Patch file:** [`patches/v1.1/PSIII_German_v1.1.bps`](patches/v1.1/PSIII_German_v1.1.bps)
- **Recommended tool:** [Floating IPS (Flips)](https://www.romhacking.net/utilities/1040/)

Steps:

1. Open Flips and choose "Apply Patch".
2. Select the `.bps` file from this repository.
3. Select your unmodified Phantasy Star III ROM.
4. Save the result under a new file name. Never overwrite your original ROM.

Alternatively, use the Online ROM Patcher on ROMhacking.net. BPS patches store a
checksum of the source ROM — if the tool reports a mismatch, your ROM is not the
expected version (see section 2).

## 4. Verifying the result

After patching, the file should match these values:

| | |
|---|---|
| Size | 786,432 bytes |
| CRC32 | `DB81C2E3` |
| MD5 | `d58ec62c1594a4aa0caed0f6fdce2035` |
| SHA-1 | `b35737e8bf7b58a0f270fa121c7d7c036e97a2a2` |
| Internal Mega Drive header checksum | `A9AE` (valid) |

Full checksum details, including the patch file's own hashes, are in
[`patches/v1.1/checksums_v1.1.txt`](patches/v1.1/checksums_v1.1.txt). The version 1.0
patch and its checksums are kept in [`patches/v1.0/`](patches/v1.0/) for reference.

The patched ROM passes the console's own integrity check and runs on original
hardware. SRAM configuration is unchanged, so battery saves work exactly as in the
original game; save files from the unpatched version remain compatible.

## 5. Tested on

- Emulator: **ares**

Version 1.1's text content was additionally verified by reconstructing the ROM from
the disassembly source and diffing it byte-for-byte against the fully reviewed 1.0
build — see the changelog for details.

## 6. Known issues

- The ß glyph looks slightly B-like at the game's native 8×8 pixel resolution.
- The end credits remain in English (they use their own, separate character set).
- No further issues are known at the time of release. Please report text bugs with a
  savestate or a description of where the passage appears (see [Contact](#9-contact)).

## 7. Credits

| | |
|---|---|
| Translation, hacking, testing | Karlhungus |
| Quality assurance | full recorded playthrough (v1.0), rebuild/diff verification (v1.1) |
| Tools | Floating IPS (Flips), custom script tooling |

The original SEGA staff credits are preserved in full. No developer has been removed
from or replaced in the in-game credit roll.

Thanks to the ROMhacking.net community for the documentation and utilities that made
a first project like this possible.

## 8. Legal

Phantasy Star III: Generations of Doom is copyright SEGA. This is an unofficial,
non-commercial fan translation distributed as a patch file only. It contains no
copyrighted game data.

The patch may be freely redistributed as long as the readme is included and no fee is
charged. **Do not distribute pre-patched ROMs.**

## 9. Contact

- YouTube: https://www.youtube.com/@rgbretrogaming
- Email: rgbretrogaming@protonmail.com

## 10. Changelog

See [CHANGELOG.md](CHANGELOG.md).

---

<details>
<summary><strong>Deutsch: Über diesen Patch</strong> (auf Klicken ausklappen)</summary>

## 1. Über diesen Patch

Dieser Patch übersetzt Phantasy Star III: Generations of Doom für das Sega Mega Drive
ins Deutsche. Es handelt sich um ein inoffizielles Fanprojekt ohne Verbindung zu SEGA.

|  |  |
|---|---|
| Dialoge | übersetzt |
| Menüs / Systemtext | übersetzt |
| Gegenstandsnamen | **nicht** übersetzt, im englischen Original belassen |
| Eigennamen | **nicht** übersetzt — Charaktere, Orte, Techniken und Gegner behalten ihre englischen Namen |

Das ist eine bewusste Entscheidung. Gegenstands- und Eigennamen sind fest mit der
Identität der Serie verbunden und den meisten Fans nur in ihrer englischen Form
geläufig. Außerdem vermeidet die Beibehaltung Platz- und Pointer-Probleme im
Menüsystem.

**Hinweis zu den Umlauten:** Ab Version 1.1 wurde der Zeichensatz um echte deutsche
Umlaute (ä ö ü Ä Ö Ü) und ß erweitert — diese werden jetzt durchgängig verwendet statt
der Ersatzschreibweise ae/oe/ue/ss aus Version 1.0. "ss" bleibt dort erhalten, wo es
nach kurzem Vokal auch nach amtlicher Rechtschreibung korrekt ist (*muss, dass,
Schloss, lassen, Prinzessin, wissen, Schlüssel*, …) — das ist korrekte Orthografie,
keine Einschränkung des Zeichensatzes mehr.

Dies ist mein erstes ROM-Hacking-Projekt. Ich habe es vollständig alleine umgesetzt
und dabei KI sowohl für die Übersetzung selbst als auch als technische Unterstützung
eingesetzt — für die Extraktion des Skripts, die Zuordnung der deutschen und
englischen Textblöcke, die Zeichensatz-Arbeit für Version 1.1 sowie Teile der
Assembler-Arbeit.

Zur Prüfung habe ich mich für Version 1.0 nicht auf Stichproben verlassen: Ich habe
ein komplettes Let's Play dieser deutschen Fassung auf meinem YouTube-Kanal
aufgenommen und das Spiel von Anfang bis Ende durchgespielt. Version 1.1 wurde durch
Neubau des ROMs aus dem Quelltext und byteweisen Abgleich gegen den vollständig
geprüften 1.0-Textstand verifiziert.

https://www.youtube.com/@rgbretrogaming

## 2. Benötigtes ROM

|  |  |
|---|---|
| Spiel | Phantasy Star III – Generations of Doom |
| Regionscode | UE (gemeinsame USA-/Europa-Fassung) |
| Seriennummer | GM 1303-01 |
| Copyright | (C)SEGA 1991.APL |
| Größe | 786.432 Bytes (768 KB / 6 Mbit) |
| Header | keiner — reiner headerloser .bin-/.md-Dump |
| CRC32 | `C6B42B0F` |
| MD5 | `82c7bc027685cc8fc6c9e077beb1a75a` |
| SHA-1 | `59d4914e652672fd1e453c76b8250d17e8ca154e` |

Der Patch lässt sich ausschließlich auf dieses ROM anwenden. Ein ROM liegt nicht bei
und wird auch nicht bereitgestellt.

## 3. Anwendung

1. Floating IPS (Flips) starten und "Apply Patch" wählen.
2. Die `.bps`-Datei aus diesem Repository auswählen.
3. Das unveränderte Phantasy Star III ROM auswählen.
4. Ergebnis unter neuem Dateinamen speichern — das Original nicht überschreiben.

Meldet das Programm eine falsche Prüfsumme, liegt eine andere ROM-Version vor.

## 4. Ergebnis prüfen

Nach dem Patchen sollte die Datei diese Werte aufweisen:

|  |  |
|---|---|
| Größe | 786.432 Bytes |
| CRC32 | `DB81C2E3` |
| MD5 | `d58ec62c1594a4aa0caed0f6fdce2035` |
| SHA-1 | `b35737e8bf7b58a0f270fa121c7d7c036e97a2a2` |
| Interne Mega-Drive-Prüfsumme | `A9AE` (gültig) |

Die SRAM-Konfiguration ist unverändert, Batteriespeicherstände funktionieren wie im
Original und bleiben kompatibel.

## 5. Credits

Übersetzung, Hacking, Test: Karlhungus. Die Original-Credits des SEGA-Entwicklerteams
sind vollständig erhalten.

## 6. Rechtliches

Phantasy Star III: Generations of Doom ist urheberrechtlich geschützt durch SEGA. Dies
ist eine inoffizielle, nicht kommerzielle Fanübersetzung, die ausschließlich als
Patchdatei verbreitet wird. Sie enthält keine geschützten Spieldaten.

Die Weitergabe ist gestattet, solange die Readme beiliegt und keine Gebühr erhoben
wird. **Die Verbreitung vorgepatchter ROMs ist untersagt.**

## 7. Kontakt

- YouTube: https://www.youtube.com/@rgbretrogaming
- E-Mail: rgbretrogaming@protonmail.com

</details>
