# DSCSAM\_BoardType

This function read the board type from SAM.

```c
BYTE DSCSAM_BoardType(BYTE * Board_type);
```

{% tabs %}
{% tab title="Input Parameters" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Name</b>
      </th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Board_type</td>
      <td style="text-align:left">
        <p>pointer to receive board type.</p>
        <p>(0 - Ziggy,</p>
        <p>1 - To be determined,</p>
        <p>3 - Stevie,</p>
        <p>5 - Elton,</p>
        <p>7 - Jethro)</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

