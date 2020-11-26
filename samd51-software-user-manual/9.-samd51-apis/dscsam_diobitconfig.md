# DSCSAM\_DIOBitConfig

This function sets the digital I/O bit direction, pull and drive configuration for the selected port bit.

```c
BYTE DSCSAM_DIOBitConfig(BYTE Port, BYTE Bit, BYTE Pull, BYTE Drive, BYTE Dir);
```

{% tabs %}
{% tab title="Input Parameters" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left"><b>Description</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Port</td>
      <td style="text-align:left">
        <p>0-1 for port A, B for Elton, Stevie &amp; Jethro</p>
        <p>0-2 for port A, B, C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Bit</td>
      <td style="text-align:left">
        <p>0-7 for port A, 0-4 for port B for Elton, Stevie &amp; Jethro</p>
        <p>0-7 for port A, 0-4 for port B and 0-7 for port C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Pull</td>
      <td style="text-align:left">1 = enabled, 0 = disabled</td>
    </tr>
    <tr>
      <td style="text-align:left">Drive</td>
      <td style="text-align:left">1 = high, 0 = normal</td>
    </tr>
    <tr>
      <td style="text-align:left">Dir</td>
      <td style="text-align:left">1 = out, 0 = in</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

