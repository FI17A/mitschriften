Hardware
========

Mainboard
=========

Formfaktoren
------------

Normierungen für Mainboards, beschreiben:

- Abmessungen des gesammten Mainboards
- Arten, Anzahl und Lage der Anschlüsse
- Position und Art der Befestigungspunkte

Beispiele: ATX, BTX, ITX, (Micro, Nano, Mini, etc.)-ITX mit integriertem Passierschein A-38, etc.

Prozessorzyklus
===============

Ablauf von einem Programm:
--------------------------

0- Startbefehlsadresse in den Befehlszähler laden

1- Befehlszähler an RAM senden 

2- RAM holt befehl aus der Speicheradresse und sendet ihn an den Prozessor über eine
   Busleitung (Befehlsregister)
   
3- Befehl decodieren und Steuerbefehle für alle beteiligten Baugruppen bilden 

4- Ausführung

5- Befehlszähler erhöhen (in der regel um 1)


Prozessoraufbau	
===============

Es war einmal der __von-Neumann-Rechner__: 1 Bus für Befehle, Addressen und Daten,
diese stellten einen Flaschenhals dar.

Dann kam die __Harward-Architektur__: Je ein Addressbus, Befehlsbus und Datenbus.

\*Das stimmt so nicht wirklich, [*Von-Neuman-Architektur* auf Wikipedia](https://de.wikipedia.org/wiki/Von-Neumann-Architektur)

-  Register: Speichern numerische Werte
- Akkumulator: Ein besonderes Register, in das Ergebnisse von Operationen gespeichert werden.
- Rechenwerk
	- *Arithmetic Logic Unit*: Führt Arithmetische und Logische operationen aus.
	- *Floating Point Unit*: Kann besser mit Gleitkommazahlen rechnen als ALU.
- Steuerwerk
	- Befehlsregister: Speichert aktuellen Befehl (in Binärer representation)
	- Befehlsdecoder: Wandelt Befehl in die entsprechenden Operationen um, die die Hardware letztlich durchführt.

![Prozessor Aufbau](img/hardware/cpu_1.svg)

Microprogramme
==============

Bei Programmen wiederholen sich oft muster von Befehlen. Diese können in sogenannte
Microprogramme, also *komplexe Befehle*, zusammengefasst werden, um weniger einzelne Befehle
über den Bus laden zu Müssen. (Weniger speicherzugriff = schnellere Ausführung)

Dies erhöt die Komplexität des Prozessors, der nun auch besagte Microprogramme speichern
und dekodieren muss.

Moderne Prozessoren haben deshalb Keine Microprogramme mehr, da es mit moderner
Technik so schneller geht.

Weiterentwicklungen
===================

- Stetige Erhöhung des Arbeitsspeichers
	- Speichermanagement in externen chipsatz ausgelagert
- Alle IO operationen in chipsatz ausgelagert
	- North Bridge: Grafik + Speicher, sehr schnell
	- South Bridge: Alles andere, nicht ganz so schnell
- Floating Point Unit
- Cache (Speicher im CPU)
	- L1 cache: Im Kern
	- L2 cache: Im Kern
	- L3 cache: Außerhalb der Kerne
