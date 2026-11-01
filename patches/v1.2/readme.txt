================================================================================

  PHANTASY STAR III: GENERATIONS OF DOOM
  German Translation / Deutsche Uebersetzung

  Version 1.2  (Quality-of-Life Edition)
  Release Date: 01.11.2026

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

Since version 1.1 the font contains proper German umlauts and the eszett,
used throughout the text. The German text of version 1.2 is identical to
version 1.1.

NEW IN 1.2 - QUALITY-OF-LIFE MENU

Version 1.2 adds a comfort menu. Press START on the field (towns,
dungeons, world map) and the game pauses with the menu at the top of the
screen. All settings can be changed at any time and are stored in the
save game. In battles, dialogues, menus and vehicles START keeps working
as the normal pause button.

  Menu controls: Up/Down select, C (or Left/Right) change,
                 B or START close the menu and continue playing.

  a) Random battles ........ on / off  (scripted battles and boss fights
                             are not affected)
  b) EXP and Meseta ........ x1 / x2 / x4 for every battle won
  c) Walking speed ......... fast (double speed, default) / normal.
                             Vehicles and scripted cutscenes always run
                             at original speed.
  d) Battle macros ......... 4 slots, full editor as in Phantasy Star IV:
                             for every party member choose the command
                             (attack, technique, item, defend), the
                             technique or item, and the target.
       Left/Right ... command      C ... next technique / item
       A ............ next target  B ... done (macro is saved)
       "Makro loeschen" clears the slot.

  Battle speed-up: hold the A button during battle and the battle runs
  at double speed. Release A for normal speed.

  Credits: the opening credits and the end credits now list
  "Deutsche Lokalisierung / Karlhungus" (German localization) before
  "Presented by Sega Enterprises".

  Using macros in battle: next to the battle command menu (Auto / One
  round / Orders / Escape) there is a separate field "M" showing the
  current macro slot. Move the cursor right from the Orders icon onto
  "M" and press C. A list of the four macros opens in the top left
  corner (used / empty):
       Up / Down ...... choose a macro
       C .............. execute the macro for one round
       B .............. close the list (Left or B on the "M" field
                        returns to the command menu)
  Macros are created and changed only in the START menu.
  "Auto" afterwards repeats the loaded orders. If a macro uses an item
  that is no longer in the same inventory slot, or a technique the
  character no longer has enough TP for, that character attacks instead.

With the default settings (random battles on, x1) the game plays like the
original, apart from the faster walking speed, which can be switched to
normal in the menu.

This is my first ROM hacking project. I worked on it entirely on my own,
using AI both for the translation itself and as technical support for the
script extraction, the alignment of the German and English text blocks,
the font/character-set work for version 1.1, and the assembly work for
the quality-of-life features in version 1.2.

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

The patch applies to this exact, unmodified ROM only - NOT to a ROM that
already has version 1.0 or 1.1 applied. If your file has a different
size or checksum, the patching tool will refuse it.

No ROM is included with this patch and none will be provided. You must
supply your own copy of the game.


--------------------------------------------------------------------------------
  3. HOW TO PATCH
--------------------------------------------------------------------------------

  Patch format:  BPS
  Patch file:    PSIII_German_v1.2.bps

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

  Size:          1.048.576 bytes  (1 MB / 8 Mbit)
  CRC32:         2298B4CD
  MD5:           4b579110261c890ff6348dddc65eacd2
  SHA-1:         e2a1844bc46b5f86536018894ed07b0d7c5bc453

  The ROM has been expanded from 768 KB to 1 MB to make room for the new
  code. The header (ROM end address) and the internal Mega Drive checksum
  have been updated and are valid (F9F4), so the ROM passes the console's
  own integrity check. 1 MB needs no mapper. Version 1.2 was tested in
  emulators only; it has not been tested on original hardware or flash
  carts.

  Save games: the SRAM configuration is unchanged. The options and macros
  use previously unused bytes of the save slot.
    - Saves from version 1.0 / 1.1 load in 1.2 (defaults: x1, random
      battles on, macros empty).
    - Saves from 1.2 also load in 1.0 / 1.1 (the extra data is ignored).

  Patch file itself:
  Size:          45.840 bytes
  MD5:           f8188cd6b8e0dec3ac8b03e7268b2d5e
  SHA-1:         4e14f2f9eaa6fcb09b7a4725ec49b0d774469d8a


--------------------------------------------------------------------------------
  5. TESTED ON
--------------------------------------------------------------------------------

  Emulator:      ares (manual playtest)
                 Genesis Plus GX (automated test runs)

  Version 1.2 was verified feature by feature in automated emulator runs
  and played through in ares:
  the START menu (all options, macro list, macro editor with techniques,
  items and targets), START still pausing normally in battle and
  dialogue, persistence across new game / save / continue, walking speed
  and party followers, random battles on/off, the EXP/Meseta multiplier,
  the battle speed-up and all battle macro functions. Text and all game
  data outside the 17 patched code locations are byte-identical to 1.1.
  The ROM is built from the disassembly source with the Macroassembler
  AS.


--------------------------------------------------------------------------------
  6. KNOWN ISSUES
--------------------------------------------------------------------------------

  The eszett glyph looks slightly B-like at the game's native 8x8 pixel
  resolution.

  The end credits remain in English (they use their own, separate
  character set).

  Macros store the orders per party position. If the party order changes
  (e.g. a new member joins), check your macros again.

  Please report bugs with a savestate or a description of where the
  problem appears. See section 9 for contact details.


--------------------------------------------------------------------------------
  7. CREDITS
--------------------------------------------------------------------------------

  Translation, hacking, testing ......... Karlhungus
  Quality assurance ..................... full recorded playthrough (v1.0),
                                          rebuild/diff verification (v1.1),
                                          automated emulator tests (v1.2)
  Tools ................................. Floating IPS (Flips),
                                          The Macroassembler AS,
                                          custom script tooling

  The original SEGA staff credits are preserved in full. No developer
  has been removed from or replaced in the in-game credit roll. Since
  version 1.2, the opening and end credits additionally list "Deutsche
  Lokalisierung / Karlhungus" before "Presented by Sega Enterprises".

  Thanks to the ROMhacking.net community for the documentation and
  utilities that made a first project like this possible. The battle
  macros are inspired by Phantasy Star IV.


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

  v1.2  -  01.11.2026  -  Comfort menu on START: random battles on/off,
                          EXP/Meseta x1/x2/x4, walking speed, battle macro
                          editor (4 slots, own "M" field in battle); battle
                          speed-up (hold A); credits list "Deutsche
                          Lokalisierung / Karlhungus" in opening and end
                          credits; ROM expanded to 1 MB; fixed shifted
                          text speed window after "continue" (bug of the
                          original game)
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

Seit Version 1.1 enthaelt der Zeichensatz echte deutsche Umlaute und das
Eszett. Der deutsche Text von Version 1.2 ist identisch mit Version 1.1.

NEU IN 1.2 - KOMFORTMENUE

Version 1.2 bringt ein Komfortmenue. START im Feld (Staedte, Dungeons,
Weltkarte) druecken: Das Spiel pausiert, oben erscheint das Menue. Alle
Einstellungen lassen sich jederzeit aendern und werden im Spielstand
gespeichert. In Kaempfen, Dialogen, Menues und Fahrzeugen bleibt START
die normale Pausetaste.

  Bedienung: Hoch/Runter waehlen, C (oder Links/Rechts) aendern,
             B oder START schliessen das Menue und setzen das Spiel fort.

  a) Zufallskaempfe ........ an / aus (geskriptete Kaempfe und
                             Bosskaempfe sind nicht betroffen)
  b) EXP und Meseta ........ x1 / x2 / x4 fuer jeden gewonnenen Kampf
  c) Laufen ................ schnell (doppeltes Tempo, Standard) /
                             normal. Fahrzeuge und Zwischensequenzen
                             laufen immer im Originaltempo.
  d) Kampf-Makros .......... 4 Plaetze, voller Editor wie in Phantasy
                             Star IV: je Gruppenmitglied Befehl
                             (Angriff, Technik, Gegenstand, Abwehr),
                             Technik bzw. Gegenstand und Ziel waehlen.
       Links/Rechts ... Befehl     C ... naechste Technik / Gegenstand
       A .............. Ziel       B ... fertig (Makro wird gesichert)
       "Makro loeschen" leert den Platz.

  Kampf-Turbo: A-Taste im Kampf gedrueckt halten, der Kampf laeuft
  doppelt so schnell. A loslassen = normales Tempo.

  Credits: Im Vorspann und im Abspann steht jetzt "Deutsche
  Lokalisierung / Karlhungus" vor "Presented by Sega Enterprises".

  Makros im Kampf: im Kampf-Befehlsmenue (Auto / Eine Runde /
  Einzelbefehle / Flucht) liegt rechts ein eigenes Feld "M" mit der
  aktuellen Makro-Nummer. Cursor vom Einzelbefehle-Symbol nach rechts
  auf "M" bewegen und C druecken. Links oben oeffnet sich eine Liste
  der vier Makros (belegt / leer):
       Hoch / Runter .... Makro waehlen
       C ................ Makro eine Runde lang ausfuehren
       B ................ Liste schliessen (Links oder B auf dem Feld
                          "M" fuehrt zurueck ins Befehlsmenue)
  Angelegt und geaendert werden Makros nur im START-Menue.
  "Auto" wiederholt anschliessend die geladenen Befehle. Liegt ein im
  Makro verwendeter Gegenstand nicht mehr im selben Inventarfach oder
  reichen die TP fuer eine Technik nicht mehr, greift die betreffende
  Figur stattdessen an.

Mit den Standardwerten (Zufallskaempfe an, x1) spielt sich das Spiel bis
auf das schnellere Laufen wie das Original; das Lauftempo laesst sich im
Menue auf normal stellen.

Dies ist mein erstes ROM-Hacking-Projekt. Ich habe es vollstaendig
alleine umgesetzt und dabei KI sowohl fuer die Uebersetzung selbst als
auch als technische Unterstuetzung eingesetzt - fuer die Extraktion des
Skripts, die Zuordnung der deutschen und englischen Textbloecke, die
Zeichensatz-Arbeit fuer Version 1.1 sowie die Assembler-Arbeit an den
Komfortfunktionen in Version 1.2.

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

  Der Patch laesst sich ausschliesslich auf dieses unveraenderte ROM
  anwenden - NICHT auf ein ROM mit Version 1.0 oder 1.1. Ein ROM liegt
  nicht bei und wird auch nicht bereitgestellt.


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

  Groesse:       1.048.576 Bytes  (1 MB / 8 Mbit)
  CRC32:         2298B4CD
  MD5:           4b579110261c890ff6348dddc65eacd2
  SHA-1:         e2a1844bc46b5f86536018894ed07b0d7c5bc453

  Das ROM wurde fuer den neuen Code von 768 KB auf 1 MB erweitert. Header
  (ROM-Ende) und interne Mega-Drive-Pruefsumme wurden angepasst und sind
  gueltig (F9F4), das ROM besteht die Integritaetspruefung der Konsole.
  1 MB braucht keinen Mapper. Version 1.2 wurde nur in Emulatoren getestet;
  auf Originalhardware und Flashcarts ist sie nicht getestet.

  Spielstaende: Die SRAM-Konfiguration ist unveraendert. Optionen und
  Makros liegen in bisher ungenutzten Bytes des Speicherplatzes.
    - Spielstaende aus 1.0 / 1.1 laufen in 1.2 weiter (Standardwerte:
      x1, Zufallskaempfe an, Makros leer).
    - Spielstaende aus 1.2 laufen auch in 1.0 / 1.1 (die Zusatzdaten
      werden dort ignoriert).


--------------------------------------------------------------------------------
  BEKANNTE EINSCHRAENKUNGEN
--------------------------------------------------------------------------------

  Die Eszett-Glyphe wirkt bei 8x8 Pixeln etwas B-aehnlich.

  Die Abspann-Credits bleiben aus technischen Gruenden (eigener
  Zeichensatz) englisch.

  Makros speichern die Befehle je Gruppenplatz. Aendert sich die
  Reihenfolge der Gruppe (z. B. durch ein neues Mitglied), die Makros
  bitte neu pruefen.


--------------------------------------------------------------------------------
  CREDITS
--------------------------------------------------------------------------------

  Uebersetzung, Hacking, Test ........... Karlhungus

  Die Original-Credits des SEGA-Entwicklerteams sind vollstaendig
  erhalten. Es wurde kein Entwickler aus dem Abspann entfernt oder
  ersetzt. Seit Version 1.2 nennen Vor- und Abspann zusaetzlich
  "Deutsche Lokalisierung / Karlhungus" vor "Presented by Sega
  Enterprises". Die Kampf-Makros sind an Phantasy Star IV angelehnt.


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

  v1.2  -  01.11.2026  -  Komfortmenue auf START: Zufallskaempfe an/aus,
                          EXP/Meseta x1/x2/x4, Lauftempo, Makro-Editor
                          (4 Plaetze, im Kampf eigenes Feld "M"); Kampf-
                          Turbo (A halten); Credits "Deutsche
                          Lokalisierung / Karlhungus" in Vor- und Abspann;
                          ROM auf 1 MB erweitert; verschobenes
                          Textgeschwindigkeits-Fenster nach "Spiel
                          fortsetzen" behoben (Fehler des Originals)
  v1.1  -  30.08.2026  -  Echte Umlaute und Eszett durchgaengig (statt
                          ae/oe/ue/ss); abgeschnittene Textbox in der
                          Hochzeitsszene behoben; Braeute-Auswahl-Text
                          ueberarbeitet
  v1.0  -  04.08.2026  -  Erstveroeffentlichung


================================================================================
