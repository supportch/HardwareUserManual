# DSCSAM\_DIOConfigAll

This function sets the digital I/O port directions, pull and drive configurations for all ports at once.

```c
BYTE DSCSAM_DIOConfigAll(BYTE *Pull, BYTE *Drive, BYTE *Dir);
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
      <td style="text-align:left">Pull</td>
      <td style="text-align:left">
        <p>Address of BYTE array of 2 pull configuration values for ports A, B for
          Elton, Stevie &amp; Jethro</p>
        <p>Address of BYTE array of 3 pull configuration values for ports A, B and
          C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Drive</td>
      <td style="text-align:left">
        <p>Address of BYTE array of 2 drive configuration values for ports A, B for
          Elton, Stevie &amp; Jethro</p>
        <p>Address of BYTE array of 3 drive configuration values for ports A, B and
          C for Ziggy</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Dir</td>
      <td style="text-align:left">
        <p>Address of BYTE array of 2 direction configuration values for ports A,
          B for Elton, Stevie &amp; Jethro</p>
        <p>Address of BYTE array of 3 direction configuration values for ports A,
          B and C for Ziggy</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

