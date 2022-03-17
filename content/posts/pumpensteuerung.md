---
title: "Bau einer Pumpensteuerung"
date: 2022-03-05T22:23:53+01:00
draft: false
---
###  Überlegungen

Benötigt wurde eine Schaltung, die für eine niveauregulierte Befüllung eines Behälters eine Pumpe ein- und ausschaltet und dabei eine relativ große Hysterese hat. Das heißt, zwischen Einschaltzeitpunkt und Ausschaltzeitpunkt soll der Höhenunterschied beim Wasserstand etwa 10cm betragen. Die jeweilige Wasserhöhe wird mittels Schwimmschalter überwacht, wobei beim verwendeten Sensor beide Wasserstände über die unterschiedlich hoch angebrachten Schwimmer erfasst werden.  
![Schwimmerschalter](/schwimmer.webp)  
Die nachfolgend gezeigte Logikschaltung schaltet erst dann die Pumpe ein bzw. aus,
 wenn entweder beide Schalter geschlossen sind (höchster Wasserstand) oder beide offen sind (niedrigster Wasserstand). 
Fällt der Wasserstand nur wenig ab (nur einer der Schalter ist geschlossen), 
so läuft die Pumpe noch nicht an. Somit wird ein zu schnell aufeinander folgendes Ein- und Ausschalten der Pumpe verhindert.  

![Logikschaltung](/Logik.png)  

Die Logikschaltung wurde, wie im nächsten Bild zu sehen, mit zwei SN7400N Logikbasuteinen realisiert. Als Ausgangsansteuerung dient ein einfacher MOSFET (BS170). Die 12V der Anlage werden mittels 7805 Linearregler auf 5V reguliert. Dieser hat jedoch nur eine geringe Verlustleistung von ca. 300mW.  

![Schaltplan](/schaltung.webp)  


Die Schaltung kann hier als [PDF](/Ausgabe.pdf)  heruntergeladen werden.  

Die Logik-Schaltung wurde zunächst auf einem Breadboard aufgebaut und getestet.  

![Prefboard1](/prefboard_1.webp)  
![Prefboard2](/prefboard_2.webp)  

…sicher kein Kandidat für einen Schönheitspreis aber funktioniert zuverlässig und hat nur eine geringe Verlustleistung  




