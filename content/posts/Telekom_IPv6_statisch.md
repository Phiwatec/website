---
title: "Statisches IPv6 Präfix für Privatkunden und Best Practises"
date: 2023-05-30
draft: false
---

Die Telekom bietet bei Ihre Privatkunde-Tarifen keine Möglichkeit statische IPv6 Präfixe zu bekommen.
Begründet wird dies unter anderem mit den hohen Kosten seitens der Telekom.  
Allerdings erschließt sich dieser Preis nicht. IPv6 Adress Space ist dank der enormen Addressmenge kaum nennenswert teuer.
Aber selbst wenn er es wäre, gibt die Begründung keinen Sinn: Auch bei dynamischen Präfixen wird die gleiche Anzahl an Präfixen benötigt. Sie werden lediglich immer neu zugeteilt.  
Der Verwaltungsaufwand wäre dank Software auch nicht nennenswert. Die die DHCP bzw. PPPoE Session werden ja bereits verwaltet.  
Die Zuweisung von Addressen geschieht aus einem Pool, welcher ebenfalls Verwaltet werden muss. Eine Erweiterung für statische Zuweisungen gibt es ja bereits für Geschäftskunden.

## RIPE

Alle IP Addressen in Europa werden von der RIPE vergeben. Diese emphielt ausdrücklich auf Ihrer Website die **statische** Zuweisung von IPv6 Präfixen.  
Siehe: [RIPE](https://www.ripe.net/publications/docs/ripe-690#5-2--why-non-persistent-assignments-are-considered-harmful)

Es ist daher fraglich, warum ein großer deutscher Internetprovider sich nicht an die Empfehlungen der europäischen Addressvergabestelle halten.

## Aber warum statisch? DNS regelt doch?

DNS kann für viele Anwendungen ein Workaround sein. Allerdings:

- Ist es aufwendiger die DNS Records jedesmal zu aktualisieren ( natürlich automatisiert aber fehleranfällig)
- Für immer wieder zu Konnektivitätsproblemen da der neue Record noch nicht bei Endgerät angelangt ist
- DNS funktionert nur bei Server Anwedungen. Wenn z.B. ein VPN für den Zugriff auf das Heimnetz betrieben werden soll, so kann man den Clients **keine** globale IPv6 Addresse zuweisen, da sie sich ändern kann. Hier muss entweder nur IPv4 oder NAT66 verwendet werden. Beide Lösungen sind aber nur Notlösungen und netzwerktechnisch eher ungünstig.
