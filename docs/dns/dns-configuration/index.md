# DNS configuratie

Je DNS configureren doe je met DNS records die je dan opslaat op uw nameserver.

!!! info "DNS notatie"
    Bij de uitleg van de DNS records zal ik het ook telkens over de technische notatie hebben. Dit is de notatie in het DNS server programma "BIND". Je gaat dit, bij basis hosting gebruik, nog zelden tegenkomen maar sommige hosters geven wel de kans om deze notatie te gebruiken. Voor de technische profielen onder ons is dat veel sneller en leuker om te doen ipv wat rond te klikken 😊

De DNS instellingen zal je meestal doen via het controlepaneel van je hoster. Bij elk controle paneel zal dat er net iets anders uitzien maar de achterliggende records zullen altijd hetzeflde zijn.

!!! info ""
    Weten welke DNS records er zijn en hoe je deze kan gebruiken stelt je dus in staat om op via alle mogelijke systemen je DNS te beheren.

Je zal zien dat DNS records ook een TTL waarde hebben. Dit is de **T**ime **To** **Live**. Dit is een suggestie voor nameservers die verteld hoe regelmatig er moet nagekeken worden of de DNS record is gewijzigd. Het resultaat van het DNS record zal voor die periode in de **cache** bijgehouden worden.

Er zijn verschillende DNS record types die je kan gebruiken:

<div class="grid cards" markdown>
- [:material-dns-outline: __A__ record](a-record)
- [:material-dns-outline: __CNAME__ record](cname-record)
- [:material-dns-outline: __MX__ record](mx-record)
- [:material-dns-outline: __TXT__ record](txt-record)
- [:material-dns-outline: __AAAA__ record](aaaa-record)
- [:material-dns-outline: __NS__ record](cname-record)
</div>
