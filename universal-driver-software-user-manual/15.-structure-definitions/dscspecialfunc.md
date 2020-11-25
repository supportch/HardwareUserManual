# DSCSPECIALFUNC

Structure containing information on all special functions. 

### Structure Definition

```c
typedef struct {

    BYTE cmd;
    BOOL *Data;
    BOOL Config;

} DSCSPECIALFUNC;
```

### Structure Members

<table>
  <thead>
    <tr>
      <th style="text-align:left">Name</th>
      <th style="text-align:left">Description</th>
      <th style="text-align:left">Applicable Boards</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">cmd</td>
      <td style="text-align:left">Command provided from the user</td>
      <td style="text-align:left">Aries</td>
    </tr>
    <tr>
      <td style="text-align:left">Data</td>
      <td style="text-align:left">To read the data from the device</td>
      <td style="text-align:left">Aries</td>
    </tr>
    <tr>
      <td style="text-align:left">Config</td>
      <td style="text-align:left">
        <p>Pull Up/Down configuration value</p>
        <p>Values : 0 - 3</p>
        <p>0 - All DIO lines Pull down</p>
        <p>1 - Group 1 DIO lines pull up and</p>
        <p>Group 2 DIO lines Pull down</p>
        <p>2 - Group 1 DIO lines pull down</p>
        <p>and Group 2 DIO lines Pull up</p>
        <p>3 - All DIO lines Pull up</p>
      </td>
      <td style="text-align:left">DS-MPE-GPIO, DS-MPE-DAQ0804.</td>
    </tr>
  </tbody>
</table>

