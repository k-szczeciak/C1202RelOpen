# Millimar Software C1202
FW ver 0.7.8.7 / 13.04.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.7/C1202.bin) )
- Erste start verbessert und optimiert: Zeitenm, artikelnummer und seriennummer richtig eingestellt
- eerpom erase moeglich um Erst Start zu simulieren

FW ver 0.7.8.6A / 13.04.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.6A/C1202.bin) )
- Neu Font fuer 32-pixel gross Fett (Font32B). bentzt in Formel -> Funktion. Chinesischbuchstaben und Sonderzeichen fuer ander sprachen in menu verfueggbar ("keine" und "Mittelwert") 
- **Sprachen** Tschechisch und Franzoesisch korrigiert
- **bug fix** ID 45804 (Menu sperre) korrigiert
- **SD** parameter uebertragung ueber marcom schnittstelle
- bugfix - 2Pmeister, first start of Nominal - plausibility check run unnecessary and cause problems

FW ver 0.7.8.6 / 09.04.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.6/C1202.bin) )
- **SD Karte** dynamische detektion in menu
- **SD Karte** Name bearbeitung - abkuerzung fuer 6-Buchstaben
- **Modul programieren** vebesseung:
  - Antwortzeit verbessert
  - Menu Texte und Titel angepasst fuer verschiedene Sprachen
  - Chinesiche Sprache programierung moeglich
- **Parameter verwalten** vebesserung:
    - Antwortzeit verbessert
    - Menu Texte und Titel angepasst fuer verschiedene Sprachen
    - datei namen liste verbessert, max laenge fuer Dateiname ist 14 total (10-vorkomma Zeichen plus Extension)
    - maximale datei liste laenge bis 24 erweitert, 6x4
    - **Dateiname editierung** bei speicher moeglich: 6 stellen + 2-stelige automatische Zahl, z.B parame01.par.
      moegliche Zeichen: [a-z][0-9][-][_]
    - Speicherikone anpassung wenn keine karte oder kein freies Paltz mehr ist
    - Firmware Version in parmaterer datei im erste stelle zugefuegt
    - algemeine verbesserungen
- **MarCom** - Seriennummer einstellung - minmal wert pruefung
- **Sprachen update**: SE, RU, CN, IT, PT, SW, EN, DE (8), bleibt noch Tschechisc, Franzoesisch und Spanisch
- Sprchewechsel verbesserung fuer **Formel**
- **Listenanzeige** verbesserung
- **Winkelaufloesung verbessuerng** - chinesische Namen - Radian war nicht richtig gezeigt in Kanji
- **Kein messmodul** - verstekte Funktion - Taste 1 Langdruck - moeglich ins menu zu gehen um z.B. falshgeflaeschte modul neu zu Falshen.
- Schnittstelle fuer **automatische tests** (Reset, Tasten, screenschot, Home, FS, Parameter Laden)

FW ver 0.7.8.5 / 30.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.5/C1202.bin) )
- Fix Fussschaluter parallel daten senden, auch Tasten
- Farbe fuer Teksttaste nach Modul Update und Kuundenkalibrierung
- Modul Update moeglich nach bestaetigung - neu Bestaetuigungsfenster
- Parameterverwalten: Parameter laden und loeschen nach bestaetigung - neu Bestaetigungsfenster
- Sprache verbesserungen in Woerterbuch und laengeanpassung, besonderes in Kundenkorrektur (kurz fuer Kunden- und Firmenkorrektur aktivirung).
- neue Woerte fuer Bestaetigubngsfenstern

FW ver 0.7.8.4D / 24.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.4D/C1202.bin) )
- Fix, Seriennummer editierung fuer MarCom (auch Produktionwerkzeug)
- Sprache Polsnisch korrigiert (nach empfehlung Mahr Polska)
- Fix, Parameteranzeige wenn Einheit und Anzahl Meister gaeendert un nachdem Funktion "atan" nach nicht-"atan" korrigiert
- Lange Liste Scroll verbessert z.B Sprache.


FW ver 0.7.8.4C / 24.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.4C/C1202.bin) )
- Sprachen wechsel verbessert (geschwidigkeit und zuferlaessigkeit)
- Marcom inch antwort runden korrigiert fuer HR modul
- Aktuelle Merkmal anzeige "hand" gaendert
- 2P-meister plausibilitaet pruefung verbeserung (extreme werte und nicht gleich) 
- Warngrenzen pruefung und aenderung ween toleranz kleiner ist und sehr enk.
- Formel aussicht verbessert (zusatzliche leertaste)
- 2P-Meister plausibilitaet pruefung - in Entry 
- extreme parameter werten pruefung aenderung ">="
- Deutschen texten korrigiert

FW ver 0.7.8.4B / 23.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.4B/C1202.bin) )
- fehlende "[" "]" "%" Zeichen und andere zugefuegt
- pinAcces Tasten ordnung geaendetr
- angepasst laenege fuer alle Sprachen und alle Worte/Saetze
- string laenge ueberwahung in code ueberall fuer sichere sprachen bearbeitung

FW ver 0.7.8.4A / 19.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.4A/C1202.bin) )
- korrigiert fehlende Fontszeichen
- aufloesung Winkel 
- Check box in Multichoice (Anzahl Merkmal, Fussschalter, Verschiedene und Servis)

FW ver 0.7.8.4 / 19.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.4/C1202.bin) )
- alle 11 Sprachen implemetiert
- angepasst Font-satzt
- Worte/Satzte korrekturen

FW ver 0.7.8.3B / 19.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.3B/C1202.bin) )
- Stabile 9 **Sprachen** ("Deutsch", "中文", "Čeština", "English", "Français", "Italiano", "Polski", "Português", "Русский")
- **Font**-satz aktualisiert und angepasst zum benutzte Werte.

FW ver 0.7.8.3A / 18.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.3A/C1202.bin) )
- 9 sprachen
- kleien verbesserungen fuer sprachen mit langere Saetze/Worte
- ersten start aenderung

FW ver 0.7.8.3 / 18.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.3/C1202.bin) )
- Navigierung im Merkmal fixed
- **Formel**: Funktion "Normal" als "x" und "keine" im Formel gezeigt
- **Korrektur** kurze Namen verbessert fuer Multilanguage
- **Sprachen** Namen abkurzung
- **erste Start** Verbessert
- (limitiert 6 sprachen)

FW ver 0.7.8.2E / 17.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.2E/C1202.bin) )
- **MarCom** fix: Warngrenze Werte pruefung wenn in C1202 ist in Laenge
- **Merkmal Auswahl** menu anzeige Korrektur - fehler von 16.03.2021 QS
- neue Sprachen" **Chinesisch** (einpaar Zeicheen fonts Felhen), **Spanisch**
- Fix: **Bug-Id: 45696** mit Winkel editierung
- Fix: **Bug-Id: 45697** Winkeleinheiten Multisprachig

FW ver 0.7.8.2D / 16.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.2D/C1202.bin) )
- **MarCom** rundungsverbesserung wenn modul wechsel HR-Normal
- **MarCom** neu kriterium fuer Werte stetzen: nachricht-laenge max 50 zeichen
- **MarCom** Rundung verbesserung fuer "deg"

FW ver 0.7.8.2C / 15.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.2C/C1202.bin) )
- **MarCom** HR-Modul Aufloesung fuer inch und mm dynamisch
- **MarCom** Min-Max pruefen verbesserung
- **MarCom** inch rundung letzte Ziffer (0/5) fuer HR und nicht-HR Modulen
- **MarCom** deg rundung letzte Ziffer (0/5)
- **MarCom** Aufloesung anpassund fuer Andere elemente
- **MarCom** neu Fehler "ERR7" wenn C1202 ist in menu Aktiv

FW ver 0.7.8.2B / 12.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.2B/C1202.bin) )
- fix: mutlichoice sturz (Merkmal Auswahl, Fussschalter, Verschiedene, Service)

FW ver 0.7.8.2 / 12.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.2/C1202.bin) )
- **Max-Min** korrigiert -> Frage: wie soll **Meister** in diesem funktion bechandelt sein?
- Sprachen: **English**, **Deutsch**, **Polnisch**, **Tchechisch**, **Franzoesisch**, **Russisch** (nicht stabil), **Schwedisch** implementiert aber noch nicht Editiert
  
FW ver 0.7.8.1E / 11.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.1E/C1202.bin) )
- MarCom fix:, **START** Echo

FW ver 0.7.8.1D / 11.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.1D/C1202.bin) )
- Marcom Neu fehler EER6 - wenn keine datei verfuegbar
- MarCom **START** **STOP** fuer ein Merkmal korrigiert, auch Reset fuer **START** zugefuegt
- MarCom **?** winkel mit toleranzgrenzen korrigiert

FW ver 0.7.8.1C / 11.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.1C/C1202.bin) )
- Menu-bau verbessert - schneller und sichere Menu upddate nach parameneter enderung, besonderes: Aufloesung, Einheit (L+W), Formel (atan), u.a.
- Werterbuch bearbeitung (doppelte werte, liste, getrennt sind werte ohne sprachen optionen wie eigene Namen) und implementierung in code 
- Fix - MarCom **START** **STOP** antwort korrigiert

FW ver 0.7.8.1B / 05.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.1B/C1202.bin) )
- grosse zahlen verbesserung Testbericht von 26.02.2021

FW ver 0.7.8.1 / 05.03.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.1/C1202.bin) )
- neu parameter fuer nicht offentliche optionen wie Optimar, FPS anzeigen und Marnet Pasiv: **Service** - PIN gesichert (1861) 
- fix: Namen in "Modul Programmieren" fuer HR-Modul
- Wuerterbuch und parameters aktualisiert (in bearbeitung)
- screenshots erweitet fuer dynamische elemente in menu (noch in bearbeitung)
- MarCom: neu Befehl **PRE, PRE1, PRE2, PRE3** Meistern
- prezision erhoert in "inch" Anzeige,
- Tastenbeschreibung in Kundenkorrektur, Werkseinstellung und Modul Programieren korrigiert (wenn prozess leuft, keine Taste ist aktiv - wird asugeblended).

FW ver 0.7.8.0 / 25.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.8.0/C1202.bin) )
- Erschrenkung der unterschtuzten Modulen nach Artickelnummern:
    ("5331120", "5331121", "1234567", "5331150", "5331151", "5331152", "5331155", "5331156", "5331157", "5331125" )
    Wenn modul nicht unterstuezt ist, Fenster mit Fehler wird gezeigt
- Neue aufloesungen implementiert: "0,00001 mm", "0,01 um" und "0,0000005 inch". Auswahl moeglich nur wenn HR-Modul angeschlossen ist.
  - wenn auf nicht HR-Modul gewchselt ist, hoechste mogiche aufloesung eingestellt ist
- "um" und "inch" parameter fuer hoehre Aufloesung editierung angepast
- Fix: einstellung fuer "inch" limitierung der erste ziffer (0-3 moeglich)
- Messanzeige erweitert auf HR hoehere Aufloesung
- Nullen speicher verbessert, 1P-nullen wird immer gespeichert, 2P-nullen wird nicht gespeichert wenn messwerte sind gleich, delta = 0 (bei delta=0 , umrechnung kann nicht durchgefuert werden).
- Messanzeige verbesset und angepasst allgemein das ist plausibel mit hoehere HR Aufloesung
- nullen in automatik Betriebsart verbessert, immer Nullen als Standart
- nullen in manuel Betriebsart verbessert. z.B. parallel Nullen: nur wenn alle Merkmalle genullt sind - umschalten auf Extremwerte-reset moeglich
- Winkelmessung genauigkeit verbessert
- screenshot in Einrichten, "spash screen", werkseinstellung (bei starten T2 und T3 - aktiv ist T3 wenn seite wird Gezeigt), "Wizzard" (T5 LP) - erst muss option aktiv in Verschiedenes Sein, nachdem Wizzard abgeschlossen ist. Nur einmal.
- Einrichten, aufloesung angepasst zum HR-modul wenn angeschlossen.


FW ver 0.7.7.9E / 23.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.9E/C1202.bin) )
- Fix: MarCom: fehlende ";" fuer mehrere Nachrichern zugefuedt 

FW ver 0.7.7.9D / 22.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.9D/C1202.bin) )
- Fix: winkelsekunde aufloesung
- Fix: einheit aenderung verbessert (selecktiv update)
- Fix: aufloesung aenderung verbesserung (selecktiv update)
- Fix: **Einrichten** schrinken und vergroessen Tastebeschreibung verbessert
- Fix: MarCom **NOMINAL?** alle werte (inkl. winkel) geshcickt.
- Fix: MarCom **";"** ueberall am Nachrichtende entfernt.
- Aenderung:: MarCom aufloesung fuer winkel **"deg"** angepasst fuer 5-nachkomma stellen
- Ausschalten moeglichkeit waerhend Wizzart einstellung (ersten Start).
- Fix MarCom: Fehler mit fehlendem ";" "MASTER?", "NOMINAL?", "TOL?" und "TOLW?"

FW ver 0.7.7.9C / 18.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.9C/C1202.bin) )
- MarCom **MASTER1,2,3** fuer 1P und 2P Meister implementiert
- MarCom **MASTER?** fuer 2P meister implementiert. 1P-Meister 3xWerte sind scheschickt wenn 1P-Meister aktiv ist, 2P-Meister 3x2=6 Werte wenn 2P meister aktiv ist
- MarCom **MASTER1,2,3; NOMINAL1,2,3; TOL1,2,3; TOLW1,2,3** mit _inch_ setzen moeglich
- MarCom **MASTER, NOMINAL, TOL, TOLW** setzen und rufen wenn Merkmal nicht Aktiv ist Fehler **ERR3** ist geschickt
- Fix: 2P-Meister display
- Fix: **hand** anzeige in automatische messung waerend messung und daten senden ist nicht parallel.
- Fix: **Data senden Ikone** gezeigt wenn MarCom **Mx?** ist angefoerdet
- MarCom **MASTER?, NOMINAL?, TOL?, TOLW?** alle werte sind uebertragen, laenge (_mm_ oder _inch_) und winkel (_deg_) fuer alle Merkmale.
- MarCom: **Artikelnummer** 9-stellig

FW ver 0.7.7.9B / 16.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.9B/C1202.bin) )
- **Screen Saver** wird deaktiviert wenn messung leuft
- **Screen saver** in menu korrigiert. wenn in menu - deaktivierung bei wer-aenderung nicht moeglich
- screen saver deaktivieung durch wert-aenderung in winkelmessung weniger sensibel (10x)
- **Fix**: Automatisches Betriebsart **Winkelmessung**: Werte in stopp sind gefrohen (wie im laenge messung)
- **"Hand"** Anzeige - Farbe gaeendert von schwarz auf dynamische Farben Hintergrund gesteuert: Weiss Hintergrund -> blau, Gruen -> blau, Gelb -> blau, Rot -> gelb) (P5. von 12.02.2021 (p4. von 12.02.2021))
- **"Hand"** Anzeige, kleine bewegung zeitgesteuert und bei Merkmall aenedung mit Taste 4. Nicht aktiv venn messung leuft
- **Menu Geaendert**: Nennmass mit Tolrenz umgetauscht (p4. von 12.02.2021)
- **Nullen/Reset** Taster in Automatik Modi geaendert. Umschaltung nur manuel moeglich. (p3. von 12.02.2021)
- **Nullen/Reset** Taster Manuel Betrieb Verbessert, automatische wechsel, start modi erkennung, u.a.
- **Mittelwert** in Automatik und Manuel Betriebsart Reset verbessert. (p2. von 12.02.2021)
- Bei neustart, **werte umrechnung** (beziehungsweise wichtig bei funktionen) erst wenn erste werte von Messmodul kommen. Anflus: Mittelwert, Min und Max
- **Winkel** messung bei _inch_, fuer rechnen sind gerundete Werte benutzt
- screen saver korrigiert
- **MarCom, "?"** daten senden fuer **"Grad"** korrigiert
- kleine verbesserungen

---
FW ver 0.7.7.9 / 11.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.9/C1202.bin) )
- MarCom:
  - Automatic betriebsart: **START, STOP, PAUSE**
  - Extremwerte Reset: **RST, RST1, RST2, RST3** - EER3 wenn Merkmal ist kein extremwert
  - Meister setzen: **MASTER1 , MASTER2, MASTER3**: einheit "mm" fuer laenge und "deg" fuer winkel. Formatierung ueberwachung: leerzeichen, punkt,.u.a. (kein 2P-meister)
  - Meister lesen: **MASTER?** - alle 6 (3 laenge und 3 winkel) unapheangig wieviel Merkmaellen sind aktiv, gild auch fuer setzen
  - Nennmass setzen: **NOMINAL1, NOMINAL2, NOMINAL3** - eanlig wie bei Meister setzen
  - Nennmass lesen: **NOMINAL?** - aenlig wie bei Meister
  - Toleranz setzen: **TOL1, TOL2, TOL3**: formatierung und uberwachung wie bei Meister, werte plausiblitaet ueberwachung, Wenn absolute Werte sind kleiner als Warmngrenzen, Warngrenzen sind automatisch koribgiert (wie diriekt bei Menu aenderung)
  - Toleranz lesen: **TOL?** - alle 6 doppel werte sind geschickt
  - Warngrenzen setzen: **TOLW1, TOLW2, TOLW3**: formatierung und uberwachung wie bei Meister, werte plausiblitaet ueberwachung. Wenn werte sind nicht mit Toleranz plausibel, EER3 fehler ist geschickt
  - Artikelnummer setzen: **T**: neu Artikelnummer ist jetzt in eeprom gespeichert. setzen moeglich nur mit "master password"
  - Serielnummer setzen: **S**: mit "master password"
  - **T** und **S** sind nicht geloscht waerend werkseinstellung durchfuerung
  - Menu Lock password: **LCK** mit aktuelles PIN und master password moeglich
  - Menu Lock aktivierung: **LCK1** ohne PIN moeglich
  - Menu Lock deaktivierung **LCK0** nur mit PIN moeglich
- Fehler behoben: Paraller Meister setzen nach ersten mal, moeglich (P1 von 05.02.2021)
- Standart werte fuer **_Anzahl meister_** und **_Verknoepfung_** neu gestzt: 1xMerkmall und alle Merkmalle standard "+C1" gestzt
- Werkseinstellung verbesserung (master, skala loeschen)
---
FW ver 0.7.7.8B / 05.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.8B/C1202.bin) )
- Anzeige mit mittlere Fontgroesse Angepast und verbesert
---
FW ver 0.7.7.8 / 04.02.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.8/C1202.bin) )
- Automatik-modi Zeiten einstellung wenn nur ein pneumatik Module eingeschlossen ist
- Menusperre mit PIN korrigiert (PIN-eintrag, Zeiten, Zeite-reset)
  Frage: soll PIN in menu Zeite laufen?
- nicht korrekt eingezeigte Ziffer waerend editirung (p.3 von 29.02.2021)
- "(M+M)" auf "(M+M)/2" umgesetzt (p.1 von 29.02.2021)
- MarCom Anfrage "?" u "M1?", "M2?", "M3?" verbessert, neue Vormatierunng: 00:00:00 dms
- Neue ikone in Automatik modi: "hand" nicht aktiv (p.14 von 22.01.2021)
- screen saver Verbessert (aublauf-zeit in Menu, deaktivierung nach funktion nicht Raw-werte)
  Frage: wenn Menusperre mint PIN und screen saver aktiv sind, soll nach screen saver Zeit Menu gespeert sein?
- MarCom - daten senden wenn in Menu - EER3 (von PC oder FS)
- Standart Werte geaendert:
    1. Mermal Auswahl: M1, M2
    2. Merkmal M1, Formel Verknoepfung: +C1 
    3. Merkmal M2, Formel Verknoepfung: +C2
    4. Merkmal M2, Formel Verknoepfung: +C1+C2
    5. Screen Saver: 5 min
    6. Aufloesung winkel M1, M2, M3: 1 (mitteleinstellung)
    7. Winkelmessung, Toleranz M1, M2, M3 Min: -1 Grad
    8. Winkelmessung, Toleranz M1, M2, M3 Max: 1 Grad
    9. Winkelmessung, Warngrenzen M1, M2, M3 Min: -1 Grad
    10. Winkelmessung, Warngrenzen M1, M2, M3 Max: 1 Grad
- Falsche "hand" Anzeige und bedienung wenn nur eine Analoganzeige und kein kabel ist - Fehler bei Her Tluczek gefunden
- Toleranzgrenzen und Warngrenzen Plusibiliaet ueberwachung (p.2, von 22.01.2021)
- fehler behoben (p.2 von 29.01.2021) - falshce Anzeige wenn messung ist nicht gestartet in "normal"
- Mittlere Fontgroesse implementier (p.9 von 22.01.2021)
---
FW ver 0.7.7.7 / 29.01.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.7/C1202.bin))
- Automatik messung, funktion" "Normal", in Stopp/Pause Zahl und Zeiger/Balken sind eingrfroren (P1, 22.01.2021)
- Automatik messung, Toleranz & Warngrenzen, funktion "Normal" auswertund in Stopp/Pause sin eingefroren (P2, 22.01.2021)
- Einrichten: Roten punkt, "Auto" und funktion anzeige entfernt (P5, 22.01.2021)
- Zeiger Anzeige verbesserung, wenn Toleranz nicht aktiv ist.
- Hauptanzeige korrigiert (Formel symbol und Auto Symbol)
- Falsche Anzeigeart nach parameter umschaltung (P6, 22.01.2021)
- 2P- Meister anzeige korrigiert und 1P meister verbessert (P7, 22.01.2021)
- 1P u. 2P Meister zustand Anzeige mit Ikone
- Menusperre mit PIN realisiert mit master PIN: "1861" (P8. 22.01.2021)
- Menusperre nach Parameter speicher wird sofort uebernohmen.
- Ensperrung nur fuer 1 minute nach der Zeit wenn keine Taste nicht betaetigt ist
- Screen Saver verbessert: deaktivierung nach: taste drueck, MarCom Datenanforderung, FS-druck, MarCom-kabel Tasterdrueck (P10, 22.01.2021)
- Screen saver deaktivierung nach Tasterwertaenderung, min. auf 2 im letzte eingestellte stelle (P10. 22.01.2021)
- "Regen" bildschirmschoinner verbessert mit gleiche eingeschaften wie in P10. von 22.01.2021 (oben geschhrieben) (P13. 22.01.2021)
- Setup 1 - Nullen Loeschen in Menu Implementiert (P15. 22.01.2021)
- in FS-einstellung - nicht aktive Zeilen sind nicht mit Kursor auswahl-moeglich. Tasten beschreibung Dynamisch aktualisiert (P12. 22.01.2021)
- Paralell nullen (u. nullen algemein) verbessert (P1, P2, P3, von 22.01.2021, Teil 3)
- Nullen loeschen nach Formel ediierung nur fuer eine Merkmalle
- Daten senden fuer markom Verbessert
---
FW ver 0.7.7.6 / 22.01.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.6/C1202.bin))
- Verschiedenes: Optimar Aktivieren wird nicht gespeichert, passiv mit reset und nicht speichern
- Betriebsart Automatik: Funktion "Normal" digialer Wert bei Pasue und Stopp eingefroreren (P1)
- Betriebsart Automatik, Funktion: Toleranz auswertung nach Pasue und Sttopp eingefroren (P2)
- Betriebsart Automatik: Messwert immer in schwarz, nur Farbe der punk aendert sich fuer Messzeit (P3)
- Betriebsart Automatik, Pausendauer = 0 und Messdauer = 0: Automatische Daten senden nur wenn "Daten Senden" is "Parallel" eingestellt (P4)
- Betriebsart Automatik, Fussschalter: "Daten Senden" + "Start" + "Messdauer" not eq 0, daten senden automatisch nach Messung. Waerend der Messung Daten senden immer aktiv. (P5)
- "Hand" Symbol bleibt aktiv waerend messung auch wenn messung leuft wenn noetig (P6)
- Bildschirmschoner auswahl 30min moeglich (P7)
- Wenn Toleranz aktiviert ist, Warngrenzen werden zuruckgeholtvon alte einstellung (P8)
- Wenn Tolernaz wird deaktiviert, Warngrenzen sind ausgegraut. (P9)
- MarCom, Befehl "?": verbessert formatierung nach letzte Interface Beschreibung stand von 21.01. Werte uebeschritt mit ERR3 implementiert
- MarCom, Befehle "M1", "M2" und "M3" implemetiert
- MarCom, Befehl "ID?" implementiert
- MarCom, Befehl "DES?" implementiert: <Brand> bleibt als Konstant in FW
- MarCom, Befehl "VER?" implementiert
- MarCom, Befehl "OFF" implementiert

q:
1. Toleranz und Warngrenzen - Sollen Warngrenzen < als Toleranz sein?
2. Automatik modi zyklische messung. anzahl der zyklen soll limiriert sein / oder einstell bar sein: 10/100/unbegrenzt
3. wenn Menu ist blockiert, soll MarCom volstaendig funktioniert?
4. HR-modul - welche tastertypen?
5. wie soll daten senden in automatik betrieb funktionieren Taste 5?
6. wenn meister messung und daten senden parallel und nur digitale werte - soll ikone sich aendern unter Taste 4
7. wann soll nullen geloesch werden - jetzt ist nach formel editierung und anzahl meister aenderung 
---
FW ver 0.7.7.5 / 14.01.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.5/C1202.bin))
- displayanzeige Merkmall synchronisiert: alle Merkmalle 1 - 3 sind berechnet mit gleiche messwerte in einem bild. 
- nullen parallel fuer alle Merkmalle auch mit Gleichen Werten
- winkel umrechnung geprueft und verbessert (runden fuer 0,00005 grad), liste in Anhang
- Warngrenzen Aktivierungs moglich nur wenn Toleranzgrenzen akiv sind.
- Wenn Tolernz deaktiviert ist, Warngrenzen werden auch automatisch deaktiviert
- Standard werte fuer Tolernaz und Warngrenzen geendert
- Standart Werte fuer 2P-Meister geaendert
- fix: parallel nullen ikonen anziege
- Optimar interface implementiert:
  - nur in "ABSOLUTE" modi moeglich,
  - bautrate 4800bps,
  - neu "m2" befehl fuer "C2" Kanal, (ist das Optimar kompatibel ?)
  - Optimar aktivierung in "System 2" -> "Verschiedenes" -> "Optimar aktivieren"
  - Wenn Optimar Interface Aktiviert ist, kiene andere befehle aktiv sind
  - manuel senden mit Taste 5, noch aktiv nur mit anderen baudrate
  - Messbild Taste 5 aktive Optimar modi Anzeige - Neue ikone Ikonen
  - parameter gilt nur fuer einmal ausschalten
- Messanzeige, digital Anzeige: Font groesse und position Verbesserung
  - Fontgroesse aphaengig von aufloesung ung Anzahl Merkmale
  - wenn 2 odeer 1 Merkmalle sind aktiv: immer Groesste Font, angepasst in freien platz unter

q:
- Toleranz & Warng. plausibilitaet pruefung? welche Standart Werte?
- welches Wert soll fuer Optimar geschickt werden: einheit = "um", kanal = "C1", offset = "kein"?
- welches fehler senden wenn optimar aktiv ist und z.B. "?" geschickt ist (senden EER2 oder EER3)
- soll T5 in Optimar modi aktiv sein?
---
FW ver 0.7.7.4B / 08.01.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.4B/C1202.bin))
- korrektur, Werte null-nah 0,0000 mm (0,0001mm)
- kein Hansymbol wenn Datenkabel nicht angeschlossen
---
FW ver 0.7.7.4 / 08.01.2021: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.4/C1202.bin))
- Logo im Startbild Verbessert
- Automatik Modi: warend messung Analogwerten gezeigt werden
- "AUTO" anzeige in Messbild
- Aktive Messunganzeige in Messung mit Gelbe und Gruene Zirkel
- Aktive Messunganzeige Ziffer Grau
- Start Verzuegreung nur einmal bei Zycklische Messung
- daten senden - when pausendauer != 0, immer (wenn kabel angeschlossen ist)
- In zyklus messung reset immer bei nue messung start
- fussschalter: MinMax Reset nur wenn in menu ausgewaehlt
- Anzeigeart: korigiert wechsel von Zeiger wenn mehr Merkmaele aktiv sind
---
FW ver 0.7.7.3 / 17.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.3/C1202.bin))
- FS debauncing fuer Messdauer (Start und Stop - fallende und steigende Flanke)
- Menu optionen ausgrauen und deaktivieren - wenn FS "Messdauer" asugewaehlt ist.
- FS bei "Messdauer", Messdauer Zeit und Pausendauer Zeit sind ignoriert
---
FW ver 0.7.7.2B / 17.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.2B/C1202.bin))
- Standardwerte fuer Messdauer, Pausendauer und StartVerzuegerung Zeiten sind gleich null.
- Ikone "Start" nach Pausieren geaendert,
- Ausgrauen und Deaktivieren: Messdauer, Pausendauer und StartVerzuegerung wenn Manuel Betriebsart asgewaehlt ist.
- FS Auswahl dynamische Regeln implemetiert (Moegliches Auswahl: entweder "Start" und/oder "Stop", oder "Messdauer").
- Neue werte in Automodi nur wenn Messung lauft
- Markierung mit Gruenen Zirkel das die Were sind angefoerdert
- Automodi: waerent messung in Pausenzustand Starttaste ohne optionalen Langdruck
- Reset bei neu Messung Start. Nach Pause Reset wird nich durchdefuehrt.
- bugfix id 45142: Formel Faktor Max Wert wenn "inch" ausgewaehlt 399.9999 statt 999.9999
- bugfix id 45142: zu lange formel endung aenderung von "..." auf "(...)", Formel verkurzung mit entvernen Leerzeichnen
- FS "Daten Senden", "Meistermessung" und "Reset Min Max" nur moeglich in Manuel und in Automatik wenn messung nicht leuft
- FS "Daten Senden" aktiv mit "Stop" oder "Messdauer" waehrend Messung aktiv.
---
FW ver 0.7.7.2 / 15.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.2/C1202.bin))
- bugfix no: 45309: "Auswahl aufloesung winkel" - interne werte umrechnung fue 0,1um gerundet
- korrigiert Werkseinstellung mit 1 Luftmodul - stuehrung - behoben
---
FW ver 0.7.7.1 / 10.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.1/C1202.bin))
- optimiertung von anzahl kanallen und modulen. wird benuzt in Modulen flashen
- Modulen Programieren ablauf verbesserung und texte besonderes in Pneumatische Modulen (richtige namen von modulen)
- Kurznamen fuer Pneumatische modulen Anzeige in Info-seite
- Automitik betriebsart verbesserung
- kleine aenderungen
---
FW ver 0.7.7.0 / 09.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.7.0/C1202.bin))
- Automatic mode implemented
---
FW ver 0.7.6.7 / 04.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.6.7/C1202.bin))
- datei ueberwachung fuer Messmodul flashen:
  - extention muss ".txt" sein,
  - Name muss "MarNet" string haben (case sensitive),
  - ganznamelaenge < 14 Zeichen
- Wenn 2 Luft modulen sind eingeschlossen, beide sind immer eine nach ander geflasht automatisch
- Luftmodulen flaschen parameter "12" ("PE-Wandler-Variante") wird bevor Flashen kopiert und nach neu Falshen wiedergestellt. Normal, nach flashen man muss das manuel einstellen (z.B in "MillimarN1700" PC Anwendung)
- Modul Falshen visusalisierung verbessert (auch Namen)
---
FW ver 0.7.6.6 / 01.12.2020: (datei unterladen: [C1202.bin](//goefs01/Mahr-Gruppe/Benutzergruppen/Transfer%20ENTW/Esslingen/C1202/Firmware/0.7.6.6/C1202.bin))
- new icons for MarCom not active
- removed digimatic parameter from menu and conditions
- Customer calibration with air gauge: initial calibration min and max: +-50 instead of +-300 for inductiove modules
- chenge of "edit button" in multichoice entry. added dynamic feature
- change in screen saver menu - one menu for on and time insead of two. matrix rain moved to "general settings"
- standard resolution for length and angle as middle one
- corrected form for no module display
- module flashing visualistaion, automatic reinit after flashing, names and dictionary
- Factory Corretion with Factory reset
- elimination of startup flash
- disabled bargraphs ake keymarkings

- Neue Ikonen Fuer MarCom wenn USB kabel nicht Verbunden ist. 4 Ikonen fuer (manuel, sequenziel, parallel und general) ausgegraut und gekruezt
- Digimatic Aktivierung entfernt von menu. Neues Logik: Digimatic bleibt aktiv immer wenn USB-kabel ist nicht verbunden. muss nicht aktiviert sein. Wenn kein USB-kabel ist nicht verbunden, snde funktion mit Taste, und Fussschalter sind nicht aktiv. Das wird mit asugegrauten Ikonen gezeigt. 
- Kundenkalibrierung fuer Luftmodulen: Initial "Min" "Max" Referenzwerte sind +-50um. Bei induktievemodulen bleibt +-300um
- neue Ikonen fuer Parametern mit mehrfach-auswahl. Dynamisch gesteuert.
- bilschirmschoner einstellung in Menu->Anzeige: Verbunden Ein-Aus mit Zeiteinstellung. Alternatives bildschirmschoner in System 2 "Verschiedenes"
- Standartwerte fuer Aufloesung (Laenge und Winkel) sind mittlere einstellung (wie in C1200)
- Verbessung im "Kein Modul" Anzeige, wenn kein modul angeschlossen ist
- Messmodul Firmware update in "System 2". datei asuwahl, Fortschritt Anzeige und Re-initialisierung nach Update. Flashen gild nur fuer ein modul. Wenn 2 Lufmodullen sind angeschlossen nur erstes wird geflasht.
  Um Messmodul zu flashen, kopieren FW-datei auf SD-karte. von menu->System 2->Modul programmieren
- bei Werkseinstellung Korrektur wird auf Wekrkorrektur umgestellt fuer beide kanaelle.
- neustart flash eliminiert
- demo balkenanzeige fuer Automatische messung deaktiviert

!!!Wichtig, 
um Bildschirmkopie zu machen, erst in "Menu->Setup 2->Verschidenes" Funktion Aktivieren.


