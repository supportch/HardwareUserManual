# 4.A3 can\_device\_stats

CAN device statistics structure

### Structure Definition <a id="structure-definition"></a>

```c
typedef struct can_device_stats {

unsigned int txerr;   
unsigned int rxerr;  
unsigned int txpackets; 
unsigned int rxpackets; 
unsigned int rx_over_errors; 
unsigned int error_active; 
unsigned int stat_change; 
unsigned int bit_error;
unsigned int stuff_error;
unsigned int form_error; 
unsigned int bus_error;       
unsigned int bus_error_enable;
unsigned int error_warning;   
unsigned int error_passive;   
unsigned int bus_off;         
unsigned int arbitration_lost;
unsigned int arbitration_lost_enable;
	
}can_device_stats;
```

### Structure Members <a id="structure-members"></a>

| Name | Description |
| :--- | :--- |
| txerr | Transmit errors |
| rxerr | Receive errors |
| txpackets | Tx transmitted count |
| rxpackets | Rx transmitted count |
| rx\_over\_errors | Rx over error count |
| error\_active | Error active enable |
| stat\_change | stat changed from passive to active ,vice versa |
| bit\_error | bit error |
| stuff\_error | stuff error |
| form\_error | Form error |
| bus\_error | Bus errors |
| bus\_error\_enable | bit error enable |
| error\_warning | Changes to error warning state |
| error\_passive | Changes to error passive state |
| bus\_off | Changes to bus off state |
| arbitration\_lost | Arbitration lost errors |
| arbitration\_lost\_enable | arbitration lost error enable |

