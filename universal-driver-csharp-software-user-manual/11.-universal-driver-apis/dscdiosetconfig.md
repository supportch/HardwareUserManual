# dscDIOSetConfig\(\)

```c
byte dscDIOSetConfig(short board, ref byte config);
```

Sets the DIO port configuration for future DIO operations.

Note: See board user manual or 82C55 datasheet \(if applicable\) for config\_byte details.

{% tabs %}
{% tab title="Input Parameters" %}
<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Name</b>
      </th>
      <th style="text-align:left"><b>Description</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">board</td>
      <td style="text-align:left">The handle of the board to operate on</td>
    </tr>
    <tr>
      <td style="text-align:left">config</td>
      <td style="text-align:left">
        <p>The value(s) used to configure the digital I/O ports. See each board&apos;s
          user manual for information on the number and definition of the configuration
          bytes.
          <br />0x0- Port A&amp;B input</p>
        <p>0x1-Port A output, B input</p>
        <p>0x2-Port A input, B output</p>
        <p>0x0- Port A&amp;B output</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

