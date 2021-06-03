
# Millimar Software C1202, Incremntal module
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
