# 5.A2 CANMESSAGE

CAN Message information strcuture.

### Structure Definition <a id="structure-definition"></a>

```c
typedef struct _CANMESSAGE{

unsigned int Can_ch;
unsigned int Rtr;
unsigned int Msg_type;
unsigned int Tb_Type; 
unsigned int Msg_ID;
unsigned int Msg_len;
unsigned char Data[68];

}CANMESSAGE
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
      <td style="text-align:left">CAN port numbers 0-3</td>
    </tr>
    <tr>
      <td style="text-align:left">Msg_type</td>
      <td style="text-align:left">
        <p>0 : Standard</p>
        <p>1 : Extended</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Tb_Type</td>
      <td style="text-align:left">
        <p>Transmit buffer type(Hex)</p>
        <p>[0 - PTB,</p>
        <p>1 - STB]</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Msg_ID</td>
      <td style="text-align:left">Hexadecimel value</td>
    </tr>
    <tr>
      <td style="text-align:left">Msg_len</td>
      <td style="text-align:left">length of the frames</td>
    </tr>
    <tr>
      <td style="text-align:left">Rtr</td>
      <td style="text-align:left">
        <p>0 : Disable</p>
        <p>1 : Enable</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Data</td>
      <td style="text-align:left">Holds the data frame of length Msg_len</td>
    </tr>
  </tbody>
</table>

