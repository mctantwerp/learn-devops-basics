# Hoe werkt DNS

## Domenextensie

We beginnen bij een domeinnaam. Zoals bvb. **kdg.be**. Dit is een **.be** domeinnaam. \(**.be** staat hier voor **België**, een echte Belgische domeinnaam dus\) Een .be domeinnaam kan je registreren bij [dns.be](https://dns.be). Als je zo'n domeinnaam registreert moet je uw persoons gegevens opgeven en ook één of meerdere **nameservers**.

{% hint style="info" %}
Een .be domeinnaam kan je bij **dns.be** registreren als je zelf een domein reseller bent. \(iemand die domeinnamen verkoopt\) Er zijn maar een beperkt aantal bedrijven die dat zijn dus meestal gaan wij als web developers via een reseller onze domeinen kopen, zoals bvb. via [Combell](https://www.combell.com/nl/domeinnamen).
{% endhint %}

Lees meer over domein extensies:

{% page-ref page="domeinextenties.md" %}

## Nameserver

Een nameserver is een server die weet waar je website "woont". Dus de server die ons kan vertellen dat [www.kdg.be](www.kdg.be) op het IP adres `94.176.99.133`  beschikbaar is.

Via [dns.be](https://dns.be) kan je bvb. bekijken welke nameserver [kdg.be](https://www.kdg.be) gebruikt.

![](../../.gitbook/assets/cleanshot-2021-09-18-at-17.16.45.jpg)

Dus in dit geval zullen de servers van **belnet** ons kunnen vertellen dat de website van KdG op het ip adres `94.176.99.133` staat.

{% hint style="info" %}
Het opzoeken van een nameserver \(of andere DNS gerelateerde informatie\) noemt men een **name server lookup** \(kort: **nslookup**\)
{% endhint %}

Lees hier meer over Name server lookups:

{% page-ref page="name-server-lookups.md" %}

## DNS records

We weten nu al dat we:

* [ ] Een domeinnaam registreren op een bepaalde extensie
* [ ] Een nameserver op deze naam moeten instellen

Next up: een configuratie koppelen aan je domeinnaam.

