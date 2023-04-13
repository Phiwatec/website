---
title: "Der Digitalführerschein - Ein Beispiel wie man es nicht macht"
date: 2023-04-13
draft: false
---

Unter [https://difü.de/](https://difü.de/) gibt es die Möglichkeit einen digitalen Führerschein zu absolvieren. Dieser wird unter anderem von Bundesministerium des Inneren und für Heimat gefördert:
![Förderung](/dif%C3%BC/F%C3%B6rderung.png)
Dabei ist die technische Umsetzung der Website leider nicht ganz auf dem Stand der Technik.  
Um das Zertifikat zu bekommen, muss nach Anmeldung eine Fragerunde absolviert werden.
Die Technik dahinter ist jedoch nicht besonders manipulationssicher...

Nach dem Start der Fragerunde werden die Fragen vom Server angefragt. Soweit so normal.  
Nur werden in der Response nicht nur die Fragen übermittelt sondern auch gleich die richtigen Antworten.
![GET Request](/dif%C3%BC/Get.PNG)
![GET Request](/dif%C3%BC/JSON.PNG)
Wer sich also ein wenig mit den Developer-Tools des Browsers auskennt hat den Test also mehr oder weniger automatisch bestanden, da man einfach die Fragen im JSON suchen und Antwort eintragen kann.  
Diesen Aufwand muss man sich aber eigentlich gar nicht machen, da die Antworten nach Ende der Umfrage im Browser ausgewertet und dann das Ergebnis ans Backend geschickt wird.
![GET Request](/dif%C3%BC/Post.PNG)
Es genügt also nach Beginn der Fragerunde einfach ein Post-Request mit dem gewünschten Scores an den Server zu schicken und bekommt diese gutgeschrieben.  
Man kann sich dabei auch mehr Punkte geben als eigentlich erreichbar wären. ;)

So eine Technik würde wahrscheinlich in der Digitalführerschein-Prüfung durchfallen.
