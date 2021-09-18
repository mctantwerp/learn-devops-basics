# A record

De A record is de basis record. Deze verwijst een host \(naam\) naar een server \(IP adres\)

bvb.:

| Hostname | IP adres |
| :--- | :--- |
| www.kdg.be | 94.176.99.133 |
| kdg.be | 94.176.99.133 |
| www.genx.be | 162.55.59.3 |

De technische notatie van deze records is als volgt:

```bash
# voor kdg.be
www IN A 94.176.99.133
@ IN A 94.176.99.133

# voor genx.be
www IN A 162.55.59.3
```

{% hint style="info" %}
Je zal merken dat we voor de root, dus bvb. **kdg.be** \(zonder www\) een @ gebruiken.
{% endhint %}

{% hint style="warning" %}
A records mag je enkel gebruiken om hostnames \(namen\) naar een IP adres te verwijzen. Je mag hier geen andere hostname ingeven. Hiervoor gebruiken we [CNAME](cname-record.md) records.
{% endhint %}

Combell heeft een interessant artikel geschreven over hoe je A records bij combell kan beheren.

{% embed url="https://www.combell.com/nl/help/kb/wat-is-een-a-record-hoe-kan-ik-een-a-record-aanmaken-wijzigen/" %}

