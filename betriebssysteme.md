Betriebssysteme
===============

Zweckbestimmung der Betriebssysteme
===

1.1. Einteilungsmöglichkeiten der Software

- Anwendungssoftware
	- Problem- und Branchenorientiert
		- Standardsoftware
		- Komerzielle Software
		- Branchensoftware
		- Technische bzw. wissenschaftliche Software
- Systemsoftware
	- Betriebssysteme
	- Dienst- und Hilfsprogramme
	- Software-Werkzeuge
	- Übersetzungssoftware
	- Programmiersprachen

Aufgaben und Funktionen
===

- Nutzerverwaltung
- Betriebsmittelverwaltung
- Task- / Prozessmanagement
- Zugriffsschutz
	- Unmittelbar mit Dateiverwaltung verbunden
- Dateiverwaltung
- EVA-Steuerung (Eingabe - Verarbeitung - Ausgabe)
- Speicherverwaltung
- Benutzeroberfläche
- Ablaufsteuerung
	- Welche Prozesse wann abgearbeited werden
- Interruptverarbeitung
- Netzwerkfähigkeit
- Multi-Tasking
	- Kooperativ
	- Präemtiv
- Abrechnung
- Multi-User
- Abstraktion
	- Benutzerfreundliche Darstellung
- Prozesssynchronisation
- Interprozesskommunikation

Arten
===

Unterteilungen nach:

- Betriebsart
	- Stapelverarbeitung
	- Interaktive Systeme / Dialogverarbeitung
	- Echtzeitsysteme
- Leistungsumfang
	- Grpßrechner
	- Systeme für mittlere Datentechnik
	- Systeme für PC
	- Systeme für Einbaucomputer
- Portabilität
	Portabel vs. nicht portabel

Stapelverarbeitung
---

(= batch processing)

Auftrag wird zusammengestellt und an das System übergeben.
Nach der Verarbeitung, werden die Ergebnisse an den Nutzer übergeben.
Man unterscheidet zw. offenem oder geschlossenem Betrieb.

- Gut bei hohem Datenaufkommen
- Benötigt vehlerfreie Programme

Dialogverarbeitung
---

Benutzer besitzt eigene Tastatur und eigenen Bildschirm und hat damit die Möglichkeit, den Ablauf zu kontrollieren und gezielt beeinflussen.
In der Art der Dialogfürung werden zwei arten unterschieden:

1. Teilnehmerprinzip: Dialog mit einem Kommando-Interpreter und mehreren Teilnehmern, die jeder für sich individuelle Programme mit individuellen Daten ausführen.
2. Teilhaberprinzip: Mehrere Benutzer setzen gleichzeitig das gleiche Programm ein und arbeiten am gleichen Datenbestand. (Auskunfts- oder Buchungssysteme)

Echtzeitsysteme
---

(= realtime processing)

Ein Basisprozess wird durch einen Rechner gesteuert und Überwacht. Dieser Prozessrechner muss ständig über alle Parameter des Prozesses informiert sein.
Unterscheidung:

1. Hartes Echtzeitsystem: Verzögerungen machen daten Wertlos bzw. führen zu katastrophalen Folgen.
2. Weiches Echtzeitsystem: Gewisse Toleranzen sind erlaubt, Verzögerungen führen zu akzeptablen Kostenerhöherungen.

Echtzeit: Relative schnelligkeit durch Toleranzen bestimmt.

Zielfunktionen
===

[Friedrich bitte verfollständigen!]

Qualitätsansprüche
===

- Robustheit
	- Fehler in OSI-8 abfangen
- Effizienz
- Datenschutz
	- Sicherung gegen Verlust von Daten
	- Am besten Automatisiert

Architekturen von Betriebssystemen
===

Monolithische Systeme
---

Struktur besteht aus: \*trommelwirbel\* KEINE STRUKTUR!

System calls == Aufrufe von Subroutinen

1. Sprung von Nutzer-Modus in Kern-Modus
2. Lookup in dispatcher table, Parameter überprüfen
3. Subroutine Starten
4. Rücksprung in Nutzer-Modus, Rückgabe der Ergebnisse

Geschichtete Systeme
---

(= Ebenenansatz konsequent durchgesetzt)

Alle Betriebssystemschichten kommunizieren nur mit der nächstniedrigeren Schicht. Bei "Quasikonsistenter" schichtung können auch schichten übersprungen werden.

Zwei sichtweisen:
- Äußere Erscheinungsform
- Innere Funktionsweise

Die Architektur kann Logisch (Von außen, wie es der nutzer wahrnimmt) oder Physisch (Von innen, wie es tatsächlisch implementiert ist) betrachtet werden.

---------------------------------------

Virtuelle Maschinen
===

[kommt noch]
