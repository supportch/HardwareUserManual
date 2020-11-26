# 9513 Interrupt Enable/Disable

**Base+06h/Base+07h \(Write\)**

![](../../../.gitbook/assets/17%20%283%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"></th>
      <th style="text-align:left"></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">INTE</td>
      <td style="text-align:left">
        <p>Interrupt enable. Write to this bit to enable or disable counter/timer
          interrupts. (Register Base+07h is a shadow of register Base+06h.)</p>
        <p>0 = disable interrupts</p>
        <p>1 = enable interrupts</p>
        <p>If IRQA and IRQB are both counter/timer interrupts, both interrupts are
          enabled or disabled by writing to this register. IRQA and IRQB are considered
          counter/timer interrupts if the interrupt source is the counter/timer output
          1-10, dedicated interrupt input, or DIO input 0. This is equivalent to
          the IRQAEN/IRQBEN and IRQADIS/IRQBDIS bits of the Interrupt Control/Status
          Register (Base+0Dh).</p>
      </td>
    </tr>
  </tbody>
</table>

 

