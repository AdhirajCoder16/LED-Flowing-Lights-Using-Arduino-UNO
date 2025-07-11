 LED Flowing Lights Using Arduino UNO
This project demonstrates how to create a flowing light effect using 8 LEDs controlled by an Arduino UNO. This is a continuation from the basic "blinking LED" project and introduces the use of for loops and arrays to control multiple LEDs in a visually appealing pattern.

📦Components Required
1 × Arduino UNO

1 × USB Cable

8 × LEDs

8 × 220Ω Resistors

1 × Breadboard

Several Jumper Wires

 Principle
The LEDs are controlled using a simple loop logic where each LED is turned on and off in a sequence, creating a flowing light effect. This simulates a water-like motion from right to left and left to right repeatedly.

The core of this effect is implemented using the for loop in Arduino, which allows us to iterate over arrays and pin numbers efficiently.

 Key Concept: for Loop in Arduino

for (initialization; condition; increment) {
   // Code to execute repeatedly
}
Initialization: Happens once at the beginning.

Condition: Checked before each loop iteration.

Increment: Runs at the end of every loop cycle.

Example:


for (int i = 0; i < 8; i++) {
  digitalWrite(ledPins[i], HIGH);
  delay(100);
  digitalWrite(ledPins[i], LOW);
}
Procedure
Step 1: Build the Circuit
Connect all 8 LEDs to digital pins on the Arduino through 220Ω resistors.

Use the breadboard and jumper wires to organize and connect the LEDs.

Step 2: Write and Upload the Code
Open the Arduino IDE.

Paste the provided code (see below).

Connect the Arduino UNO via USB.

Select the correct board and COM port.

Upload the sketch to the Arduino.

Step 3: Observe the Effect
LEDs will light up one-by-one from right to left and then back from left to right.

This sequence repeats continuously, creating a flowing water-like animation.

