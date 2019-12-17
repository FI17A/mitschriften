<<<<<<< Updated upstream
Strukturierte Verkabelung
=========================

Breitbandinternet
=================

Großer Frequenzbereich mit vielen Kanälen und hohe Übertragungsrate.
Alles über 64 kbit/s ist Breitband.

Sonderformen
------------

Glasfaseranschluss
------------------

=======
>>>>>>> Stashed changes
Transmission Control Protocol
=============================

Sliding-Window-Prinzip
----------------------

[Wikipedia](https://en.wikipedia.org/wiki/Sliding_window_protocol)

Überlastkontrolle
-----------------

TCP erkennt Überlastung durch hohe Paketverlustraten, hat sonst aber
keine anderen Mechanismen, um Netzüberladung zu erkennen. Das Problem
ist: die Datagramme werden nur beim Sender und beim Empfänger als TCP
Pakete interpretiert, und im restlichen Netz als verbindungslose IP
Datagramme behandelt.\
\
Algorithmen zur Überlastkontrolle:

-   Slow-Start-Algorithm

-   [Nagle-Algorithm](https://en.wikipedia.org/wiki/Nagle's_algorithm)

-   Ermitteln der RTT[^1]

Weitere informationen hierzu sind auf
[Wikipedia](https://en.wikipedia.org/wiki/Sliding_window_protocol) zu
finden.\
\
Mögliches Problem dabei: [Silly Window
Syndrome](https://en.wikipedia.org/wiki/Silly_window_syndrome)

<<<<<<< Updated upstream
=======
Strukturierte Verkabelung
=========================

Breitbandinternet
=================

Großer Frequenzbereich mit vielen Kanälen und hohe Übertragungsrate.
Alles über 64 kbit/s ist Breitband.

Sonderformen
------------

Glasfaseranschluss
------------------

Kein plan, ist aber nicht mehr Glasfaser
----------------------------------------

LEX

:   Local Exchange – Teilnehmervermittlungsknoten\
    Teilnehmer und Leitungen werden an
    Vermittlungsstellen angeschlossen.

TEX

:   Transit Exchange – Durchgangsnetzknoten\
    Dient für Übertragung der Daten im Netz.

UNI

:   User Network Interface\
    Anschluss von Teilnehmergeräten an LEX.

    -   Public UNI

    -   Private UNI

NNI

:   Network Node Interface\
    Schnittstelle zwischen Netzknoten.

Die Elemente verzweigen $X$, leiten $X$ um, fassen $X$ zusammen, und
passen $X$ an\
mit $X$ = Datenströme\
Vorfeldeinrichtungen:

Multiplexer

:   Fassen Datenströme Signalisierung zusammen

Konzentratoren

:   Fassen Datenströme Signalisierung zusammen

Cross-Connect (CC)

:   Lenken und verteilen zusammengefasste...

Interworking Unit (WU)

:   Anpassung für Verbindung bestehender Netzwerke

$\{Multiplexer\} \cup \{Konzentratoren\} = AAE$

Teilnehmeranchluss bei Breitbandnetzen
--------------------------------------

-   Alle Elemente sowie Referenzpunkte sind für breitbandige
    Kommunikation ausgelegt

-   Netzabschluss durch B-NT1 (Public-UNI)

-   ...And then the slide was gone.

>>>>>>> Stashed changes
[^1]: Round-Trip-Time
