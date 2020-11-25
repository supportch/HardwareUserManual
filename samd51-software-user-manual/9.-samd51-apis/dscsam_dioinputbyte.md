# DSCSAM\_DIOInputByte

This function reads in the data from the specified port and returns it in the location specified by the pointer to data.

```c
BYTE DSCSAM_DIOInputByte(BYTE Port, BYTE* Data);
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
      <td style="text-align:left">pointer to receive the data read from the port</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

