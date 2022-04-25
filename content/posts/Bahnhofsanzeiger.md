---
title: "Anzeigen in der U-Strab Karlsruhe - Wenn Ausfall die Regel ist"
date: 2022-04-25
draft: false
---
In der Kombilösung in Karlsruhe werden die Abfahrten über Monitore angezeigt.  
Allderdings ist mir dabei aufgefallen, dass das Fahrgastinformationssystem häufig ( mehrmals pro Woche) ausfällt.
Deshalb  habe ich angefangen, Fotos von den Fehlern zu machen.
Nachfolgend stelle ich diese Bilder online.
Es handelt sich bei dem System um ein Windows 10 !?! auf welchem ein Firefox im Vollbildmodus eine Website anzeigt.  
Da es sich dabei nicht um ein echtes eingebettes System handelt, sind die Ausfälle häufig und andauernd ( mehrere Stunden).  

Immer wieder einzelne Displays komplett aus:  
![Dunkles Display](anzeigen/Fehlendes_Bild.jpg)
Wenn das Display nun dennoch funktioniert kommt es vor das der Firefox-Tab abstürzt (und das auch bleibt):  
![Tab crash](/anzeigen/Tab_Crashed.jpg)
Ein weiterer häufiger Fehler ist die Fehlermeldung "Forbidden". Das heißt, die Anzeige darf das, was ihre einzige Aufgabe ist nicht anzeigen...:  
![Forbidden](/anzeigen/Activate_Windows.jpg)

Dort ist auch das "Activate Windows" Wasserzeichen zu sehen, was von eimem Konfigurationsfehler zeugt...  

Es kann aber auch sein, dass der komplette Firefox abstürzt und sich Windows meldet. (Dieses Bild wurde übrigens am Tag der Eröffnung aufgenommen....)  
![Broswer Crash](/anzeigen/Minidump.jpg)

Wenn nun tatsächlich eine Website angezeit wird, kommt es vor das Bilder fehlen ( Firefox Zeichen für fehlendes Bild..):  
![Fehlendes Bild](/anzeigen/Fehlendes_Bild.jpg)

Aber auch im Normalbetrieb läuft nicht alles rund...:

{{< rawhtml >}}
<figure class="video_container" >
  <video controls="true" style="width: 30%;" allowfullscreen="false" poster="/anzeige/stottern.jpg">
    <source src="/anzeigen/stottern.mp4" type="video/mp4">
  </video>
</figure>
{{< rawhtml >}}  
Das Stocken des Laufbalken ist wahrscheinlich auf schlechte Programmierung oder falsche Konfiguration zurückzuführen...  
Man sieht also, dass man vllt. eine Qualitätskontrolle beim Softwarentwickler einführen sollte. Und das Windows als Embedded System weitesgehend ungeeignet ist. Und das ein Browser im Vollbildmodus **kein** eingebettetes System ist.

