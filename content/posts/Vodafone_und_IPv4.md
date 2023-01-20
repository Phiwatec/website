---
title: "Vodafone und IPv4 - Änderungen mitten am Tag"
date: 2022-08-19
draft: false
---

Am Nachmittag des 19.08. bekam ich probleme bestimmte Websites zu erreichen. 
Um dem auf den Grund zu gehen, loggte ich mich im Router ein und stellte fest, dass ich als WAN Gateway IPv4 Adresse eine private Adresse (siehe unten) bekommen habe. 
![PrivateIPv4](/private_v4.png)
Ein Telefonat mit Vodafone - der Technikabteilung wohlgemerkt - brachte leider nicht viel zu Tage. Laut Ihnen soll ich natives Dualstack haben. Nur bekomme ich leider keine öffentliche IPv4 Adresse.. 
Weitere Infos folgen..  
Als Workaround habe ich im Moment auf das Öffentliche NAT64/DNS64 Gateway von Christian Dresel (https://nat64.dresel.systems) umgestellt. So werden aus den IPv4 Adressen der Server IPv6 Adressen synthetisiert, welche dann im Gateway auf IPv4 übersetzt werden. Vielen Dank an Herrn Dresel und Freifunk Franken, welche diesen Dienst bereitstellen.  
**Edit 20/01/2023:**  
Das NAT64 Gateway von Herrn Dresel existiert leider nicht mehr.  
Als Alternative gibt es unter [https://nat64.xyz/](https://nat64.xyz/) eine Auflistung öffentlicher NAT64 Gateways.  
Nach weiterer Untersuchung hat sich herausgestellt, das die IP vom DHCP-Server des Kabelmodems vergeben wird. Weshalb dies der Grund ist, muss ich noch evaluieren.  
Als Workaround kann im Router die IP des Modems als verbotener DHCP Host eingetragen werden. Die Antwort des Vodafone DHCPs dauert dann allerdings relativ lange. Wieso dies der Fall ist, kann ich momentan noch nicht sagen.  
