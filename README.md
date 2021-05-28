[all versions](https://github.com/k-szczeciak/C1202RelOpen)
# Millimar Software C1202, Incremntal module
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