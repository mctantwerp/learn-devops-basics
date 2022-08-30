# A record

De A record is de basis record. Deze verwijst een host (naam) naar een server (IP adres).
Je kan ook een **wildcard** record aanmaken dmv het gebruiken van een **`*`** als je die gebruikt gaat alles wat je in de plaats zet naar dat specifiek IP adres.

<div class="annotate" markdown>

| Hostname      | IP adres        |
| ------------- | --------------- |
| `www.kdg.be`  | 94.176.99.133   |
| `kdg.be`      | 94.176.99.133   |
| `www.genx.be` | 162.55.59.3     |
| `*.staging.be`  | 123.123.123.123 |

</div>

!!! info "__*__"
    __*__ is een wildcard, je kan hier dus eender wat zetten. bvb.: __test__.staging.be, __mywebsite__.staging.be,... Al deze records zullen dan allemaal naar hetzelfde IP adres gaan.

De technische notatie van deze records is als volgt:

```md
# voor kdg.be
www IN A 94.176.99.133
@ IN A 94.176.99.133

# voor genx.be
www IN A 162.55.59.3

# wildcard
* IN A 123.123.123.123
```

!!! info ""
    Je zal merken dat we voor de root, dus bvb. **kdg.be** (zonder www) een @ gebruiken.

!!! warning "LET OP"
    A records mag je enkel gebruiken om hostnames (namen) naar een __IP adres__ te verwijzen. Je mag hier geen andere hostname ingeven. Hiervoor gebruiken we [CNAME](cname-record.md) records.

!!! tip "Meer lezen?"
    Combell heeft een interessant artikel geschreven over [hoe je A records bij combell kan beheren](https://www.combell.com/nl/help/kb/wat-is-een-a-record-hoe-kan-ik-een-a-record-aanmaken-wijzigen/){:target="_blank"}.
