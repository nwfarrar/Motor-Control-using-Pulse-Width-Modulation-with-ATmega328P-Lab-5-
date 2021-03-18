# Motor-Control-using-Pulse-Width-Modulation-with-ATmega328P-Lab-5-
In this lab you will use the analog input developed in Lab 4 as a control signal for a permanent magnet DC motor. Based on the five stages of potentiometer reading outlined in Lab 4, the motor speed is to be controlled in five discrete steps: forward and backward slow, forward and backward fast, and stopped. You will still use LEDs to indicate the speed and direction settings of the motor.

Part 1 (circuit): Parts needed: Same as Lab 4 plus:
Small permanent magnet DC motor (1)
SN754410NE H-Bridge chip (1)
Keep the circuit from Lab 4 and add a permanent magnet DC motor and SN754410NE H-bridge chip as the power circuit so that you can drive the motor forward and backward at different speeds. Schematics of the H-bridge are shown in Figure 1, and a photo of an example circuit is shown in Figure 2.

Part 3 (code): Program your microcontroller such that the five ranges of the potentiometer reading used in Lab 4 are now used to create the following motor control settings:
- There will be five motor speed settings: stopped, forward slow, backward slow,
forward fast, and backward fast (where “slow” is 25% duty cycle and “fast” is
75% duty cycle).
- The motor speed settings will be determined based on the position of the
potentiometer. Divide the output voltage range of the potentiometer into five subranges of approximately 1 volt each. Motor speed is to be set as:
o The lowest voltage range corresponds to fast backward motor speed. o The second voltage range corresponds to slow backward motor speed. o The middle voltage range corresponds to a stopped motor.
o The fourth voltage range corresponds to slow forward motor speed.
o The highest voltage range corresponds to fast forward motor speed.
- The LEDs must match the motor speeds as done in Lab 4: o Center LED is on when the motor is stopped
o An outer LED is on when motor is moving fast (one for forward and one
for backward)
o An inner LEDs is on when the motor is moving slowly (one for forward
and one for backward)
Note that in practice one could control the motor in discrete speed increments as is done in this lab or as a continuously-varying speed according to the potentiometer setting.
