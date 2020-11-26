# DSCSAM\_DIOInputBit

This function reads in the specified bit from the specified port and returns it in the location specified by the pointer to data.

```c
BYTE DSCSAM_DIOInputBit(BYTE Port, BYTE Bit, BYTE * Value);
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
      <td style="text-align:left">Bit</td>
      <td style="text-align:left">
        <p>0-7 for port A, 0-4 for port B for Elton, Stevie &amp; Jethro</p>
        <p>0-7 for port A, 0-4 for port B and 0-7 for port C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Value</td>
      <td style="text-align:left">
        <p>pointer to receive the bit data;</p>
        <p>return data is always 0 or 1</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

[  
](https://app.gitbook.com/@diamondsystems/s/samd51-api-user-manual/9.-samd51-apis/dscsam_dioconfigall)

