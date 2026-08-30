# Changelog

All notable changes to this translation are documented here.
Alle nennenswerten Änderungen an dieser Übersetzung stehen hier.

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
