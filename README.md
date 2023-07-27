# Robot_Circuit
### Task 3 of the Electric Engineering path

* Design and program distance sensor circuit
* Design and program an electric circuit of digital type

## Ultrasonic Sensor
Ultrasonic sensor HC-SR04 is used to measure the distance to an object using ultrasonic waves.

The ultrasonic sensor includes four  pins, VCC pin which needs to be connected to VCC(5V), GND which needs to be connected to the ground, TRIG pin which receives the control signal (pulse) from the Arduino, and the ECHO pin which sends a signal (pulse) to the Arduino and the Arduino measures the duration of pulse to calculate the distance.


### Applications of Ultrasonic
  * Anti-Collision Detection
  * Presence Detection
  * Monitor how close the car comes to a wall or other vehicles

    
### Requirements
* Arduino Uno
* Ultrasonic Sensor (HC-SR04)
* Mini BreadBoard
* 1 KOhm Resistor
* Jumpers
* LED
  
![Ultrasonic Sensor](https://github.com/iidabawaj/Robot_Circuit/assets/139181626/de79a9ea-5a46-4ef5-9940-d739bb379c0a)


### How to get the distance
  * Generate a 10-microsecond pulse on TRIG pin
  * Measure the pulse duration in ECHO pin, and then calculate the distance between the sensor and the object

***

## Light Dependent Resistor (LDR)
LDRs are light-dependent resistors, whose resistance decreases when light falls on them and increases in darkness. 

When a light-dependent resistor is kept dark, it has very high resistance. It can be as high as 4.5 Ω. If the device can absorb light, its resistance is dramatically reduced. The current increases when a constant voltage is applied and the light intensity increases.


### Features
* Wide spectral response
* Wide ambient temperature range
* Low cost


### Digital Applications of LDR
  * Night light control
  * Street light control
  * Automatic Headlight Dimmer


### Requirement
  * Arduino Uno
  * Breadboard
  * Photoresistor
  * 2 220 Ohm resistor
  * LED
  * Jumpers
    
![LDR ON](https://github.com/iidabawaj/Robot_Circuit/assets/139181626/7b958a97-ea13-4ea4-9fbf-01b23648057b)

![LDR OFF](https://github.com/iidabawaj/Robot_Circuit/assets/139181626/b9f52b8b-8be8-4569-8fd8-9f9a41eac999)

LDR connected to analog pin A0. In series with 10K resistor another end of the resistor will go to GND. LED connected from digital pin 2 to ground through a 220ohm resistor.

### code
Using analogRead(LDRInput), we read the value of the LDR. In the for loop, there is an if statement that will turn the LED on if it's dark (High resistance), or turn the LED off if there is light( low resistance).


  
  
  
