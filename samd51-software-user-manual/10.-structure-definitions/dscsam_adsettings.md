# DSCSAM\_ADSETTINGS

Structure containing AD input parameters.‌

### Structure Definition <a id="structure-definition"></a>

```c
typedef struct {

int Sedi;	
int Lowch;	
int Highch;
int Currentch;    
int ScanEnable;	
int Adtrig;	   
int Adsel;	  
int Adref;	   
int Adtag;
int Adchset;	
int Adres;   
int Adsamples;
 
} DSCSAM_ADSETTINGS;

```

### Structure Members <a id="structure-members"></a>

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
      <td style="text-align:left">Sedi</td>
      <td style="text-align:left">0 = single-ended</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x200B;</td>
      <td style="text-align:left">1 = differential ended</td>
      <td style="text-align:left">Elton, Stevie, Jethro</td>
    </tr>
    <tr>
      <td style="text-align:left">Lowch</td>
      <td style="text-align:left">low channel, 0-5(Single ended)</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">low channel, 0-2(Differential ended)</td>
      <td style="text-align:left">Elton, Stevie, Jethro</td>
    </tr>
    <tr>
      <td style="text-align:left">Highch</td>
      <td style="text-align:left">high channel, 0-5(Single ended)</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left"></td>
      <td style="text-align:left">high channel, 0-2(Differential ended)</td>
      <td style="text-align:left">Elton, Stevie, Jethro</td>
    </tr>
    <tr>
      <td style="text-align:left">Currentch</td>
      <td style="text-align:left">channel number 0-5 for current conversion</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">ScanEnable</td>
      <td style="text-align:left">0 = sample, 1 = scan</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adtrig</td>
      <td style="text-align:left">
        <p>00 = software initiated A/D conversion</p>
        <p>01 = external GPIO pin is used to trigger A/D conversion</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adsel</td>
      <td style="text-align:left">0 = A/D circuit 0, 1 = AD circuit 1</td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adref</td>
      <td style="text-align:left">
        <p>00 = external reference (set to 3.3V )</p>
        <p>01 = internal bandgap reference</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adtag</td>
      <td style="text-align:left">
        <p>0 = upper 4 bits of 16-bit value = 0000</p>
        <p>1 = upper 4 bits of 16-bit value contain A/D channel number</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adchset</td>
      <td style="text-align:left">
        <p>ADCHSET = 0: Selects channel number for current conversion</p>
        <p>ADCHSET = 1: Selects high/low channel number</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adres</td>
      <td style="text-align:left">
        <p>0 - No oversampling, A/D resolution = 12 bits</p>
        <p>1 - A/D resolution = 14 bits</p>
        <p>2 - A/D resolution = 15 bits</p>
        <p>3 - A/D resolution = 16 bits</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
    <tr>
      <td style="text-align:left">Adsamples</td>
      <td style="text-align:left">
        <p>Number of samples to be accumulated to calculate average sample:</p>
        <p>1, 2, 4, 8, 6, 32, 64,128, 256, 512 and 1024</p>
        <p></p>
        <p>(Please refer section 45.6.2.10 in SAMD51 datasheet for more information)</p>
      </td>
      <td style="text-align:left">Elton, Stevie, Jethro, Ziggy</td>
    </tr>
  </tbody>
</table>



