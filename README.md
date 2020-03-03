# UltrasonicSensorTivaC

#Ultrasonic Ranging Module HC - SR04 
Interfacing of Ultrasonic sensors with TIVA-C ARM Cortex


Module operating operating operating operating Principle Principle Principle Principle
Set low the Trig and Echo port when the module initializes , firstly, transmit
at least 10us high level pulse to the Trig pin (module automatically sends eight
40K square wave), and then wait to capture the rising edge output by echo port,
at the same time, open the timer to start timing. Next, once again capture the
falling edge output by echo port, at the same time, read the time of the counter,
which is the ultrasonic running time in the air. According to the formular: test
distance = (high level time * ultrasonic spreading velocity in air) / 2, you can
calculate the distance to the obstacle.


Interfacing of two ultrasonic sensors (graduation project sub-project)
Using of 
timer0 for delay using Interrupt
timer3 for ultrasonic sensor 1 as trigger      
timer2 for ultrasonic sensor 2 as trigger

Pins used for ultrasonic sensor1 using timer3 as counter
PA3 (Trigger)  -   PB2 (Echo)

Pins used for ultrasonic sensor1 using timer2 as counter
PA2 (Trigger)  -   PB0  (Echo)

