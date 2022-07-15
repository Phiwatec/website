---
title: "Anzeigen in der U-Strab Karlsruhe - Wenn Ausfall die Regel ist"
date: 2022-04-25
draft: false
---

Im Tunnel der Kombilösung in Karlsruhe werden die Abfahrten über Monitore angezeigt.  
Allderdings ist mir dabei aufgefallen, dass das Fahrgastinformationssystem häufig (mehrmals pro Woche) ausfällt.
Deshalb habe ich angefangen, Fotos von den Fehlern zu machen.
Nachfolgend stelle ich diese Bilder online.
Es handelt sich bei dem System um ein Windows 10 (!?) auf welchem ein Firefox-Browser im Vollbildmodus eine Website anzeigt.  
Da es sich dabei also nicht um ein echtes eingebettes System handelt, sind die Ausfälle häufig und länger andauernd (manchmal mehrere Stunden).

Immer wieder fallen einzelne Displays komplett aus:  
![Dunkles Display](/anzeigen/Kaputt.jpg)

Wenn das Display funktioniert kommt es vor, dass der Firefox-Tab abstürzt (und das auch so bleibt):  
![Tab crash](/anzeigen/Tab_Crashed.jpg)

Ein weiterer häufiger Fehler ist die Fehlermeldung "Forbidden". Das heißt, die Anzeige darf das, was sie anzeigen soll, nicht anzeigen...:  
![Forbidden](/anzeigen/Activate_Windows.jpg)

Dort ist auch das "Activate Windows"-Wasserzeichen zu sehen, was eimen Konfigurationsfehler vermuten lässt...

Es kann aber auch sein, dass der Firefox-Browser komplett abstürzt. (Dieses Bild wurde übrigens am Tag der Eröffnung aufgenommen....)  
![Broswer Crash](/anzeigen/Minidump.jpg)

Wenn nun tatsächlich eine Website angezeit wird, kommt es vor, dass Bilder fehlen (Firefox-Symbol für fehlende Bilder vor den Wagen..):  
![Fehlendes Bild](/anzeigen/Fehlendes_Bild.jpg)

Oder es wird einfach mal die Schrift- und Bildgröße geändert. Wohlbemerkt nur bei einer einzigen Anzeige...  
Normale Größe:  
![Normale Größe](/anzeigen/normal.jpg)
![Zu klein](/anzeigen/kleine_schrift.jpg)


Aber auch im Normalbetrieb läuft nicht alles rund...:

{{< rawhtml >}}

  <video controls="true" style="width:50%;" allowfullscreen="false" poster="/anzeigen/stottern.jpg">
    <source src="/anzeigen/stottern.mp4" type="video/mp4">
  </video>

{{< /rawhtml >}}

Das Stocken des Laufbalkens ist wahrscheinlich auf eine ineffiziente Programmierung oder falsche Konfiguration zurückzuführen...  
Man sieht also, dass man eine bessere Qualitätskontrolle beim Software-Entwickler einführen sollte. Und es zeigt sich, dass Windows als Embedded System weitestgehend ungeeignet ist. Und dass ein Browser im Vollbildmodus eben noch **kein** eingebettetes System ist...

Hier noch ein Bonus:  
Der vollständige Bootprozess:  
{{< rawhtml >}}

<video controls="true" style="width:50%;" allowfullscreen="false" poster="/anzeigen/boot.png">

<source src="/anzeigen/boot.mp4" type="video/mp4">
</video>
{{< /rawhtml >}}
