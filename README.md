
# Millimar Software C1202, Incremntal module
### **FW ver 0.8.0.9 / 16.07.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.9/C1202.bin)**
- Einrichten neue Name: "SENSOR" statt "ABSOLUTE"
- Inkremental modul - Parameter: Analoge werte mit Max Anzeige ("gitterkonstante", "ink. pro. Umdreh", "Anzahl Ref. pro U.", "Dist. zwisch. ref.")
- Referenzierung behoben (Messanzeige und Einrichten)
- Fehler reset in Einrichten unter Tatse 5
- Modulfehler (bzw. Kanalfehler) wird als ERR5 ("Daten unvollständig") in MarCom uebertragen statt messwert 
- Inkrementalsensor automatisch Aufloesung anpassung nach dem Gitter konstante und Interpolation Faktor:
  - gilt nur fuer Linear taster und fuer laenge aufloesung
  - berechnet wird nach: resol_f [mm] = gitterkonstante [um] / interpolation_faktor / 1000
      ```c
  	  // resolution boundaries:
	    if (resol_f >= 0.005)
		    result = 0; // i.e. 0.01 mm
	    else if ( (resol_f < 0.005) && (resol_f >= 0.0005) )
		    result = 1; // i.e. 0.001 mm
	    else if ( (resol_f < 0.0005) && (resol_f >= 0.00005) )
		    result = 2; // i.e. 0.0001 mm
	    else if (resol_f < 0.00005)
		    result = 3; // i.e. 0.00001 mm
	    else
		    result = 3; // i.e. 0.00001 mm
    ```
  - auf groesste mogliche Aufloesung es wurde automatisch gaendert
  - wenn 2 kanaele sind in Verknoepfung: Groeste afulesung ausgewertet ist
  - Aufloesung liste ist automatisch gekurtzt
- Phasenkorrektur ist nicht brechbar moeglich (messmodul in phansenkorrektur marnet schnittstelle ist nicht aktiv)
- Firmware update von menu:
  - dateinahme mit verion info in menu angezeigt (jetzt alle, in Zukunft nur neueste FW wird gezeigt)
  - dateiname wird geprueft ("z.B.: C1202_FW_0.8.0.9.bin")
  - nach dem langetsasterdruck wird restet drurgefuehrt
  - Taste 1 ist nur fuer bestrommung sicherheit
  - C1202.bin wird nicht in menu gezeigt

### **FW ver 0.8.0.8 / 09.07.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.8/C1202.bin)**
- fix - Inkrmentalmodul parameter in "Gitterkonstante", "Inkremente pro umdrehung", "Anzahl Ref. pro U." u. "Dist. zwisch. Ref." editierung mit maximale Werte verbessert
- fuer induktive module gruenepunkt nicht blinkend
- Inkrementalmodul Parameter - positionierungs verbessert
- Inkrementalmodul Parameter - parmater speicher detektion verbessert
- fix - pinAccess wenn eingestellte pin ist 0000, wird auch gefragt
- "Fehlermeldungsfenster Aktiv." von Setup 1 -> Setup 3 
- alle neue komentaere (Inkrementalmodul parameter und fehleranzeige) von wuerterbuch gezeigt (jetzt nur Deutsch und englisch)
- erste start fehler erkennung und referenzierung - fix
- Inkrementalmodul parameter Tastenbeschreibung fuer "checkbox" angepasst (wie in Fussschalter)
- Werkseinstellung: modul wird nicht gefragt nach parametern die sind nicht modulrelevant, dadurch kein lesefehler wird nicht gezeigt
- Messanzeige meldefenster management, bzw. Fehler meldungen
- speicher optimalisierung


### **FW ver 0.8.0.7 / 25.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.7/C1202.bin)**
- Tolernaz und Warngrenzen fuer winkel in inkremental modul
- optimisierung von Inkrementalmodul parameter behandlung entMultiPar() modul:
  - neu state-basierte struktur
  - Leistung, speicher und zuverlaessigkeit verbesserung
  - Modul antwort fehler bearbeitung (wenn modul shickt keine antwort - wird nicht gefroren)
  - Phasekorrektur durchfuhrung fehlerbehandlung verbessert
  - Phasenkorrektur durchfuehrung anhalten moeglichkeit (anhalten von Inkrementalmodul ist nicht moeglich ?)
- Inkremantal modul Fehler fenster Nachricht geaendert
- Zaehler reset in "Absolute" mode unter Taste 5
- Name fuer Einrichten geaenderet nur fuer Inkremntal modul
- Fix: induktivmessmodul: zeigt Messwerte und Referenzpunkt ist statisch

### **FW ver 0.8.0.6 / 17.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.6/C1202.bin)**
- fix: Kundekorrektur korrigiert (4-auswahl)
- neu: Referenzpunkt logik angepasst
- neu: gruen/rot punk an Anzeige gaeendert:
  - Gruen wenn messung leuft,
  - Dunkelrot wenn messung angehaltet,
  - blinkend Gruen oder Dunkelrot wenn Inkremental Taster nicht referenziert
  - Rot wenn Messmodul Fehler geschickt hat
- neu: dynamische Menu: 
  - "Tastertyp" (Induktive oder pneumatische Modulen) oder "Sensortyp" (Inkremntale Modulen)
      je nach dem welches Messmodul angeschlossen ist
  - Kundenkorrektur wenn Inkrementalmodul angeschlossen ist - wird nicht angezeigt
  - Aufloesung erhoerung fuer Inkrementalmodul (wie bei HR modul)
  - multiturn korigiert
  - Einrichten fuer drehgeber angepasst
  - korrigiert und verbessert analoganzeige skala fuer Inch und Radiant,
    - skala "ticks" briete angepasst fuer alle Einheten
  - Fehlermeldungsfenster in Messeuzeige fuer Messmodul Fehler:
    - neu Fehlermesde fenster
    - bis 10 letzen Fehler wird gezeigt.
    - fehleranzeige wechsel nach jede sekunde
    - Fehelrhaftekanal wird gezeigt
    - normalarbeit nach fehlervermeidung (wenn meesmodul erlaubt)
    - fehlerbeschreibung und vermoetliche urhsache

### **FW ver 0.8.0.5 / 10.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.5/C1202.bin)**

- fix von 0.7.9.0:
  - Werte plausiobilitaet proefung, keine Diskette u. blinkende Pfeil wenn werten sind nicht plausibel
  - kundenkorrektur duerfuehrung falsches Fehler (timeout fenster)
- Referenz Marke bearbeitung und auf dem Messanzeige zeigen
- Marnet Fehler reaktion modulen:
  - zeigen als rotepunkt in messmodulen
  - 10 leztze Fehler registrieren
  - diese fehler in Info-seite wird uter der Taste T5 gezeigt
- Lesen drehgeber:
  - singleturm mit und ohne referenzmakre
  - multiturn - anzahle umdrehungen sind multipliziert 360 Grad
- Formel anpassung nach drehgeber aktivierung:
  - Verknuepfung limitiert wenn einkanal ist linear und andere ist rotativ. Wenn beide dleis sind, verknoepfunk ist nicht limitiert
  - Funktion fuer Merkmale wenn in verknoepfung drehgeber implementiert ist, ATAN ist nicht auswahlbar
- Menu anpassug fuer Drehgeber: winkeleincheiten sind aktiv
- fix: diagnosis Zaehler nullen vervbessert
- in Menue als parameter ist auch sensortyp gezeigt, entweder Drehgeber oder Lilnear Tatser
- neue skalen fuer inkremental modul:
  - fuer laenge: zusaezliche 30 mm, 
  - fuer winkel: zusaetzliche 360 Grad
- andere fixen und verbesserungen

### **FW ver 0.8.0.4 / 02.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.4/C1202.bin)**
- inkrmental: linear werte lesen und zeigen
- einfache diagnostic ueber MarCom (7 zaehler)
- Keine Antwort von Modul Fehler Nachricht Anzeige 
- Forel, T&W und 2P-Meister: Paremeter geendert in Titel Anzeige, von "*" fuer Farbe Grau
- Forel, T&W und 2P-Meister: Parameter editierung: pfeil bleibt permanent
- Inkremental modul Parameter: springen ueber ausgegeute Werte
- Inkremental modul Parameter: Referenz punkte logik: erst muss Referenz Punkte bearbeitung aktiviert sein
- INkremental Anzeige: blinkende Kreiss wenn Taster nicht referneziert ist


### **FW ver 0.8.0.3 / 28.05.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.3/C1202.bin)**
- demos fuer Geschwindigkeit und Umdrehungen entfernt
- neues bedien konzept fuer Formel, Toleranz&Wangrenzen und 2P-Meister implementiert
- Incremental Modul parametrierung verbesserung:
  - Shift Phase correction prozedure implementiert (ablaufzeit, neu wert anzeige, fehler anzeige, Tasten aktiv)
  - 2-Kanllen bearbeitung
  - min-max Werte bearbeitung mit aktive Speicher moeglichkeit
  - Fehler bearbeitung - paramater lesen (meldung mit fensetr)
  - Automatische Parameter aenderung am Start fuer Differenz messun (Geschwindigkeit)
  - "Messaufgabe" statisch ausgegraut und nicht editierbar.
  - kleine fixen
- vorbereitunng fuer messwerte lesen

### **FW ver 0.8.0.2 / 21.05.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.2/C1202.bin)**
- bugfix - wizzard, kein einheit auswahl
- N1702 VSS parameter lesen und zeigen
- Neu N1700 PC SW anpassung:
  - Anzahl Referenzpunte, von Liste auf Checkbox
  - gitterkonstante mit 100um genauigkeit
  - aphaengigkeiten zwischen "Count ref. points" und "Reference punkt. processing"
  - phase shift correction Wert anzeige
- parameter aenden, senden und speicher in Messmodul. 
- Ziffer editierung richtung zurueckumgesetzt
- Formel beispiel fuer geschwidigkeitund Anzahl Umdreungen
---
### **FW ver 0.8.0.1 / 06.05.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.1/C1202.bin)**
- Inkremental Modul erkennung und bearbeitung, neu artikelnummer, modul typ evaluierung nach Artickelnummer nicht Name
- Tastertyp menu angepasst fuer modulparamater nach PC-SW N1700:
- namen angepasst
- Listen angepasst,
- dynamische menu:
  - wechsel zwischen "gitter Konstante" und "inkremente pro umdreh", "Anzahl Referenzpunkte pro Umdreh" und "Distand zwischen Referenzpunke" nach sensorTyp: "Linar" und "Rotary"
  - nicht aktive parameter
  - phase shift korrektur durchfuhren
  - interaktive Referenzpunkt proc nach zustand der Anzahl Referenzpunkte
  - kries-navigation fuer parameter
- Anzeige parameter neu: (1) Position, (2) Geschwindigkeit, (3) Anzahl Umdrehungen
- Anpassung einheit in Messanzeige
- Kreiss - scrollen in Menu
---
### **FW ver 0.8.0.0 / 06.05.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.0/C1202.bin)**
- neu Tasteryp menu fuer inkremental modul

# Millimar Software C1202, Inductive modules
FW ver 1.0.0.1 / 01.07.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/1.0.0.1/C1202.bin)
- Werkseintellung ohne software reset: nach automatisches restart nicht immer hochgelaufen, neu:
  - nach werkseinstellung, reset wird nicht durchdefuehrt, statt wizzard startet dirakt
- fix 4800 kbps bei ersten start

FW ver 1.0.0.0 / 29.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/1.0.0.0/C1202.bin)
- Name änderung
- 
FW ver 0.7.9.0 / 02.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.9.0/C1202.bin)
- neues Bedienkonzept für Formel, Toleranz&Warngrenzen und 2P-meister:
  - diskette für speicher
  - parameter änderung überwachung
  - binkende pfeil nach oben wenn parametern geändert sind
  - graue titel wenn parametern geändert sind
- menu bedienung "im kreiss"
- modul antwort WD überwachung mit Meldungsfenster
- dignose zehler implementiert, über MarCom verfügbar

FW ver 0.7.8.9B / 10.05.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.9B/C1202.bin)
- werkseinstellung delay
- Fussschalter - am ersten start avtiviert
- MarCom baudrate 4800bps am ersten start entfernt

FW ver 0.7.8.9A / 29.04.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.9A/C1202.bin)
- automatisch testen AT?STD - werkseintellung
- AT?SCR=filename.bmp
- send UART message on Hard Fault

FW ver 0.7.8.9 / 21.04.2021:  [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.9/C1202.bin)
- bug fix, wenn Anzahl Merkmall ist 1 - C1202 startet nicht.

FW ver 0.7.8.8A / 19.04.2021:  [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.8A/C1202.bin)
- Sprache: Spanish aktualisiert (mit Font)
- fix, bug-ID: 45848 - meister Wert editierung verbesserung. Jetzt kann man erst kleinerwert editieren statt groser als erster schritt. Wird das nicht direkt mit default Werte umgesetzt. Werte Plausibilitaetproefung wird erst bevor speicher geprueft und Wertenm werden nicht automatisch ungestzt, sondern gelb-markiert. Diese Funktion war nur gedacht fuer parameter von par-datei lesen (SD-speicherkarte). Und so jetzt funktioniert.
- Gleiche Logik fuer Toleranz und Warngrenzen ralisiert
- Artikelnummer Aktualisiert fuer: 5312025

FW ver 0.7.8.8 / 15.04.2021:  [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.8/C1202.bin)
- seriennummer und artikelnummer werden nicht von par-datei uebernohmen
- anpassung fuer fertigungstools: Seriennummer erset FW ladung: 0 und erste start MarCom mit 4600bps (das kommt von C1200) sn-werkzeug bps ist festkodiert
- "Kein modul" verbesserung - screenshot und tastendrueck verbessrung

FW ver 0.7.8.7 / 13.04.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.7.8.7/C1202.bin)
- Erste start verbessert und optimiert: Zeitenm, artikelnummer und seriennummer richtig eingestellt
- eerpom erase moeglich um Erst Start zu simulieren
