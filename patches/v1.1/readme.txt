================================================================================

  PHANTASY STAR III: GENERATIONS OF DOOM
  German Translation / Deutsche Uebersetzung

  Version 1.1
  Release Date: 30.08.2026

  Author: Karlhungus
  Platform: Sega Mega Drive / Genesis

================================================================================


--------------------------------------------------------------------------------
  1. ABOUT THIS PATCH  (English)
--------------------------------------------------------------------------------

This patch translates Phantasy Star III: Generations of Doom for the Sega
Mega Drive / Genesis into German. It is an unofficial fan project and is
not affiliated with or endorsed by SEGA.

  Dialogue ............ translated
  Menus / System text . translated
  Item names .......... NOT translated - left in the original English
  Proper names ........ NOT translated - characters, places, techniques
                        and enemies keep their original English names

This was a deliberate decision. Item and proper names are deeply embedded
in the series' identity and are widely recognised by fans in their English
form. Keeping them intact also avoids space and pointer problems in the
menu system.

A note on umlauts: as of version 1.1, the font has been extended to
include proper German umlauts (ae oe ue Ae Oe Ue written here as plain
ASCII - use a viewer that supports the accented letters to see them
correctly) and the eszett. These are now used throughout, replacing the
ae/oe/ue/ss transcription from version 1.0. Double-s ("ss") is still used
where standard German spelling actually calls for it after a short vowel
(muss, dass, Schloss, lassen, Prinzessin, wissen, Schluessel, ...) - that
is correct orthography, not a font limitation.

This is my first ROM hacking project. I worked on it entirely on my own,
using AI both for the translation itself and as technical support for the
script extraction, the alignment of the German and English text blocks,
the font/character-set work for version 1.1, and parts of the assembly
work.

To check the result, I did not rely on spot tests for version 1.0: I
recorded a complete Let's Play of the game in the German version on my
YouTube channel and played it through from start to finish. Version 1.1
was verified by rebuilding the ROM from source and diffing it byte-for-
byte against the fully reviewed version 1.0 text base.

  https://www.youtube.com/@rgbretrogaming


--------------------------------------------------------------------------------
  2. REQUIRED ROM
--------------------------------------------------------------------------------

  Game:          Phantasy Star III - Generations of Doom
  Region code:   UE  (USA / Europe combined release)
  Serial:        GM 1303-01
  Copyright:     (C)SEGA 1991.APL
  Size:          786.432 bytes  (768 KB / 6 Mbit)
  Header:        none - plain headerless .bin / .md dump

  CRC32:         C6B42B0F
  MD5:           82c7bc027685cc8fc6c9e077beb1a75a
  SHA-1:         59d4914e652672fd1e453c76b8250d17e8ca154e

The patch applies to this exact ROM only. If your file has a different
size or checksum, the patching tool will refuse it.

No ROM is included with this patch and none will be provided. You must
supply your own copy of the game.


--------------------------------------------------------------------------------
  3. HOW TO PATCH
--------------------------------------------------------------------------------

  Patch format:  BPS
  Patch file:    PSIII_German_v1.1.bps

  Recommended tool: Floating IPS (Flips)
                    https://www.romhacking.net/utilities/1040/

  Steps:
    1. Open Flips and choose "Apply Patch".
    2. Select the .bps file from this archive.
    3. Select your unmodified Phantasy Star III ROM.
    4. Save the result under a new file name.
       Never overwrite your original ROM.

  Alternatively, use the Online ROM Patcher on ROMhacking.net.

  BPS patches store a checksum of the source ROM. If the tool reports a
  mismatch, your ROM is not the expected version - see section 2.


--------------------------------------------------------------------------------
  4. VERIFYING THE RESULT
--------------------------------------------------------------------------------

  After patching, the file should match these values:

  Size:          786.432 bytes
  CRC32:         DB81C2E3
  MD5:           d58ec62c1594a4aa0caed0f6fdce2035
  SHA-1:         b35737e8bf7b58a0f270fa121c7d7c036e97a2a2

  The internal Mega Drive checksum has been recalculated and is valid
  (A9AE). The patched ROM therefore passes the console's own integrity
  check and runs on original hardware.

  The SRAM configuration is unchanged, so battery saves work exactly as
  in the original game. Save files from the unpatched version remain
  compatible.

  Patch file itself:
  Size:          39.656 bytes
  MD5:           8a24162c4af991f10291df24a745276f
  SHA-1:         612afbeaba72e4c8ac366c821504b371ac6af2ac


--------------------------------------------------------------------------------
  5. TESTED ON
--------------------------------------------------------------------------------

  Emulator:      ares

  Version 1.1's text content was additionally verified by rebuilding the
  ROM from the disassembly source and diffing it byte-for-byte against
  the fully reviewed version 1.0 build, and by independently re-applying
  the published patch and comparing checksums.

  The ROM size is unchanged, so the patch works on flash carts and
  reproduction hardware without special requirements.


--------------------------------------------------------------------------------
  6. KNOWN ISSUES
--------------------------------------------------------------------------------

  The eszett glyph looks slightly B-like at the game's native 8x8 pixel
  resolution.

  The end credits remain in English (they use their own, separate
  character set).

  Please report text bugs with a savestate or a description of where the
  passage appears. See section 9 for contact details.


--------------------------------------------------------------------------------
  7. CREDITS
--------------------------------------------------------------------------------

  Translation, hacking, testing ......... Karlhungus
  Quality assurance ..................... full recorded playthrough (v1.0),
                                          rebuild/diff verification (v1.1)
  Tools ................................. Floating IPS (Flips),
                                          custom script tooling

  The original SEGA staff credits are preserved in full. No developer
  has been removed from or replaced in the in-game credit roll.

  Thanks to the ROMhacking.net community for the documentation and
  utilities that made a first project like this possible.


--------------------------------------------------------------------------------
  8. LEGAL
--------------------------------------------------------------------------------

  Phantasy Star III: Generations of Doom is copyright SEGA.
  This is an unofficial, non-commercial fan translation distributed as a
  patch file only. It contains no copyrighted game data.

  The patch may be freely redistributed as long as this readme is
  included and no fee is charged. Do not distribute pre-patched ROMs.


--------------------------------------------------------------------------------
  9. CONTACT
--------------------------------------------------------------------------------

  YouTube ........... https://www.youtube.com/@rgbretrogaming
  Email ............. rgbretrogaming@protonmail.com


--------------------------------------------------------------------------------
  10. CHANGELOG
--------------------------------------------------------------------------------

  v1.1  -  30.08.2026  -  Real umlauts and eszett throughout (replacing
                          ae/oe/ue/ss); fixed cut-off dialogue box in the
                          wedding scene; revised bride-selection phrasing
  v1.0  -  04.08.2026  -  Initial release


================================================================================
================================================================================


--------------------------------------------------------------------------------
  UEBER DIESEN PATCH  (Deutsch)
--------------------------------------------------------------------------------

Dieser Patch uebersetzt Phantasy Star III: Generations of Doom fuer das
Sega Mega Drive ins Deutsche. Es handelt sich um ein inoffizielles
Fanprojekt ohne Verbindung zu SEGA.

  Dialoge ............. uebersetzt
  Menues / Systemtext . uebersetzt
  Gegenstandsnamen .... NICHT uebersetzt, im englischen Original belassen
  Eigennamen .......... NICHT uebersetzt - Charaktere, Orte, Techniken
                        und Gegner behalten ihre englischen Namen

Das ist eine bewusste Entscheidung. Gegenstands- und Eigennamen sind fest
mit der Identitaet der Serie verbunden und den meisten Fans nur in ihrer
englischen Form gelaeufig. Ausserdem vermeidet die Beibehaltung Platz-
und Pointer-Probleme im Menuesystem.

Hinweis zu den Umlauten: Ab Version 1.1 wurde der Zeichensatz um echte
deutsche Umlaute und das Eszett erweitert - diese werden jetzt
durchgaengig verwendet statt der Ersatzschreibweise ae/oe/ue/ss aus
Version 1.0. "ss" bleibt dort erhalten, wo es nach kurzem Vokal auch nach
amtlicher Rechtschreibung korrekt ist (muss, dass, Schloss, lassen,
Prinzessin, wissen, Schluessel, ...) - das ist korrekte Orthografie,
keine Einschraenkung des Zeichensatzes mehr.

Dies ist mein erstes ROM-Hacking-Projekt. Ich habe es vollstaendig
alleine umgesetzt und dabei KI sowohl fuer die Uebersetzung selbst als
auch als technische Unterstuetzung eingesetzt - fuer die Extraktion des
Skripts, die Zuordnung der deutschen und englischen Textbloecke, die
Zeichensatz-Arbeit fuer Version 1.1 sowie Teile der Assembler-Arbeit.

Zur Pruefung habe ich mich fuer Version 1.0 nicht auf Stichproben
verlassen: Ich habe ein komplettes Let's Play dieser deutschen Fassung
auf meinem YouTube-Kanal aufgenommen und das Spiel von Anfang bis Ende
durchgespielt. Version 1.1 wurde durch Neubau des ROMs aus dem Quelltext
und byteweisen Abgleich gegen den vollstaendig geprueften 1.0-Textstand
verifiziert.

  https://www.youtube.com/@rgbretrogaming


--------------------------------------------------------------------------------
  BENOETIGTES ROM
--------------------------------------------------------------------------------

  Spiel:         Phantasy Star III - Generations of Doom
  Regionscode:   UE  (gemeinsame USA-/Europa-Fassung)
  Seriennummer:  GM 1303-01
  Copyright:     (C)SEGA 1991.APL
  Groesse:       786.432 Bytes  (768 KB / 6 Mbit)
  Header:        keiner - reiner headerloser .bin-/.md-Dump

  CRC32:         C6B42B0F
  MD5:           82c7bc027685cc8fc6c9e077beb1a75a
  SHA-1:         59d4914e652672fd1e453c76b8250d17e8ca154e

  Der Patch laesst sich ausschliesslich auf dieses ROM anwenden. Ein ROM
  liegt nicht bei und wird auch nicht bereitgestellt.


--------------------------------------------------------------------------------
  ANWENDUNG
--------------------------------------------------------------------------------

  1. Floating IPS (Flips) starten und "Apply Patch" waehlen.
  2. Die .bps-Datei aus diesem Archiv auswaehlen.
  3. Das unveraenderte Phantasy Star III ROM auswaehlen.
  4. Ergebnis unter neuem Dateinamen speichern - das Original nicht
     ueberschreiben.

  Meldet das Programm eine falsche Pruefsumme, liegt eine andere
  ROM-Version vor.


--------------------------------------------------------------------------------
  ERGEBNIS PRUEFEN
--------------------------------------------------------------------------------

  Nach dem Patchen sollte die Datei diese Werte aufweisen:

  Groesse:       786.432 Bytes
  CRC32:         DB81C2E3
  MD5:           d58ec62c1594a4aa0caed0f6fdce2035
  SHA-1:         b35737e8bf7b58a0f270fa121c7d7c036e97a2a2

  Die interne Mega-Drive-Pruefsumme wurde neu berechnet und ist gueltig
  (A9AE). Das gepatchte ROM besteht damit die Integritaetspruefung der
  Konsole und laeuft auf Originalhardware.

  Die SRAM-Konfiguration ist unveraendert, Batteriespeicherstaende
  funktionieren wie im Original und bleiben kompatibel.


--------------------------------------------------------------------------------
  BEKANNTE EINSCHRAENKUNGEN
--------------------------------------------------------------------------------

  Die Eszett-Glyphe wirkt bei 8x8 Pixeln etwas B-aehnlich.

  Die Abspann-Credits bleiben aus technischen Gruenden (eigener
  Zeichensatz) englisch.


--------------------------------------------------------------------------------
  CREDITS
--------------------------------------------------------------------------------

  Uebersetzung, Hacking, Test ........... Karlhungus

  Die Original-Credits des SEGA-Entwicklerteams sind vollstaendig
  erhalten. Es wurde kein Entwickler aus dem Abspann entfernt oder
  ersetzt.


--------------------------------------------------------------------------------
  RECHTLICHES
--------------------------------------------------------------------------------

  Phantasy Star III: Generations of Doom ist urheberrechtlich geschuetzt
  durch SEGA. Dies ist eine inoffizielle, nicht kommerzielle
  Fanuebersetzung, die ausschliesslich als Patchdatei verbreitet wird.
  Sie enthaelt keine geschuetzten Spieldaten.

  Die Weitergabe ist gestattet, solange diese Readme beiliegt und keine
  Gebuehr erhoben wird. Die Verbreitung vorgepatchter ROMs ist untersagt.


--------------------------------------------------------------------------------
  KONTAKT
--------------------------------------------------------------------------------

  YouTube ........... https://www.youtube.com/@rgbretrogaming
  Email ............. rgbretrogaming@protonmail.com


--------------------------------------------------------------------------------
  CHANGELOG
--------------------------------------------------------------------------------

  v1.1  -  30.08.2026  -  Echte Umlaute und Eszett durchgaengig (statt
                          ae/oe/ue/ss); abgeschnittene Textbox in der
                          Hochzeitsszene behoben; Braeute-Auswahl-Text
                          ueberarbeitet
  v1.0  -  04.08.2026  -  Erstveroeffentlichung


================================================================================
