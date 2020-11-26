# Interrupt Source

**Base+0Ch \(Read/Write\)**

![](../../../.gitbook/assets/24%20%286%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">IRQA</td>
      <td style="text-align:left">
        <p>Select the IRQA interrupt source</p>
        <p>00h = Counter/timer 1 output
          <br />01h = Counter/timer 2 output 02h = Counter/timer 3 output 03h = Counter/timer
          4 output 04h = Counter/timer 5 output 05h = Counter/timer 6 output
          <br />06h = Counter/timer 7 output
          <br />07h = Counter/timer 8 output
          <br />08h = Counter/timer 9 output
          <br />09h = Counter/timer 10 output 0Ah = dedicated interrupt input pin &#x25C4;
          (Reset value)
          <br />0Bh = DIO input 0
          <br />0Ch = 8255-1 C0
          <br />0Dh = 8255-1 C3
          <br />0Eh = 8255-2 C0
          <br />0Fh = 8255-2 C3</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">IRQB</td>
      <td style="text-align:left">Select the IRQB interrupt source, using the same values as for IRQA, above.
        The reset value for IRQB is 0Ch.</td>
    </tr>
  </tbody>
</table>

