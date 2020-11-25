# DSCSAM\_InitBoard

This function initializes the SPI driver, BUSY GPIO, read the A/D, D/A calibration constants, read the board type and return to application.

```c
BYTE DSCSAM_InitBoard(BYTE * Board_type)
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
      <td style="text-align:left">Board_type</td>
      <td style="text-align:left">
        <p>pointer to receive board type</p>
        <p>(0 - Ziggy, 1 - TBD, 3 - Stevie, 5 - Elton, 7 - Jethro)</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

