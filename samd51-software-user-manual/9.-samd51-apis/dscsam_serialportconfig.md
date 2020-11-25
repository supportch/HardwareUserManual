# DSCSAM\_SerialPortConfig

This function configures the serial port mode.

```c
BYTE DSCSAM_SerialPortConfig(BYTE Mode, BYTE Port);
```

{% tabs %}
{% tab title=" Input Parameters" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Applicable Boards</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Mode</td>
      <td style="text-align:left">
        <p>0 &#x2013; RS232,</p>
        <p>1 &#x2013; RS422,</p>
        <p>2 &#x2013; RS485</p>
      </td>
      <td style="text-align:left">Elton, Stevie and Jethro</td>
    </tr>
    <tr>
      <td style="text-align:left">Port</td>
      <td style="text-align:left">0 &#x2013; Serial Port Pair 1 and 2</td>
      <td style="text-align:left">Elton, Stevie and Jethro</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">1 &#x2013; Serial Port Pair 3 and 4</td>
      <td style="text-align:left">Elton and Stevie</td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

