# Changelog

All notable changes to this translation are documented here.
Alle nennenswerten Änderungen an dieser Übersetzung stehen hier.

## [1.2] — 2026-11-01

### Added / Neu
- Comfort menu on START (field): random battles on/off, EXP/Meseta x1/x2/x4, walking
  speed fast/normal, battle macro editor. START keeps its pause function in battle,
  dialogue, menus and vehicles. All settings stored in the save game.
  *Komfortmenü auf START (im Feld): Zufallskämpfe an/aus, EXP/Meseta x1/x2/x4,
  Lauftempo schnell/normal, Makro-Editor. In Kampf, Dialog, Menüs und Fahrzeugen bleibt
  START die Pausetaste. Alle Einstellungen werden im Spielstand gespeichert.*
- Battle macros with 4 slots and a full editor (inspired by Phantasy Star IV): command,
  technique/item and target for every party member, edited in the START menu. In
  battle: a separate field "M" right next to the command menu (cursor right from the
  Orders icon, then C) opens a list of the macros; choose one and C runs it for one
  round. Item and TP checks on load.
  *Kampf-Makros mit 4 Plätzen und vollem Editor (nach PS IV): Befehl, Technik/Gegenstand
  und Ziel je Gruppenmitglied, bearbeitet im START-Menü. Im Kampf: Ein eigenes Feld "M"
  direkt neben dem Befehlsmenü (Cursor vom Einzelbefehle-Symbol nach rechts, dann C)
  öffnet die Makro-Liste; Makro wählen, C führt es eine Runde aus. Gegenstand und TP
  werden beim Laden geprüft.*
- Battle speed-up: hold A during battle for double speed.
  *Kampf-Turbo: A im Kampf halten für doppeltes Tempo.*

### Fixed / Behoben
- Text speed selection after "Continue": the windows were drawn shifted and cut off,
  because the saved camera and scroll values were loaded before the selection (bug of
  the original game, also in the English version).
  *Textgeschwindigkeit nach "Spiel fortsetzen": Die Fenster erschienen verschoben und
  abgeschnitten, weil Kamera- und Scrollwerte des Spielstands schon vor der Abfrage
  geladen wurden (Fehler des Originals, auch in der englischen Fassung).*

### Changed / Geändert
- ROM expanded from 768 KB to 1 MB for the new code; header and checksum updated.
  *ROM für den neuen Code von 768 KB auf 1 MB erweitert; Header und Prüfsumme angepasst.*
- Save games stay compatible in both directions (1.0/1.1 ↔ 1.2).
  *Spielstände bleiben in beide Richtungen kompatibel (1.0/1.1 ↔ 1.2).*

### Verification / Verifikation
- German text and all data outside the 14 patched code locations are byte-identical
  to 1.1.
  *Deutscher Text und alle Daten außerhalb der 14 geänderten Codestellen sind
  byte-identisch mit 1.1.*
- ROM built from `ps3.asm` + `ps3.qol.asm` with the Macroassembler AS. All features
  verified in automated emulator runs, including test saves at ten story points of
  the first generation.
  *ROM aus `ps3.asm` + `ps3.qol.asm` mit dem Macroassembler AS gebaut. Alle Funktionen
  in automatisierten Emulatorläufen geprüft, auch mit Testspielständen an zehn
  Story-Punkten der ersten Generation.*

## [1.1] — 2026-08-30

### Added / Neu
- Full support for real German umlauts and ß (ä ö ü Ä Ö Ü) throughout all dialogue
  and menu text, replacing the ae/oe/ue/ss transcription used in 1.0.
  *Echte deutsche Umlaute und ß im gesamten Dialog- und Menütext, statt der
  Ersatzschreibweise ae/oe/ue/ss aus Version 1.0.*

### Fixed / Behoben
- Wedding-scene dialogue box that was cut off — two dialogue boxes had been
  incorrectly merged into a single script block.
  *Abgeschnittene Textbox in der Hochzeitsszene — zwei Dialoge waren fälschlich in
  einem Skriptblock zusammengefasst.*
- Revised phrasing on the bride-selection screen ("Ich heirate …" instead of the
  earlier "Ich nehme …").
  *Überarbeiteter Text bei der Bräute-Auswahl ("Ich heirate …" statt "Ich nehme …").*

### Verification / Verifikation
- ROM rebuilt from the disassembly source (`ps3.asm`) and diffed byte-for-byte
  against the reference build — identical apart from the recalculated header
  checksum, confirming the toolchain and source are consistent.
  *ROM aus dem Disassembly-Quelltext neu gebaut und byteweise mit dem Referenzbuild
  verglichen — identisch bis auf die neu berechnete Header-Prüfsumme.*
- The published `.bps` patch was independently re-applied to a clean source ROM;
  all three checksums embedded in the patch (source, target, patch) matched, and the
  resulting ROM was byte-identical to the rebuilt one.
  *Der veröffentlichte `.bps`-Patch wurde unabhängig erneut auf eine saubere
  Quell-ROM angewendet; alle drei im Patch enthaltenen Prüfsummen (Quelle, Ziel,
  Patch) stimmten, das Ergebnis war byte-identisch mit dem neu gebauten ROM.*

### Known issues / Bekannte Einschränkungen
- The ß glyph looks slightly B-like at 8×8 pixels.
  *Die ß-Glyphe wirkt bei 8×8 Pixeln etwas B-ähnlich.*
- End credits remain in English (separate character set).
  *Die Abspann-Credits bleiben englisch (eigener Zeichensatz).*

## [1.0] — 2026-08-04

### Added / Neu
- Initial German translation release: dialogue, menus and system text.
  *Erstveröffentlichung der deutschen Übersetzung: Dialoge, Menüs und Systemtext.*
- Umlauts transcribed as ae/oe/ue/ss due to font limitations of the original
  character set.
  *Umlaute als ae/oe/ue/ss umschrieben, bedingt durch den originalen Zeichensatz.*
- Item names and proper nouns intentionally left in English.
  *Gegenstands- und Eigennamen bewusst im englischen Original belassen.*
- Verified via a complete recorded playthrough (YouTube Let's Play).
  *Verifiziert durch ein komplettes aufgezeichnetes Let's Play.*

Patch and checksums kept in [`patches/v1.0/`](patches/v1.0/) for reference.
*Patch und Prüfsummen liegen in [`patches/v1.0/`](patches/v1.0/) zum Nachschlagen.*
