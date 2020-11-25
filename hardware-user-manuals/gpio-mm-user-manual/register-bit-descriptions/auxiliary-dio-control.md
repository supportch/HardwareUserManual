# Auxiliary DIO Control

**Base+0Eh \(Write\)**

![](../../../.gitbook/assets/28%20%283%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">AUXnOUT</td>
      <td style="text-align:left">Auxiliary DIO line. Write the low-level or high-level value to the AUXnOUT
        bit to set the respective auxiliary DIO line level. The level applies even
        if the line direction, AUXnDIR, is set to input mode. The value will be
        applied when the line direction is set to output mode. 0 = low level 1
        = high level</td>
    </tr>
    <tr>
      <td style="text-align:left">AUXnDIR</td>
      <td style="text-align:left">
        <p>Auxiliary line I/O direction and state. Write the following values to
          the AUXnDIR bit to set the I/O direction (output/input) for the respective
          auxiliary DIO line.</p>
        <p>0 = output mode 1 = input mode</p>
      </td>
    </tr>
  </tbody>
</table>

          

          

