# Name server lookups

## NSLOOKUP

Een name server lookup of nslookup is het opzoeken van technische informatie van een domeinnaam. Dit kan zijn welke name servers een domeinnaam gebruikt maar ook welke records naar welk ip adres gaan.

Een nslookup kan je op elke computer (mac, windows of linux) uitvoeren door het commando `nslookup` te gebruiken in de command line interface.

![](/_resources/graphics/cleanshot-2021-09-18-at-17.24.02.jpg)

!!! info "NSlookup"
    Meer weten over hoe je het nslookup commando moet gebruiken? Check deze [youtube video](https://www.youtube.com/watch?v=jf-x76XYY2o){:target="_blank"}.

## Online DNS lookups

Er zijn ook verschillende manieren om online DNS records op te zoeken. Een super makkelijke website om dit te doen van onze vrienden van [Spatie](https://spatie.be){:target="_blank"} is [dnsrecords.io](https://dnsrecords.io/){:target="_blank"}.

Daar kan je op de website intypen over welk domein of welke record je meer informatie wilt en dan zullen zij die nslookup voor u doen.

![](/_resources/graphics/cleanshot-2021-09-18-at-17.30.42.jpg)

![](/_resources/graphics/cleanshot-2021-09-18-at-17.30.52.jpg)

!!! info "dnsrecords.io"
    De broncode van de [dnsrecords.io](https://dnsrecords.io){:target="_blank"} website is ook te vinden op de github van spatie: [https://github.com/spatie/dnsrecords.io](https://github.com/spatie/dnsrecords.io){:target="_blank"}

## Around the world

Als alle mensen ter wereld telkens naar uw nameserver moeten gaan om een DNS record te "resolven" dan gaat uw server zwaar belast worden en als mensen aan de andere kant van de wereld wonen dan gaat dat niet snel gaan en we willen toch een snel internet, right?

!!! info "DNS resolving"
    "resolven" (resolve / resolving) is het omzetten van een naam (bvb. kdg.be) naar een IP adres (bvb `123.123.123.123`). Je zal deze term wel meer horen, zeker onder sysadmins.

De oplossing voor dit probleem zijn **root servers**. Root servers zijn servers die opereren in de DNS root zone. Zo heb je 13 root servers, van a tot m. bvb. a.root-servers.org, b.root-servers.org, ...

![Bron: https://www.cloudflare.com/learning/dns/glossary/dns-root-server/](/_resources/graphics/dns-root-server.webp)

!!! info "Root servers"
    Meer info over welke root servers er allemaal zijn en door wie ze beheerd worden vind je op [root-servers.org](https://root-servers.org/){:target="_blank"}

    Meer info over wat een root server juist is vind je hier: [cloudflare.com/learning/dns/glossary/dns-root-server](https://www.cloudflare.com/learning/dns/glossary/dns-root-server/){:target="_blank"}

Als je een domeinnaam opzoekt gaat jouw dns server (die door uw provider wordt aangeboden, bvb van telenet of een publieke van google (= `8.8.8.8`)) aan de root servers vragen wat de dns records zijn die dan door de root server aan de domein name server wordt gevraagd. De root en provider servers gaan deze DNS dan ook cachen.

!!! info "Caching"
    Caching is gegevens lokaal bijhouden zodat deze in de toekomst niet meer opgevraagd moeten worden.

Op DNS records kan je een TTL instellen. Een **T**ime **T**o **L**ive. Hiermee kan je bepalen hoelang de servers mogen wachten voor ze naar uw nameserver moeten kijken om nieuwere gegevens op te vragen.

!!! warning "Around the world"
    Door deze DNS caching kan het tot 24u duren eens een wijziging op DNS niveau "heel de wereld" rond is. Hou hier dus rekening mee!
