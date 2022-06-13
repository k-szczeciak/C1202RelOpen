[all versions](https://github.com/k-szczeciak/C1202RelOpen)
# Millimar Software C1202, Incremntal 
### **FW ver 0.8.4.3 / 02.06.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.4.3/C1202_FW_0.8.4.3.bin)**
-	fix: Inkrementalmodul Parameter
-	fix: entTxt Titel länge Anpassung
-	MarCom "MSG=...$0G" Befehl endlos Zeit Nachricht eingeführt
-	fix: Datei-Änderung verbessert
-	Sprache Aktualisierung - Französisch

### **FW ver 0.8.4.2 / 25.05.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.4.2/C1202_FW_0.8.4.2.bin)**
-	MarCom Schnittstelle verbessert: jetzt für anfrage für mehrere Werte (z.B. „TOL?“)  nach jede ‘;‘ wird Befehl widerholt, z.B. „TOL1 …“
- 	Fix: werte Mappings für Anfrage angepasst
-	Bildschirmkopie in Messbild Anzeige:
- 	Wird automatisch angepasst
-	Graph Anzeige mit Toleranz und Warngrenzen Fläche verbessert:
  - Getestet mit Toleranz, Toleranz mit Warngrenzen, Skalierung und Zentrieren auf Nennmaß oder Toleranz
-	Messanzeige: Zeiger: Skalierung Weiße Linie entfernt
-	Sprache und Font update. Nur FR, PT und ES sind nicht vollständig übersetzt
-	Messanzeige Verbesserungen:
  -	Graph: Digital anzeige Vertikal Positionierung:
  -	Graph und Digital: Weisses Strich in Tolernz aktiv entfent 
  -	Andere

### **FW ver 0.8.4.1 / 20.05.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.4.1/C1202_FW_0.8.4.1.bin)**
-	fix: Messanzeige Toleranz und Warngrenzen Anzeige in Balken und Zeiger - nicht sichtbar wen außer Skalierung
-	upgrade: wenn keine Sprache installiert ist, nur Kurtz druck für Sprache Installierung ist nötig
-	upgrade: Bildschirmkopie Aktivierung Anzeige mit Ikone:    Sichtbar überall außerdem Messanzeige	
-	fix: nach Werkseinstellungen Installierte Sprache ist verfügbar und Auswahl in Wizzard (Sprache Installierung Option in Wizzard nicht möglich)
-	fix: Messanzeige Einheit nicht sichtbar - behoben
-	update Sprachen: DE, EN, PT, ES, 
-	MarCom update:
  - "?" immer alle 3 Merkmale mit entsprechendem Fehler anzeige: z.B.: "1 0.000 mm;2 ERR6;3 ERR6" ERR6 - Merkmal nicht verfügbar , ERR5 - Messung nicht gültig (z.B. Sensor nicht angeschlossen), ERR3 - Messung nicht verfügbar, z.B. 2P-messung läuft
  - "Mx?" ohne Merkmalnummer Bezeichnung,
  - "TOL?", "TOLW?", "NOMINAL?", "MASTER?" umgeordnet und mit ";" Trennung
  - neue befehle: "TOLx?", "TOLWx?", "NOMINALx?", "MASTERx?" für Einzelmerkmal anfrage
  - Schreibfunktionen: "TOLx", "TOLWx", "NOMINALx", "MASTERx", Antwort ohne Werte-Bestätigung, Bestätigung nur mit Befehl, z.B.: "TOL1/r"
  - "ID?" Antwort umstrukturiert, Beispiel: "ID1 T 005312025 S 00010000;ID2 T 5331161 S 00000000"
  - "DES?" Antwort umstrukturiert, Beispiel: "DES1 Mahr Millimar C1202;DES2 N 1702 VSS" 
  - "VER?" Antwort umstrukturiert, Beispiel: "VER1 0.8.4.1;VER2 V1.1.5a" 
  - Neue Befehle: "BRAND_<BRAND>_1861" und "DEVICE_<DEVICE>_1861":
    - BRAND und DEVICE sind maximal 10 Zeichen breit (ASCII nur)
    - BRAND und DEVICE sind intern in Eeprom gespeichert
    - BRAND und DEVICE sind einstellen möglich nur wenn keine bekannte Artikelnummer eingestellt ist. Tabelle ist automatsch generiert und intern gespeichert in FW): 
    - Um BRAND und DEVICE zu einstellen Artikel Nummer muss erst eingestellt außer Liste sein
    - wenn Artikel Nummer zurück zum Artikel von liste eingestellt ist, eingestellte DEVICE und BRAND wird gelöscht
    - es ist möglich BRAND und DEVICE löschen mit Befehl: "BRAND_1861" oder "DEVICE_1861"
    - Wenn BRAND oder DEVICE nicht eingestellt oder gelöscht ist, dann Standardwerte sind übernehmen: für DEVICE: "Millimar C1202", fuer Brand: "Mahr"
    - es ist möglich Leer BRAND oder DEVICE machen mit Befehl: "BRAND__1861" oder "DEVICE__1861" (Doppel Leerzeichen)
    - Antwort für Befehl "DES?" ist folgendes: Standard: "DES1 Mahr Millimar C1202;DES2 N 1702 VSS", mit Brand und Device: "DES1 MyBrand MyDevice;DES2 N 1702 VSS", nur Brand: "DES1 MyBrand;DES2 N 1702 VSS", nur Device: "DES1 MyBrand;DES2 N 1702 VSS"
    - Eingestellte BRAND und DEVICE wird in Info-seite gezeigt, in MarCom, in CSV-Datei, und Start -Bild:

### **FW ver 0.8.4.0 / 12.05.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.4.0/C1202_FW_0.8.4.0.bin)**
-	fix: Inkremental Module Parameter Fix (falscher Font für Werte)
-	fix: Fehlende Zeichen in Standardfont
-	fix: Font Anpassung in Formel - fehlende Zeichen.
-	update: Sprache Auswahl
  -	"(Sprache installieren)" jetzt in ausgewählte Sprache und einsprechenden Font, anderes als installierte Sprache
  -	Trennung der Name und "()"
-	fix: Zeiger und Balken Anzeige in außerhalb Scala behoben
-	Dateiliste Anzeige (Parameter, FW update, Messdaten):
  -	fix: mehrere Seiten Bewegung mit Tasten 4 und 5 Rückgang moeglich
  -	neu: Lange tastedrueck Tasten 4 und 5 Seitensprung
  -	neu: unabhängig von installierter Sprache und Font, Dateinahmen immer in Standartfont gezeigt
  -	neu: Schriftausrichtung links statt mittel
-	MarCom Befehlssatz update:
  -	Mx? ohne Merkmalnummer
  -	TOL? Antwort mit TOL1...
  -	TOLx? implementiert
  -	TOLW? Antwort mit TOLW1...

### **FW ver 0.8.3.9 / 1.05.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.9/C1202_FW_0.8.3.9.bin)**
- INtsalierbare sprachen, Version wo Font für Menue->Formel->Funktion Auswahl implementiert ist.
  2 Font-Sätze werden bei Sprache Installierung implementiert.

### **FW ver 0.8.3.8a / 28.01.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.8a/C1202_FW_0.8.3.8a.bin)**
- Version mit 7 sprachen(DE, CN, CZ, EN, FR, IT, PL)
  fehlt noch 4 sprachen(PT, RU, ES, SE)

### **FW ver 0.8.3.8 / 29.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.8/C1202_FW_0.8.3.8.bin)**
-	"EER7 - Menue aktiv" wird ersetzt mit "EER3 - Auftrag kann nicht ausgeführt werden" 
-	"ERR5 - Daten unvollständig" Korrektur, allein ohne Merkmal Nummer, 
-	fix: Marcom,  Zeitgesteuerte Messung:  wenn Modulfehler, "START"-befehl ist nicht möglich
-	Installierte Sprache wird am Start:
  -	Installierte Font wird geprüft ob gültig ist
  -	Installierte Wörterbuch wird, geprüft ob gültig ist
  -	Wenn Installierte Sprache nicht gültig ist und Installierte Sprache aktive ist, Wizzard wird ausgeführt.
  -	Bei neu FW update, und aktives Installierte Sprache, Wizzard wird ausgeführt
  -	Wenn Installierte Sprache nicht gueltig ist, diese option wir nicht in wizzard gezeigt
  -	Wenn INstallierte Sprache gueltich ist, diese option wird gezeigt
-	"Checkbox unchecked" und "Checkbox checked" wird in getrennten Font benutzt statt Standard Microsoft YaHei - sichtbar in installierte Sprache
-	Umsetzung "/x0A" oder "/r" von Text String zu ASCII wert bei Sprache Installierung
-	Bei Sprache Installierung Version von Datei und aktuellen FW geprüft werden (in diese Version 3 erste nummern, letzte wird nicht geprüft)
-	Formel-->Funktion Auswahl bei Installierte Sprache englische Wörterbuch wird benutzt

### **FW ver 0.8.3.7b / 22.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.7b/C1202_FW_0.8.3.7b.bin)**
- linie und Fette linie

### **FW ver 0.8.3.7a / 22.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.7a/C1202_FW_0.8.3.7a.bin)**
- version wo in Graph/Füll Warngrenzen implementiert sind

### **FW ver 0.8.3.7 / 22.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.7/C1202_FW_0.8.3.7.bin)**
-	fix: FW upgrade falsche Datei richtige Datei übernehmen würde,
-	geprüft: Artikelnummer bei Neugerät würde 5312025 automatisch gesetzt (Serialnummer 00000000), wenn keine andere ist geschrieben
-	Wizzard Seite Tastenbeschreibung korrigiert (Flasche USB-Schnittstelle und blinkende "Ausgang" Taste)
-	Sprache instalation:
  -	Sprachedatei geprüft nach Anzahl Einträge (wenn sprach Datei hat wenige eintrage, fehlende werden mit "no entry" automatisch nachgefühlt)
  -	Sprachdatei nach Version Nummer geprüft
  -	Sprachdatei wird nach Font geprüft
  -	Sprachdatei wird nach Checksumme (MD5 hash wird berechnet und vergleicht mit gespeicherte)
  -	Checksumme wird mit "Saltz" gepflegt.  Zusammen mit Hash wirkt als ein Digitales Unterschrift für sprach Datei.
  -	"Ungültige Datei" Fenster wird gezeigt, wenn Prüfung nicht positiv abgelaufen ist.
-	Graph Anzeige, für Modus verbessert (Warngrenzen immer noch nicht implementiert in diese Modi)

### **FW ver 0.8.3.6 / 8.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.6/C1202_FW_0.8.3.6.bin)**
-	Graph anzeige Beispiele:
-	Menü:
  -	Pixel (Standard bis letzte Version)
  - Pixel Fett (3pixel) 
  - Linie
  - line Fett (3 pixel)
  - Füll

### **FW ver 0.8.3.5 / 01.04.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.5/C1202_FW_0.8.3.5.bin)**
-	Letzte Listenposition Anzeige in Menü - jetzt sichtbar
-	speicher optimiert und reduziert
-	Sprache Installieren:
  -	Sprache wird mit eigenem Font installiert
  -	 automatische installierte Sprache Übernahme
  -	nach werkseinstellung, Installierte Sprache wird aktiv
  -	Neuer Font aktiv global (außer Formel-Funktion Auswahl)

### **FW ver 0.8.3.4 / 18.03.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.4/C1202_FW_0.8.3.4.bin)**
-	Millimar Tool Upload sicher
-	scrollen in listen im kreiß
-	listen Anzeige verbessert (Antwort Zeit)
-	installierbare Sprachen:
  -	Datei Name: ".lng"
  -	Menue Sprache, letzte Zeile: installieren mit Lange Tastendruck, Auswahl mit Kurze Tastendruck
  -	Wörterbuch wird auf Flash kopiert (256 positionen moeglich, 183 in version 0.8.3.4 belegt, 8kB) 
  -	Datei löschen nicht möglich

### **FW ver 0.8.3.3 / 11.03.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.3/C1202_FW_0.8.3.3.bin)**
-	fix: Parameterdatei entfernen 
-	keine Datei Auswahl und Pfeil-navigation Verbesserung
-	FW update Datei Prüfung Verbesserung (Backup Datei Update möglich)
-	Upload Verarbeitung

### **FW ver 0.8.3.2 / 25.02.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.2/C1202_FW_0.8.3.2.bin)**
-	Sprache update für PL, EN und DE
-	Datei Upload fortschrittanzeige
-	Datei unterladen Anzeigefenster
-	MarCom: Datei Liste mit Beschreibung und Dateigröße
-	MarCom: Datei-empfangen für Byte-datei erweitert
-	Sprache Installierung von SD-Karte - Menü Auswahl nur.
  -	Sprache Datei Beispiel im Anhang

### **FW ver 0.8.3.1 / 18.02.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.1/C1202_FW_0.8.3.1.bin)**
- updtae für MillimarTool

### **FW ver 0.8.3.0 / 28.01.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.3.0/C1202_FW_0.8.3.0.bin)**
- fix: Meister fuer Drehgeber und referenzpunktbearbeitung. Nur relevanten kanal wird zuruckgesetzt
- upgrade: erweitere information fuer Parameter-datei verbessert
- update: Wuerterbuch Deutsch
- update: Wuerterbuch FR und CN - nicht gezeigte Nachrichten in Kundenkorrektur durchfuehrung
- fix: falsche Erste anzeige fuer aktive Korrektur in menu
  
### **FW ver 0.8.2.9 / 25.01.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.9/C1202_FW_0.8.2.9.bin)**
- aktive parameter anzeige:
  - parameter aenederung Anzeige mit "*"
  - MarCom aktive datei uebertragung
- parameter-Datei mit Beschreibung
- fix: parameter anzahl bis 99 fuer gleiche 
- folder zuordnung:
  - /csv fuer csv-Datei
  - /par fuer parameter-Datei
  - /bmp fuer bildschirmkopie
- Marcom Schnittstelle fuer Datei:
  - unterordner Anfrage
  - Datei-filtrierung

### **FW ver 0.8.2.8 / 13.01.2022: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.8/C1202_FW_0.8.2.8.bin)**
- x-mass Edition entfernt
- Modul FW Evaluierung Verbesserung und Info-Seite
- Info-seite Einzel Pneumatisches Modul anzeige Verbesserung
- 2-Punkt Meister nicht plausible Werte Meldungsfenster
  - 2 Sekunden Meldungsfenster Dauer
  - Anzeige Welche Merkmal nicht plausibel ist
- Inkremental Modul Fehler Quittierung von Messanzeige
- Wörterbuch update
- Meldungsfenster Verbesserungen
---
### **FW ver 0.8.2.7 / 24.12.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.7/C1202_FW_0.8.2.7.bin)**
- Drehgeber mit Referenzpunt Fix fuer Extreme Werte (Min, Max)
- Faktor auch fuer Inkrementale module.
---
### **FW ver 0.8.2.6 / 22.12.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.6/C1202_FW_0.8.2.6.bin)**
- bugfix 46920 - Toleranz ausschalten
- Drehgeber ohne Referenz Meistern bei maximale anzeigewerte ~19999 grad
- xmass edition
- inkremental Modul parameter speicher Fix
---
### **FW ver 0.8.2.5 / 09.12.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.5/C1202_FW_0.8.2.5.bin)**
- Deutsch, Englisch und Polish Wuerterbuch update
- par-Datei lesen sprache wir ignoriert
- sd-Karte Name Anzeige in System 2 korrektur "microSD" und detektion verbesserung in "Firmware Aktualizierung"
- Kundenkorrektur Min und Max Sollwerte wirden behalten bis ausschalten
- Update Marker fuer Wizzard und Standard Werte
- .bin-Datei wird geprueft fuer Grosse und richtige FW evrsion
- QR-code in Info seite
---
### **FW ver 0.8.2.4 / 24.11.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.4/C1202_FW_0.8.2.4.bin)**
- fix: Drehgeber Meister saklierung
- neu: Dregeber, anpassung der Meister für Bearbeitung mit Refernzpunkt
- neu: Dregeber, anpassung der Meister für Bearbeitung mit Refernzpunkt in multiturn modi
- upgrade: INkremental Modul Parameter Reinfolge änderung
- fix: Einrichten für Drehgeber
- fix: Sprache wechsel, Inkremental Modul aktualisierung
---
### **FW ver 0.8.2.3 / 19.11.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.3/C1202_FW_0.8.2.3.bin)**
- neu: Module FW erkennung nach Modul typ - wird nur FW gezeigt der passt zum Modul
- neu: neue Begriefe in Wuertebuch von Kartenspeicher behandlung fuer Datenausgang
- fix: Balkenanzeige und Zeigeranzeige "Anzeige zentrieren auf" fuer derhgeber verbessert - Warngrenzen
- fix: Balkenanzeige und Zeigeranzeige fuer "inch" umrechnung verbesserung inkl. Funktionen
- upgrade: Analoganzeige - Toleranz und Warngrenzen wenn nicht in bereich werden nicht gezeigt
- Skalenbeareibung:
  - fix: inch kleinesete Skale
  - upgrade: dynamische berechnung nach Zentrieren auf
  - upgrade: dynamische berechnung nach Nennmass
- graph upgrade:
  - fix: funktion Anzeige verbessrung
  - neu: dynamische Skalaanzeige (mit Zentrieren auf ind Nennmass)
  - upgrade: curvenanzeige anpassung fuer Zentrieren auf und Nennmass
- neu: Japanisch detektion nach Artikelnummer: ***5312024***
- neu: Japanisch Wuerterbuch Installiert nach Uebersetzung mit entsprechendem Font-upgrade (4Bk uebersetzung + 12kB Font)
---
### **FW ver 0.8.2.2 / 12.11.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.2/C1202_FW_0.8.2.2.bin)**
- upgrade: Graph visualisierug verbesserung: Digitalanzeige in vordegrung und positionierung
- fix: Anzeigeart fuer Zeiger nicht geaendert wenn "Verschiedene" editiert sind
- fix: Graph interne skalierung verbesserung fuer kleine Werte
- fix: Graph Punkte Diskoninuitaet verbesserung
- fix: Graph Skala fuer **Rad** und **um** verbessert
- upgrade: Analoganzeige (Balken un Zeiger) interne skalierung verbesserung fuer kleine Werte
- neu: Graph Netzpunkte fuer visualisierung und Ticks fuer Skala
- fix: Nennmass drehgeber
- fix: Zentrieren auf Nennmass fuer Drehgeber
- Zeiger Zentrieren auf Tolernaz dynamisch skala-Bezeichnung (min, max und mitte)
- fix: Formel Bilnkende Pfeil
- neu: Japanisch (ohne uebersetzung) eingefuehrt
---
### **FW ver 0.8.2.1f / 04.11.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.1f/C1202_FW_0.8.2.1f.bin)**
- Graph Inkremnetal Modul, Drehgeber. Grafikanzeige x10 behoben
- Graph ikonen positionierung verbesserung:
---
### **FW ver 0.8.2.1e / 04.11.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.1e/C1202_FW_0.8.2.1e.bin)**
- speicher optimalisierung, alle 11 sprachen
- Balken Zeiger Skala bearbeitung:
  - fix: negative Grad werto ohne zusatzlichen Zeichen (wie F)
  - neue skalierung: mm: 0.0001, um: 1, inch: 0.00003
  - neue skalierung moeglich nur in HR modul und Inkrmental Modul nach einstellungen
  - einstellung fuer laenge: 30mm limitiert nur fuer Inkremental Modul
  - einstellung fuer Winkel 360 grad limitiert nur fuer Inkremental Modul und Drehgeber
  - Neue skalierung in Einrichten: minimale skala immer fuer HR-modul und Inkremental Modul
  - Maksimale skalierung in einrichtung limitiert fuer Inkremental Modul
---
### **FW ver 0.8.2.1d / 29.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.1d/C1202_FW_0.8.2.1d.bin)**
- scale 0.0001 added
---
### **FW ver 0.8.2.1 / 29.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.1/C1202_FW_0.8.2.1.bin)**
- SD-card komunikations verbesserung
  - vermeidung synchronisation fuer manche Karten
  - Verschidene tests und optimieruung (11 karten getestet, FAT16 und FAT32)
  - karte endekung verbesserung
  bemerkung: FW-update mit gesendete Karte (synchronisierungs problem) nur ueber Menu moeglich. BL ist nicht geendert.
- Fix: Falshe Markierung bei FW-update nach Werkseinstellung
- fix: Datenausgabe zum SD Karte - Dritte Merkmal verschiebung
- Scale fuer laenge: "mm" ind "um" erweitert.
---
### **FW ver 0.8.2.0 / 21.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.2.0/C1202_FW_0.8.2.0.bin)**
- inklusiv FW versionen: 0.8.1.9d, 0.8.1.9r, 0.8.1.9s
- fix: Datenausgand mikro-SD karte - csv-Datei fuer Manuel und Senquentionel
- fix: Messmodul FW update,
- laenger Dateinahmen sichtbar
- FW update, backup ohne "_bak" Suffix
- Rohwerte in Einrichten
---
### **FW ver 0.8.1.8 / 15.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.8/C1202_FW_0.8.1.8.bin)**
- drehgeber und "Ref. Punkte >1" aktiv ist
  - "Anzahl Ref. pro U." - nur wert "1" moeglich
  - "Anzahl Ref. pro U." - nicht editierbar
  - "Anzahl Ref. pro U." - bei erste start geprueft und auf 1 gesetzt.
- "Graph" Nennmass wird auf null beziehen
- fix: "Graph" skalierung bei mehrerem Merkmaele
---
### **FW ver 0.8.1.8d / 13.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.8d/C1202_FW_0.8.1.8d.bin)**
- CSV-Detei mormatierung:
  - spalte einheit eingefügt
  - "°", "µ" und "12°54'32" formatierung
  - "." auf "," wechsel fuer bes
  - Toleranz und Warngrenzen sind abgelehnt
- fix: alle csv-Datei sind gezeigt
- fix: C1202 FW update:
- C1202 FW update proyedure geändert
- fix: Module FW update
- fix: Kundenkorrektur plausibilität prüf änderung (if ( abs(calibMaxAct[actParaT] - calibMinAct[actParaT]) < abs(calibMax - calibMin) / **100** ))
- fix: Englische Sprache: "Repeat Customer Calibration" & "Values are not valid"
---
### **FW ver 0.8.1.7 / 07.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.7/C1202_FW_0.8.1.7.bin)**
- SD-karte pruefung nur bei start und datenausgang
- grafik-anzeige verbessert
- datei bearbeitung - seiten
- dateibearbeitung (parameter, FW update modul, FW update C1202, Karten-datenspeicher) undefinierte anzahl der neuer Datei
- masimal Dateinamelaenge 26-Zeichen
- Modulen FW - update - aktuele parmater sind gespeichert
- Linear-taster, umrechnung fuer mehrere referenzpunkte
---
### **FW ver 0.8.1.6 / 01.10.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.6/C1202_FW_0.8.1.6.bin)**
- Digimatic schnitstelle:
  - fix: negative werte
  - Winkeleinheiten: fuer alle nur Grad
  - 9-Ziffer fall, erste Ziffer wird nicht augedruckt
- Datenausgang:
  - neues struktur (liste statt multichoice)
    - USB, Digimatic, micro-SD
  - Neue ikonen in Messenzeige (unter Taste 5)
- Datenausgang micro-SD
  - datenauswahl mit name editor
  - datenformat ist .csv
  - datenstruktur mit spatlen spaltennamen nach ausgewaehle Sprache
  - SD-karte und Datei pruefung
  - aktive dateinahme wird gespaeichert. bei neustart wird automatisch aktiv
  - aktive dateiwalidierung (gesichert mit check-summe)
  - datei loeschen
- Datei editierung, verbessung
  - dynamische nahmelaenge
  - 3 spalten fuer alle faelle (Fw update, parameterverwalte, modul programiern und Dateispeicher)
  - dateinahme-justierung
  - laengere namen fuer parameter, bis 12-zeichen plus Zaehler
  - dateinahmen ohne extention (.par, .csv. .bin)
  - dateinahmen abkurzung
- Modul flashen verbesserung
- Test FW fuer modul: Dreiekgenerator und Segezahn
  - neues MarCom befehll fuer MarNet: "AT?MNT="
  - Grafik Anzeige in Menu -> Merkmal -> Anzeigeart -> Graph
  - Jederpunkt in Grafik ist ein messung, Pufferlaenge 400 messungen = 4sekunden
- fix, nach George Schutz, nahme fuer ein pneumatisches modul
- andere kleine verbesserungen und optimierung
  ---
### **FW ver 0.8.1.5 / 10.09.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.5/C1202_FW_0.8.1.5.bin)**
- Data anforderung verbesserung / stabilitaet:
  - empfangene Datei plausibilitaet pruefung (datei format, CRC-pruefung)
  - interrupts ausgeschaltet fuer Merkmale umrechnung
- Inkrmental modul parameter ueberwachung fuer "Reference point-proc" und "Ref.punkte >1"
- Meister reset in einrichten und bei Inkrmental Sensor parameter aenderung
- Meister fuer Drehgeber
  - bei ref-punkt bearbeitung, nur positive Werte
  - fuer Drehgeber in Multiturn modi verbessert
  - fuer 2 kanaelen Drehgeber implementiert aber nicht getestet
- Digimatic 2.0:
  - Einstellung in Menu unter: System 2 -> Data Ausgang
  - Messanzeige Ikone fuer Daten Senden aktiv wenn Digimati ausgewaehlt mit kleine "D" bezeichnung
  - Manule, Sequenziell und Parallel modis implementiert (in parallel modi druker ist zeitlimitiert aber in mitutoyo druker Datei sind im Puffer gespaeichert)
  - Logik MarCom - Digiomatic impelmentiert (ausname: wenn digimatic ausgewaehlt ist, MarCom befehle sind noch aktiv)
  - Digimatic ausdruck moegllich wenn: Taste 5 gadrueckt, drucker oder kabel Taste gedrueckt
- Messdaten in SD-karte speicher:
  - Aktivierung in System 2 -> Data Ausgang parallel zum Marcom oder Digimatic
  - Wenn MarCom kabell nicht angeschlossen ist, datenausgang zum SD-karte noch moeglich
  - dateiformat: artikelnummer_zaehler.csv (excel oder txt editierbar)
  - datei sind in spalten gespeichert
  - neudatei ist bei neu einschalten hoch gezaehlt
- allgemeine optimierung
---
### **FW ver 0.8.1.4A / 03.09.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.4A/C1202_FW_0.8.1.1A.bin)**
- minor stability at 100Hz update
---
### **FW ver 0.8.1.4 / 03.09.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.4/C1202_FW_0.8.1.4.bin)**
- Inkremental modul Drehgeber, maximle Werte erhoehung in kleinere aufloesung bis +-19999.999 (ca. +-55 Umdreungen).
  - wert ist limitiert nach 32-bit wert (-2,147,483,648 <-> +2,147,483,647) nominiert in 10^5 grad (in versionen bis 0.8.1.3 10^6). Das gild nur fuer Inkremental drehgeber.
  - Meister, nennmass, Toleranz und Warngrenzen, analog anzeige un digital angepasst
  - Font-grosse un positionierung angepasst
  - Einrichten angepasst fuer maximale aufloesung und wert
  - max 32bit wert ueberfluss limitierung eingefuegt
  - Radiant Anzeige angepasst (max wert in radiant ist: 349.99999 - ca. 19999.999 grad)
  - winkelsekunde Anzeige angepasst
- Toleranz und Warngrenzen, Nennmass und Meister maximale Eingabe erhoehrt von 399.99995 Grad fuer 999.99995
- Inkremental sensor mit Drehgeber:
  - ohne referenzierung, Meister funktionieret genauso wie bei laenge
  - mit referenzierung, Meister bei jede Umdrehung wird zurueckgestzt
  - mit referenzierung und multiturn (anzahl referenzpunkte > 1 = 1): wird meister aktiv verschoben nach umdreung. In dise version funktioniert nur fuer positive werte.
---
### **FW ver 0.8.1.3 / 27.08.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.3/C1202_FW_0.8.1.3.bin)**
- fix: Inkremental sensor Parameter-> "Ref. punkte > 1" mit 3 Merkmale Gefrohene Werte problem behoben.
  - Werte plausibilitaet verbessert fuer 100Hz. Werte anforderung -> wenn neue werte sind erhalten, bearbeitung. unaphaengig von Anzeige
- fix: "Distanz zwisch. Ref." Max Wert anzeige korrektur
- Inkremental modul Parameter aktive Taste fuer "check box"
- Werte plausibilitaet fuer anzeige verbessert. In Anzeigebild werte fuer alle Merkmale sind von einem Zeitpunkt
- Digimatic 2.0 implementiert:
  - einheiten "mm" und "inch" sind uebertragen je nach dem welche Einheit aktiv ist. Wenn "um" aktiv ist, wert ist als "mm" gesendet.
  - nur eine Wert nach anforderung oder datentaste gesendet wird.
  - in einem fall wenn zeichen sind mehr als 8 letzte ziffer ist entfernt
  - fuer negative werte drucker zeigt 7 stellen statt 8
  - bei einheit aenderung oder prezision aenderung, drucker zeigt "POIN ERROR" oder "UNIT ERROR". nach quittung neue Werte werden ausgedruckt
---
### **FW ver 0.8.1.2 / 20.08.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.2/C1202_FW_0.8.1.2.bin)**
- phasenkorrektur speicher verbessert, nach dem korrekturablauf wird automatisch in modul gespeichert. Fuer das richtig zu funktionieren ein neues fw ist notwendig fuer inkremntalmodul, Version 1.15a 
- Inkremental modul Paramater speicher verbessert
- Messmodulfehler in Einrichten Reset-Taste Rot markiert
- "atan" funktion einstellung, prameter umstellung auf Winkel in Induktive Modulen behoben 
- 100Hz abtstrate implementiert fuer alle funktionen
- Sprache umstellung fuer alle paremeter  
- Laengere Dateinamen fuer Modul programieren
- speicher optimierung
---
### **FW ver 0.8.1.1 / 13.08.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.1/C1202_FW_0.8.1.1.bin)**
- Name "preparing for backup" auf "Creating Backup" geendert
- Wueterbuch aktualisiert fuer FW update und inkremental modul, neue Begrife:
- "Backup vorbereitung..." in FW update 
- "Neu Wert ist:" in phase correction ablauf
- "Update mit:" in FW update
- "Drucken und Halten beide Taste" nin FW update
- "Neu Dateiname:" in Parameterverwalten
- Speicher in Inkrementalmodul Parameter verbessert
- FW update Tasterhintengrund fuer neustart auf rot geendert
- FW update, "Backup vorbereitung..." Fortschrittsanzeige
- optimalisierung
---
### **FW ver 0.8.1.0 / 16.07.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.1.0/C1202_FW_0.8.1.0.bin)**
- Firmware Update Dateiname verlaengfert, Standart name: "C1200_FW_x.x.x.x.bin"
- Fix: Inkremental Sensor Parameter: Speicher Ikone war nicht imme gueltig - korrigiert
- Fix: Inkremental Sensor Phasenkorrektur durchlauf korrigiert - neu Wert Speicher, specher ermoeglich und Sensortyp nach phasenkorrektur wechsel
- Inkremental Sensor - Werte editierung Farbe Gelb nach ungueltige Werte
- Inkremental Sensor Parameter - von name geendert: "count ref points" fuer "Ref. Points  > 1"
- Menue - name geendert: von "Tastatur / Menu sperre" fuer "Menue sperre"
- Firmware Update ohne Datei loeschen - Dateiname nach aktualisierung bleibt ungeaendert
- Firmware update: bevore Aktualisierung, wird Aktuele FW backup gemacht und auf SD-karte gespeichert under name: "C1202_FW_x.x.x.x_bak.bin"
---
### **FW ver 0.8.0.9 / 16.07.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.9/C1202.bin)**
- Einrichten neue Name: "SENSOR" statt "ABSOLUTE"
- Inkremental modul - Parameter: Analoge werte mit Max Anzeige ("gitterkonstante", "ink. pro. Umdreh", "Anzahl Ref. pro U.", "Dist. zwisch. ref.")
- Referenzierung behoben (Messanzeige und Einrichten)
- Fehler Anzeige sebst-reset ohne neistart (neue logik) und Fehler reset in Einrichten unter Tatse 5
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
---
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
---
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
---
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
---
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
---
### **FW ver 0.8.0.4 / 02.06.2021: [download C1202.bin](https://github.com/k-szczeciak/C1202RelOpen/raw/master/0.8.0.4/C1202.bin)**
- inkrmental: linear werte lesen und zeigen
- einfache diagnostic ueber MarCom (7 zaehler)
- Keine Antwort von Modul Fehler Nachricht Anzeige 
- Forel, T&W und 2P-Meister: Paremeter geendert in Titel Anzeige, von "*" fuer Farbe Grau
- Forel, T&W und 2P-Meister: Parameter editierung: pfeil bleibt permanent
- Inkremental modul Parameter: springen ueber ausgegeute Werte
- Inkremental modul Parameter: Referenz punkte logik: erst muss Referenz Punkte bearbeitung aktiviert sein
- INkremental Anzeige: blinkende Kreiss wenn Taster nicht referneziert ist
---
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
---
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