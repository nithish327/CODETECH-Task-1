Name: NITHISH S
Company: CODETECH IT SOLUTIONS
ID:CT08DS6336
Domain: Embedded Systems
Duration: August to September 2024

Overview of the LED Blinking with Arduino Project

Project Title: LED Blinking with Arduino

Objective:
     The primary goal of this project is to introduce basic embedded programming concepts and interfacing with hardware by using an Arduino board to blink an LED at a specific interval. This foundational project helps users understand how to control electronic components through code.

Materials Needed:
- Arduino board (e.g., Arduino Uno)
- LED
- Resistor (220 ohms recommended)
- Breadboard and jumper wires
- USB cable to connect the Arduino to a computer

 Project Steps:

1. Hardware Setup:
   - Connect the LED:
   - Connect the anode (longer leg) of the LED to a digital pin on the Arduino (e.g., pin 13).
   - Connect the cathode (shorter leg) of the LED to one end of the resistor.
   - Connect the other end of the resistor to the GND (ground) pin on the Arduino.
   - 
2. Software Setup:
   - Install the Arduino IDE: Download and install the Arduino Integrated Development Environment (IDE) from the official Arduino website.
   - Write the Code: Open the Arduino IDE and write the code to control the LED.

   cpp
   const int ledPin = 13;

   void setup() {
     pinMode(ledPin, OUTPUT);
   }

   void loop() {
     digitalWrite(ledPin, HIGH);
     delay(1000);
     digitalWrite(ledPin, LOW);
     delay(1000);
   }
   
    
3. Upload the Code:
   - Connect the Arduino board to the computer using the USB cable.
   - Select the correct board and port from the Tools menu in the Arduino IDE.
   - Click the upload button to transfer the code to the Arduino board.
   - 
4.Observation:
   - Once the code is uploaded, the LED should start blinking with a 1-second interval.
Explanation of Code:
- pinMode(ledPin, OUTPUT); sets the specified pin (ledPin) as an output pin.
- digitalWrite(ledPin, HIGH);* turns the LED on by setting the pin voltage to HIGH.
- delay(1000); pauses the execution of the program for 1000 milliseconds (1 second).
- digitalWrite(ledPin, LOW); turns the LED off by setting the pin voltage to LOW.
- The loop() function runs indefinitely, causing the LED to continuously blink on and off.

Learning Outcomes:
- *Basic Hardware Interfacing:* Understanding how to connect an LED to an Arduino and the importance of using resistors.
- *Embedded Programming:* Learning to write simple programs to control hardware components.
- *Timing Control:* Using the delay function to create time intervals for controlling the blink rate of the LED.

Further Exploration:
- Modify the blinking interval by changing the delay values.
- Connect and control multiple LEDs using different digital pins.
- Integrate sensors or buttons to create more complex interactions.

