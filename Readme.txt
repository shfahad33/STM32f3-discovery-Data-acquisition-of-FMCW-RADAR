This code has configration of 12 bit adc at chenal A0 with 10kSPS. And at the edge of conversion the adc sample is converted
to a string array and sent to Com Port with board rate of 115200.
A saw tooth wave form is generated With DAC 0 to drive the VCO at 110 Hz. 
STM only takes 0-3.3 volts in input only unipolar input at adc channel. 
So if you want to insert a negative cycle in the input you have to use a level shifter. 


External circuit. 

The external circuit attached in figure has a opamp with 10 gain in non inverting configration. 
And a level shifter coupled with a 10uf capacitor. 
If you don't want to apmlify the signal jut replace 12k feed back resistor with a 1.2k to act as buffer.
