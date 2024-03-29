# Wat is DNS

!!! info ""
    We kunnen eigenlijk niet over hosting praten zonder eerst DNS uit te leggen.
    DNS staat namelijk aan de basis van hosting en zonder DNS kan je hosting zo goed als niet functioneren.

## Een grote verzameling van IP adressen

Een website staat op een webserver. Zoals je computer thuis in een netwerk staat (al dan niet wifi) en op dat netwerk een IP adres heeft, staat een webserver ook in een netwerk ("het internet") en heeft die dus ook een IP adres.

!!! info "IP adres"
    Als je niet meer weet wat een IP adres is? Een IP adres is een unieke nummer van een computer waardoor je op een netwerk tussen verschillende computers kan communiceren. Enkele voorbeelden: `127.0.0.1` (localhost, je eigen computer of server), `192.168.0.1` (een intern bereikbaar ip adres), `195.12.45.65` (een extern bereikbaar ip adres op het internet)

!!! info "Web server"
    Een webserver is eigenlijk een computer die een specifiek doel heeft. In dit geval het "serveren" van websites. Meestal zijn servers wel wat krachtiger als gewone computers en hebben deze niet perse bvb. een scherm of keyboard aangesloten.

Dus elke website staat op een webserver en elke webserver heeft een IP adres. Als we surfen naar dat IP adres komen we terecht op die webserver.

Je zal bvb. merken dat als je naar [http://172.217.23.110](http://172.217.23.110){:target="_blank"} surft dat je op [google.com](https://google.com){:target="_blank"} terecht komt.

Maar er zijn **4.294 biljoen** ipv4 IP adressen in de wereld. Als we die moeten gaan onthouden voor elke website ... Like WTF, onmogelijk!

!!! info "ipv4 en ipv6"
    Een [ipv4](https://en.wikipedia.org/wiki/IPv4){:target="_blank"} adres is een 32-bit adres dat als volgt geformuleerd wordt: `123.123.123.123`. Omdat deze adressen op beginnen te geraken hebben we tegenwoordig ook [ipv6](https://en.wikipedia.org/wiki/IPv6){:target="_blank"} adressen om terug "plaats" te maken op het internet.

Dus 4.294 biljoen verschillende nummertjes die we niet kunnen onthouden, hoe doen we dat dan wel? Well, ... here comes DNS into play

## Domain Name Service

DNS staat voor **D**omain **N**ame **S**ervice. Weet je nog, [ons huis](/ons-huis) met het adres? DNS is dat adres. Dat verteld ons dus waar je website staat.

Dus met DNS kan je een naam koppelen aan een nummertje. bvb.:

> www.mijnwebsite.be = `173.194.69.99`

DNS zal ons dan vertellen dat we www.mijnwebsite.be eigenlijk moeten gaan zoeken op de webserver met IP adres `173.194.69.99`.
