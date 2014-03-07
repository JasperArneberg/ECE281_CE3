ECE281_CE3
==========
######ECE 281 Computer Exercise 3: Advanced Elevator Controller

C3C Jasper Arneberg  
M6A ECE 281  
Dr. Neebel  

## Moore Machine

#### Waveform Output
Here is the screenshot of the waveform output of the Moore Machine.
![alt text](https://github.com/JasperArneberg/ECE281_CE3/blob/master/moore_waveform.png?raw=true "Moore Machine waveform screenshot")

#### Explanation of Testbench Results
The Moore Machine was verified to behave correctly by inspection. Just as planned, the floor advances by one every two clock cycles until it reaches the top. Then, it descends one floor every clock cycle until it meets the bottom.

## Mealy Machine

#### Waveform Output
Here is the screenshot of the waveform output of the Mealy Machine.
![alt text](https://github.com/JasperArneberg/ECE281_CE3/blob/master/mealy_waveform.png?raw=true "Mealy Machine waveform screenshot")

#### Explanation of Testbench Results
The Mealy Machine was verified to behave correctly by inspection as well. The same testbench stimuli were used for this one as the Moore Machine.  The nextfloor output is the only visible difference between the two. The nextfloor output accurately predicts what the next floor will be as long as the inputs don't change at the next clock cycle. Simple inspection shows that this works correctly.

## Answers to Questions
The clock frequency is 100 MHz when the clock period is equal to 10 ns. To obtain a frequency of 50 MHz, a clock period of 20 ns should be used.

The reset in both designs is synchronous because it is reliant on the clock cycle.

When stop='1', we want to stay on the same floor regardless. Otherwise, we want to go up a floor when updown='1' and down a floor when updown = '0'.

The Mealy Machine next-state process code is exactly the same as it was for the Moore Machine.

## Documentation
None.
