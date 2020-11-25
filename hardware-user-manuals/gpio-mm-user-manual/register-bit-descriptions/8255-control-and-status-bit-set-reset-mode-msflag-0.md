# 8255 Control and Status \(Bit SET/RESET Mode – MSFLAG=0\)

**DIO Base+03h \(8255-1\), DIO Base+07h \(8255-2\) - \(Read/Write\)**

![](../../../.gitbook/assets/33%20%283%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">SET</td>
      <td style="text-align:left">Bit set/reset individual command. 0 = reset 1 = set</td>
    </tr>
    <tr>
      <td style="text-align:left">BSEL</td>
      <td style="text-align:left">Port C bit select. 0 = bit 0 1 = bit 1 2 = bit 2 3 = bit 3 4 = bit 4 5
        = bit 5 6 = bit 6 7 = bit 7</td>
    </tr>
    <tr>
      <td style="text-align:left">MSFLAG</td>
      <td style="text-align:left">
        <p>Mode set flag. Selects the port configuration mode. 0 = Bit set/reset
          control register mode When MSFLAG is reset, this register is used to set/reset
          individual Port C Bits.</p>
        <p>1 = Basic mode definition control register mode When MSFLAG is set, this
          register is used for direction and mode selection.</p>
        <p>NOTE: When the control word is read, the value of MSFLAG is always 1,
          implying basic control word information is being read.</p>
      </td>
    </tr>
  </tbody>
</table>

    

                                                           

