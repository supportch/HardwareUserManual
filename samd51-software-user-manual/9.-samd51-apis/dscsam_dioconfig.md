# DSCSAM\_DIOConfig

This function sets the digital I/O port direction, pull and drive configuration for the selected port.

```c
BYTE DSCSAM_DIOConfig(BYTE Port, BYTE Pull, BYTE Drive, BYTE Dir);
```

{% tabs %}
{% tab title=" Input Parameters" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Port</td>
      <td style="text-align:left">
        <p>0-1 for port A, B for Elton, Stevie &amp; Jethro</p>
        <p>0, 1 and 2 for port A, B and C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Pull</td>
      <td style="text-align:left">1 = pull up, 0 = pull down</td>
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

