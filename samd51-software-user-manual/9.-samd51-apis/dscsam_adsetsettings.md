# DSCSAM\_ADSetSettings

This function configures the A/D channel\(current,low & high\), scan settings, A/D Trigger, A/D reference, oversampling/averaging, A/D single ended and A/D differential ended.

```c
BYTE DSCSAM_ADSetSettings(DSCSAM_ADSETTINGS* settings);
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
      <td style="text-align:left">Sedi</td>
      <td style="text-align:left">0-1; 0 = single-ended, 1 = differential (Elton, Stevie &amp; Jethro)</td>
    </tr>
    <tr>
      <td style="text-align:left">Lowch</td>
      <td style="text-align:left">low channel, 0-5(Single ended) [Elton, Stevie, Jethro &amp; Ziggy]</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">low channel, 0-2(Differential ended) [Elton, Stevie &amp; Jethro]</td>
    </tr>
    <tr>
      <td style="text-align:left">Highch</td>
      <td style="text-align:left">high channel, 0-5(Single ended) [Elton, Stevie, Jethro &amp; Ziggy]</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">high channel, 0-2(Differential ended) [Elton, Stevie &amp; Jethro]</td>
    </tr>
    <tr>
      <td style="text-align:left">Currentch</td>
      <td style="text-align:left">channel number 0-5 for current conversion</td>
    </tr>
    <tr>
      <td style="text-align:left">ScanEnable</td>
      <td style="text-align:left">
        <p>0 = sample,</p>
        <p>1 = scan</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adtrig</td>
      <td style="text-align:left">
        <p>00 = software initiated A/D conversion</p>
        <p>01 = external GPIO pin is used to trigger A/D conversion</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adsel</td>
      <td style="text-align:left">
        <p>0 = A/D circuit 0,</p>
        <p>1 = A/D circuit 1</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adref</td>
      <td style="text-align:left">
        <p>00 = external reference (set to 3.3V)</p>
        <p>01 = internal bandgap reference</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adtag</td>
      <td style="text-align:left">
        <p>0 = upper 4 bits of 16-bit value = 0000</p>
        <p>1 = upper 4 bits of 16-bit value contain A/D channel number</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adchset</td>
      <td style="text-align:left">
        <p>ADCHSET = 0: Selects channel number for current conversion</p>
        <p>ADCHSET = 1: Selects high/low channel number</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adres</td>
      <td style="text-align:left">
        <p>00 = No oversampling, A/D resolution = 12 bits</p>
        <p>01 = A/D resolution = 14 bits</p>
        <p>10 = A/D resolution = 15 bits</p>
        <p>11 = A/D resolution = 16 bits</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Adsamples</td>
      <td style="text-align:left">
        <p>Number of samples to be accumulated</p>
        <p>1, 2, 4, 8, 16, 32, 64, 128, 256, 512 and 1024</p>
      </td>
    </tr>
  </tbody>
</table>
{% endtab %}
{% endtabs %}

| Return Value |
| :--- |
| Error code or 0. |

