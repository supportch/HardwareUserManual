# 8255 Control and Status \(Basic Mode Definition – MSFLAG=1\)

**DIO Base+03h \(8255-1\), DIO Base+07h \(8255-2\) - \(Read/Write\)**

![](../../../.gitbook/assets/32%20%283%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">PCLDIR</td>
      <td style="text-align:left">Port C (lower) direction. Sets the direction of the port C I/O signals
        0-3. 0 = output 1 = input &#x25C4; (Reset value)</td>
    </tr>
    <tr>
      <td style="text-align:left">PBDIR</td>
      <td style="text-align:left">Port B direction. Sets the direction of the port B I/O signals. 0 = output
        1 = input &#x25C4; (Reset value)</td>
    </tr>
    <tr>
      <td style="text-align:left">MSELB</td>
      <td style="text-align:left">
        <p>Group B mode selection. Sets the mode of operation for the group B signals.
          0 = mode 0 &#x25C4; (Reset value)</p>
        <p>1 = mode 1</p>
        <p>NOTE: 1. Only mode 0 is currently implemented. 2. All output registers
          are reset when the mode is changed.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">PCUDIR</td>
      <td style="text-align:left">Port C (upper) direction. Sets the direction of the port C I/O signals
        4-7. 0 = output 1 = input &#x25C4; (Reset value)</td>
    </tr>
    <tr>
      <td style="text-align:left">PADIR</td>
      <td style="text-align:left">Port A direction Sets the direction of the port A I/O signals. 0 = output
        1 = input &#x25C4; (Reset value)</td>
    </tr>
    <tr>
      <td style="text-align:left">MSELA</td>
      <td style="text-align:left">
        <p>Group A mode selection. Sets the mode of operation for the group B signals.
          00h = mode 0 &#x25C4; (Reset value)</p>
        <p>01h = mode 1</p>
        <p>1xh = mode NOTE: 1. Only mode 0 is currently implemented. 2. All output
          registers are reset when the mode is changed.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">MSFLAG</td>
      <td style="text-align:left">
        <p>Mode set flag. Selects the port configuration mode. 0 = Bit set/reset
          control register mode When MSFLAG is reset, this register is used to set/reset
          individual Port C bits.</p>
        <p>1 = Basic mode definition control register mode &#x25C4; (Reset value)</p>
        <p>When MSFLAG is set, this register is used for direction and mode selection.</p>
        <p>NOTE: When the control word is read, the value of MSFLAG is always 1,
          implying basic control word information is being read.</p>
      </td>
    </tr>
  </tbody>
</table>

        

