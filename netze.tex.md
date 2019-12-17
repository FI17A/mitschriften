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

[^1]: Round-Trip-Time
