# DSCSAM\_DIOOutputByte

This function outputs the specified data to the specified port. The data is 8 bits for ports A and 5 bits for port B.

```c
BYTE DSCSAM_DIOOutputByte(BYTE Port, BYTE Data);
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
        <p>0 = A, 1 = B for Elton, Stevie &amp; Jethro</p>
        <p>0 = A, 1 = B, 2 = C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Data</td>
      <td style="text-align:left">8 bit value to write to the Port 0 and 5 bit value for Port 1</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

