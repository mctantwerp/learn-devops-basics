# A record

De A record is de basis record. Deze verwijst een host \(naam\) naar een server \(IP adres\).  
Je kan ook een **wildcard** record aanmaken dmv het gebruiken van een **`*`** als je die gebruikt gaat alles wat je in de plaats zet naar dat specifiek IP adres.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Hostname</th>
      <th style="text-align:left">IP adres</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">www.kdg.be</td>
      <td style="text-align:left">94.176.99.133</td>
    </tr>
    <tr>
      <td style="text-align:left">kdg.be</td>
      <td style="text-align:left">94.176.99.133</td>
    </tr>
    <tr>
      <td style="text-align:left">www.genx.be</td>
      <td style="text-align:left">162.55.59.3</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>*.staging.be</p>
        <p>= test.staging.be</p>
        <p>= mywebsite.staging.be</p>
        <p>= ...staging.be</p>
      </td>
      <td style="text-align:left">123.123.123.123</td>
    </tr>
  </tbody>
</table>

De technische notatie van deze records is als volgt:

```bash
# voor kdg.be
www IN A 94.176.99.133
@ IN A 94.176.99.133

# voor genx.be
www IN A 162.55.59.3

# wildcard
* IN A 123.123.123.123
```

{% hint style="info" %}
Je zal merken dat we voor de root, dus bvb. **kdg.be** \(zonder www\) een @ gebruiken.
{% endhint %}

{% hint style="warning" %}
A records mag je enkel gebruiken om hostnames \(namen\) naar een IP adres te verwijzen. Je mag hier geen andere hostname ingeven. Hiervoor gebruiken we [CNAME](cname-record.md) records.
{% endhint %}

Combell heeft een interessant artikel geschreven over hoe je A records bij combell kan beheren.

{% embed url="https://www.combell.com/nl/help/kb/wat-is-een-a-record-hoe-kan-ik-een-a-record-aanmaken-wijzigen/" %}

