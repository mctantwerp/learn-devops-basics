# CNAME record

Een nadeel van A-records is dat IP adressen kunnen wijzigen.

!!! example "Stel"
    Je hebt een web server op IP adres 123.123.123.123 en heb hier 35 websites op staan. Het is echter tijd voor een nieuwe server en deze krijgt een nieuw IP adres, bvb.: 456.456.456.456. Nu moet je al je DNS records gaan aanpassen met dat nieuwe IP adres.

Hier komt het CNAME record in play. CNAME staat voor **Canonical Name** (1), dit is een record die doorverwijst naar een andere hostname.
{ .annotate }

1.  Canonical staat voor "In relation to"

Dus als je `www.mijnwebsite.be IN CNAME server.mijnwebsite.be` instelt dan gaat de `www.mijnwebsite.be` record naar het IP adres van `server.mijnwebsite.be`.

Je kan zo meerdere hosts naar die 1ne server record zetten en zo hoef je maar 1x het ip adres te wijzigen.

!!! error "BELANGRIJK"
    Het is jammergenoeg niet mogelijk om een root record als cname te gebruiken. Dus de zogenaamde **@** __moet__ altijd naar een IP adres staan.

CNAME records worden vooral veel gebruikt bij extern gehoste diensten zoals Google sites, WIX sites, squarespace, spotify, etc....

Dus als een groot bedrijf een website host die jij wil gebruiken zullen ze je meestal vragen om hier een CNAME record voor toe te voegen. Zo moet je je geen zorgen maken als het IP adres evt. zou wijzigen.

Bvb. voor google: `www.mijnwebsite.be IN CNAME ghs.googlehosted.com`

!!! tip "Meer lezen?"
    Combell heeft een interessant artikel geschreven over [hoe je CNAME records bij combell kan beheren](https://www.combell.com/nl/help/kb/wat-is-een-cname-record-hoe-kan-ik-een-cname-record-aanmaken-wijzigen/){:target="_blank"}.
