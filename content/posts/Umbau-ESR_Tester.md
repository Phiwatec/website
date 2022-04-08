---
title: "ESR Tester Umbau auf 9V Block"
date: 2021-03-02
draft: false
---

![Das Atlas ESR70 Messgerät](/messgeraet_haupt.webp)  

Zum Testen von Kondensatoren auf Kapazität und [ESR](https://de.wikipedia.org/wiki/Kondensator_(Elektrotechnik)#Normung_und_Ersatzschaltbild) (Equivalent Series Resistance = Serienwiderstand) verwende ich das Peak Atlas ESR 70.
Leider verbraucht das Gerät auch im ausgeschalteten Zustand Strom, wenn auch nur etwa 0,5 µA.
Benötigt wird eine relativ teure 12 Volt-Batterie, wie sie auch in Garagentor-Fernbedienungen oder Steckdosen-Fernschaltern verwendung finden.
Die Batterie kann man nur entnehmen, wenn man das Gehäuse aufschraubt, was man natürlich nicht für nur gelegentliche Messungen macht.
So passiert es, dass man das Gerät einschaltet und der Strom nur noch für eine Messung ausreicht und dann geht nichts mehr.
Eine Ersatzbatterie ist auch nicht immer gleich beim Supermarkt um die Ecke erhältlich.

![Aufgeschraubt mit Original Batterie](/esr_aufgeschraubt.webp)

So kam mir die Idee mit meinem geregelten Labornetzteil auszuprobieren, bei welcher Mindestspannung das Gerät noch zuverlässig arbeitet.
Und Überraschung: das geht ab 8 Volt!
Erst darunter kommt der LowBat-Hinweis.
Dann habe ich noch getestet, ob die Messergebnisse mit den unterschiedlichen Spannungen unterschiedlich ausfallen, was aber nicht der Fall war.

![Stromversorung mitttels Labornetzteil….](/esr_mit_netzteil.webp)

![… und einer Spannung von 8V](/labornetzteil.webp)

Wenn das Gerät mit 8 Volt zufrieden ist dann funktioniert es mit einer 9 Volt Blockbatterie erst recht.
Also habe ich ein Anschlussclip für 9-Voltbatterien auf die Platine gelötet und das Doppelkabel durch eine ohnehin vorhandene Gehäuseöffnung nach draußen geführt.
So kann ich nun günstige 9 Volt-Zellen verwenden (also auch Akkus) und diese bei Nichtgebrauch des Gerätes leicht abclipsen was die Verwendungssicherheit erhöht und gleichzeitig Geld spart.

![Das Kabel vom externen Clip](/esr_cable_clip.webp)

![So sieht es fertig aus ohne und …](/esr_closed.webp)

![mit neuer Batterie.](/esr_closed_with_bat.webp)

Hinweis:
Test
Das Gerät gibt es mittlerweile in einer 1,5 Volt-Version, die mit ganz normalen 1,5 Volt-Micro Batterien (AAA) betrieben werden kann.

Ich bin nicht verantwortlich, wenn die Modifikation bei jemand zum Defekt des Gerätes führt.
