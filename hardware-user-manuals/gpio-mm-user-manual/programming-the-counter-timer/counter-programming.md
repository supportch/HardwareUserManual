# Counter Programming

Before programming any individual counter, the 9513 Master Mode Register must be programmed. Programming an individual counter requires several steps. First, the Counter Mode Register must be set to indicate the desired operating characteristics of the counter, such as gating level and type, count direction and type, and output type. 

After the Counter Mode Register is programmed, load the appropriate data into the Load and/or Hold register\(s\). The Load register is used to set the divide-by-n and initial count values. The Hold register may also be required for certain counter modes, such as variable-duty-cycle square wave functions. 

You may optionally want to set the initial output level. 

If you are using counters 1 or 2 in alarm mode, the alarm register must also be programmed. 

Next, load the initial count into the Count register using the Load command. 

Finally, "arm", or enable, the counter using the Arm command. To read a counter, issue a Save command. 

This stores the counter’s current contents in the Hold register. Then, read the Hold register. 

A counter can be armed or disarmed, and its current contents can be saved, at any time under software control through these commands. 

The information below summarizes the procedure for programming a counter: 

To set up counter operation: 

1. Program the Master Mode Register. 
2. Program the Counter Mode Register.
3. Load initial data into the Load Register.
4. \(Optional\) Load initial data into the Hold Register.
5. Issue a Load and Arm command for the counter.

To read counter contents:  

1.  Issue a Save or Disarm and Save command.  
2. Read the Hold Register. 

