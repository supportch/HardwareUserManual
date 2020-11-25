# DSCSAM\_CAMERAControl

This function controls the camera specific to Jetson carrier.

```c
BYTE DSCSAM_CAMERAControl(BYTE Value);
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
        <p>1 - 1P2 camera enable</p>
        <p>2 - 1P8 camera enable</p>
        <p>3 - 1P2 camera &amp; 1P8 camera enable</p>
        <p>4 - 2P8 camera enable</p>
        <p>5 - 1P2 camera &amp; 2P8 camera enable</p>
        <p>6 - 1P8 camera &amp; 2P8 camera enable</p>
        <p>7 - 1P2 camera,1P8 camera &amp; 2P8 camera enable</p>
        <p>0 &#x2013; All camera OFF</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

