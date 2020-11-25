# DSCSAM\_LTEControl

This function controls the LTE modem specific to Jetson carrier.

```c
BYTE DSCSAM_LTEControl(BYTE Value);
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
      <td style="text-align:left">Value</td>
      <td style="text-align:left">
        <p>1 = enable,</p>
        <p>0 = disable</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

