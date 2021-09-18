# NS record

De NS record is de nameserver record waar we het al uitgebreid over hebben gehad bij "[Hoe werkt DNS](../hoe-werkt-dns/)". Dit is dus de server die de **baas** is over je domeinnaam en zal bepalen welke andere DNS records hier op staan.

Doorgaans worden er altijd meer dan 2 nameservers ingesteld want je wil niet dat als er 1 server down is dat je domeinnaam niet meer werkt! Nameservers worden altijd met bijhorend IP adres ingesteld.

bvb.: voor kdg.be

| Host | IP adres |
| :--- | :--- |
| ns1.belnet.be | 193.190.198.14 |
| ns2.belnet.be | 193.190.182.40 |

bvb.: voor combell.be

| Host | IP adres |
| :--- | :--- |
| ns1.combell.net | 193.111.95.21 |
| ns2.combell.net | 62.213.205.134 |
| ns3.combell.net | 83.217.73.172 |
| ns4.combell.net | 86.39.202.67 |

De technische notatie van deze records is alsvolgt:

```bash
# voor kdg.be
@ IN NS ns1.belnet.be.
@ IN NS ns2.belnet.be.

# voor combell
@ IN NS ns1.combell.net.
@ IN NS ns2.combell.net.
@ IN NS ns3.combell.net.
@ IN NS ns4.combell.net.
```

{% hint style="info" %}
Als je DNS technisch moet noteren dan moet je als je hostnames gebruikt daar een `.` ****achterzetten. Als je dat niet doet zal DNS er altijd de eigen domeinnaam terug achter zeggen. Dus dan wordt het bvb **ns1.belnet.be.kdg.be**. Wat niet klopt natuurlijk.
{% endhint %}

Combell heeft een interessant artikel geschreven over hoe je nameservers bij combell kan beheren.

{% embed url="https://www.combell.com/nl/help/kb/naar-welke-nameservers-verwijst-mijn-domeinnaam/\#setting" %}



