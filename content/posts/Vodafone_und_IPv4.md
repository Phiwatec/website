---
title: "Vodafone und IPv4 - Änderungen mitten am Tag"
date: 2022-07-05
draft: false
---

Am Nachmittag des 19.08. bekam ich probleme bestimmte Websites zu erreichen. 
Um dem auf den Grund zu gehen, loggte ich mich im Router ein und stellte fest, dass ich als WAN IPv4 Adresse eine private Adresse (siehe unten) bekommen habe. 
![PrivateIPv4](/private_v4.png)
Diese hatte jedoch kein Zugriff auf das Internet. Ein Telefonat mit Vodafone - der Technikabteilung wohlbemerkt - brachte leider nicht viel zu Tage. Laut Ihnen soll ich natives Dualstack haben. Nur bekomme ich leider keine öffentliche IPv4 Adresse.. 
Weitere Infos folgen..  
Als Workaround habe ich im Moment auf das Öffentliche NAT64/DNS64 Gateway von Christian Dresel (https://nat64.dresel.systems) umgestellt. So werden aus den IPv4 Adressen der Server IPv6 Adressen synthetisiert, welche dann im Gateway auf IPv4 übersetzt werden. Vielen Dank an Herrn Dresel und Freifunk Franken, welche diesen Dienst bereitstellen.