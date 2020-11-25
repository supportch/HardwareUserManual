# 5.A1 CANCONFIG

CAN configuration structure.

### Structure Definition <a id="structure-definition"></a>

```c
typedef struct _CANCONFIG{

unsigned int Can_ch;
unsigned int BaudRate;
unsigned int Rtr;
	
}CANCONFIG;
```

### Structure Members <a id="structure-members"></a>

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Can_ch</td>
      <td style="text-align:left">CAN port number 0-3.</td>
    </tr>
    <tr>
      <td style="text-align:left">BaudRate</td>
      <td style="text-align:left">
        <p>Constant indicating the baud rate.</p>
        <p>[0 - B1000 &#x4E00; 1000kbit/s,</p>
        <p>1 - B800 &#x4E00; 800kbit/s,</p>
        <p>2 - B500 &#x4E00; 500kbit/s,</p>
        <p>3 - B250 &#x4E00; 250kbit/s,</p>
        <p>4 - B125 &#x4E00; 25kbits/s,</p>
        <p>5 - B100 &#x4E00; 100kbit/s,</p>
        <p>6 - B50 &#x4E00; 50kbit/s,</p>
        <p>7 - B20 &#x4E00; 20kbit/s,</p>
        <p>8 - B10 &#x4E00; 10kbit/s ]</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Rtr</td>
      <td style="text-align:left">
        <p>RTR.</p>
        <p>[0 - Disable,</p>
        <p>1 - Enable]</p>
      </td>
    </tr>
  </tbody>
</table>

