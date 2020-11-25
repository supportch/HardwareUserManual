# EEPROM Control

**Base+0Ah \(Write\)**

![](../../../.gitbook/assets/21%20%286%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">EE_RW</td>
      <td style="text-align:left">
        <p>EEPROM data transfer direction. Read or write the EEPROM at the EEPROM
          address in the Address Register (Base+09h).</p>
        <p>0 = Write</p>
        <p>1 = Read</p>
        <p></p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">EE_EN</td>
      <td style="text-align:left">
        <p>EEPROM enable.</p>
        <p>Set bit to 1 to initiate an EEPROM byte transfer in the direction indicated
          by the EE_RW bit.</p>
      </td>
    </tr>
  </tbody>
</table>

 

