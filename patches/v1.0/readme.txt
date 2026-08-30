================================================================================

  PHANTASY STAR III: GENERATIONS OF DOOM
  German Translation / Deutsche Uebersetzung

  Version 1.0
  Release Date: 04.08.2026

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

A note on umlauts: the game's font contains no German special characters.
Umlauts are therefore transcribed the traditional way - ae, oe, ue and ss
instead of the accented letters and the eszett. The text reads
"Schluessel" rather than the accented spelling. This is a limitation of
the original character set, not an oversight.

This is my first ROM hacking project. I worked on it entirely on my own,
using AI both for the translation itself and as technical support for the
script extraction, the alignment of the German and English text blocks,
and parts of the assembly work.

To check the result, I did not rely on spot tests: I recorded a complete
Let's Play of the game in this German version on my YouTube channel and
played it through from start to finish. Every line of dialogue in the
patch has therefore been seen in its actual context, including all three
generations and every branching path of the story.

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
  Patch file:    phantasy_star_3_german_v1.0.bps

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
  CRC32:         C4349C75
  MD5:           88b5040748a5afaaa8eba659990df324
  SHA-1:         a1830b5d3755ac09e08b0fc86acd5bfbc5cc43f7

  The internal Mega Drive checksum has been recalculated and is valid
  (3442). The patched ROM therefore passes the console's own integrity
  check and runs on original hardware.

  The SRAM configuration is unchanged, so battery saves work exactly as
  in the original game. Save files from the unpatched version remain
  compatible.


--------------------------------------------------------------------------------
  5. TESTED ON
--------------------------------------------------------------------------------

  Emulators:     ares, Kega Fusion
  Hardware:      Mega Drive Model 1/2 via flash cart

  The ROM size is unchanged, so the patch works on flash carts and
  reproduction hardware without special requirements.


--------------------------------------------------------------------------------
  6. KNOWN ISSUES
--------------------------------------------------------------------------------

  No issues are known at the time of release.

  Please report text bugs with a savestate or a description of where the
  passage appears. See section 9 for contact details.


--------------------------------------------------------------------------------
  7. CREDITS
--------------------------------------------------------------------------------

  Translation, hacking, testing ......... Karlhungus
  Quality assurance ..................... full recorded playthrough,
                                          see section 1
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

Hinweis zu den Umlauten: Der Zeichensatz des Spiels enthaelt keine
deutschen Sonderzeichen. Umlaute werden daher klassisch umschrieben -
ae, oe, ue und ss statt der Umlautzeichen und des Eszett. Im Spiel steht
also "Schluessel" statt der Schreibweise mit Umlaut. Das ist eine
Beschraenkung des originalen Zeichensatzes, kein Versehen.

Dies ist mein erstes ROM-Hacking-Projekt. Ich habe es vollstaendig
alleine umgesetzt und dabei KI sowohl fuer die Uebersetzung selbst als
auch als technische Unterstuetzung eingesetzt - fuer die Extraktion des
Skripts, die Zuordnung der deutschen und englischen Textbloecke sowie
Teile der Assembler-Arbeit.

Zur Pruefung habe ich mich nicht auf Stichproben verlassen: Ich habe ein
komplettes Let's Play dieser deutschen Fassung auf meinem YouTube-Kanal
aufgenommen und das Spiel von Anfang bis Ende durchgespielt. Jede
Textzeile des Patches wurde damit im tatsaechlichen Spielkontext
gesichtet, ueber alle drei Generationen und saemtliche Handlungspfade
hinweg.

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
  CRC32:         C4349C75
  MD5:           88b5040748a5afaaa8eba659990df324
  SHA-1:         a1830b5d3755ac09e08b0fc86acd5bfbc5cc43f7

  Die interne Mega-Drive-Pruefsumme wurde neu berechnet und ist gueltig
  (3442). Das gepatchte ROM besteht damit die Integritaetspruefung der
  Konsole und laeuft auf Originalhardware.

  Die SRAM-Konfiguration ist unveraendert, Batteriespeicherstaende
  funktionieren wie im Original und bleiben kompatibel.


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


================================================================================
