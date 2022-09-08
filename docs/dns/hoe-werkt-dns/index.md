# Hoe werkt DNS

## Domenextensie

We beginnen bij een domeinnaam. Zoals bvb. **kdg.be**. Dit is een **.be** domeinnaam. (**.be** staat hier voor **België**, een echte Belgische domeinnaam dus) Een .be domeinnaam kan je registreren bij [dns.be](https://dns.be){:target="_blank"}. Als je zo'n domeinnaam registreert moet je uw persoons gegevens opgeven en ook één of meerdere **nameservers**.

!!! info ""
    Een .be domeinnaam kan je bij **dns.be** registreren als je zelf een domein reseller bent. (iemand die domeinnamen verkoopt) Er zijn maar een beperkt aantal bedrijven die dat zijn dus meestal gaan wij als web developers via een reseller onze domeinen kopen, zoals bvb. via [Combell](https://www.combell.com/nl/domeinnamen){:target="_blank"}.

!!! warning "Let op als je een domeinnaam registreert"
    Als je een domeinnaam registreert moet je je gegevens doorgeven. Je kan hier bvb. ook een Bedrijfsnaam doorgeven. Vanaf je dat doet zullen al je gegevens publiek beschikbaar staan op dns.be. Dus denk hier goed over na en geef bvb. geen bedrijfsnaam op als je geen bedrijf hebt 😉. Als je geen bedrijfsnaam opgeeft dan zullen je gegevens verborgen zijn.

<div class="grid" markdown>
[:octicons-link-16: Meer over domein extensies.](domeinextensies)
{ .card }
</div>

## Nameserver

Een nameserver is een server die weet waar je website "woont". Dus de server die ons kan vertellen dat [www.kdg.be](www.kdg.be) op het IP adres `94.176.99.133`  beschikbaar is.

Via [dns.be](https://dns.be){:target="_blank"} kan je bvb. bekijken welke nameserver [kdg.be](https://www.kdg.be){:target="_blank"} gebruikt.

![](/_resources/graphics/cleanshot-2021-09-18-at-17.16.45.jpg)

Dus in dit geval zullen de servers van **belnet** ons kunnen vertellen dat de website van KdG op het ip adres `94.176.99.133` staat.

!!! info ""
    Het opzoeken van een nameserver (of andere DNS gerelateerde informatie) noemt men een **name server lookup** (kort: **nslookup**)

Lees hier meer over Name server lookups:

<div class="grid" markdown>
[:octicons-link-16: Meer over name server lookups.](name-server-lookups)
{ .card }
</div>

## DNS records

We weten nu dus al dat we:

* [x] Een domeinnaam registreren op een bepaalde domeinnaam extensie
* [x] Een nameserver op deze domeinnaam moeten instellen

[Next up: een configuratie koppelen aan je domeinnaam. :material-arrow-right:](/dns/dns-configuration/){ .md-button }
