# DSCSAM\_DIOOutputBit

This function outputs a single bit to an output port. The other bits remain at their current values.

```c
BYTE DSCSAM_DIOOutputBit(BYTE Port, BYTE Bit, BYTE Value);
```

{% tabs %}
{% tab title="Input Parameters" %}
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
        <p>Port to write bit to: 0 = A, 1 = B for Elton, Stevie &amp; Jethro</p>
        <p>Port to write bit to: 0 = A, 1 = B, 2 = C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Bit</td>
      <td style="text-align:left">
        <p>0-7 indicates the bit position in the port A and for port B the value
          should be 0-4 for Elton , Stevie &amp; Jethro</p>
        <p>0-7 indicates the bit position in the port A and for port B the value
          should be 0-4 and 0-7 for port C for Ziggy.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Value</td>
      <td style="text-align:left">0 or 1</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

