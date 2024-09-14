#Water Level Alarm

I created this alarm to warn me when my christmas tree ran out of water. It can also be used to alert the user if a plant runs out of water.

The functioning of this alarm is reliant on the water acting as a resistor in a voltage divider.
The output of the voltage divider is connected to the non-inverting input of an LM358 op-amp configured as a comparator. The inverting input is connected to the middle pin of a potentionmeter which sets the threshold voltage.

Normally, the presence of water pulls the output of the voltage divider towards ground. When water is absent, the output of the voltage divider is pulled up, in turn pulling the output of the LM358 to the positive supply rail. This powers the 555 timer, which pulses an LED and beeper via NPN transistors to create an alert sound.
