# smart-stick-project
Smart Cane for Visually Impaired

Hey! Welcome to my smart stick project. I built this to help visually impaired people navigate safely by detecting obstacles using sound and light. It's like a bat, but a stick! 

Note: Some features might be changed in different commits as I experiment with the code.

What effectively does it do?
This stick uses an ultrasonic sensor (like "sonar") to measure distance. Then, it uses a buzzer to beep at you. The closer you get to an object, the faster it beeps! It also has some smart features to stop it from being annoying.

Cool Features
* Alert Zones:
    * Warning Zone (100cm): Slow beeps. "Hey, watch out."
    * Caution Zone (50cm): Medium beeps. "Okay, getting closer..."
    * DANGER ZONE (20cm): Fast beeps! "STOP! or you'll crash!" 
* Stair Detection: If the ground suddenly disappears (like a drop-off), it makes a frantic high-pitched beep so you don't fall down the stairs.
* Wall Following Mode: If you're just walking next to a wall, the stick is smart enough to know that and won't annoy you with constant beeping.
* Sleep Mode: If you don't use the stick for 30 seconds, it goes to sleep to save battery. Just move it or wave your hand in front of it to wake it up!
* Auto-Calibration: When you first turn it on, it spends 10 seconds looking around to set the perfect sensitivity for where you are.

How the Beeps Work (The "Language")
We used a passive buzzer so we can make different sounds:
* Low Tone (1000Hz): Something is far away.
* Medium Tone (1500Hz): Something is kinda close.
* High Tone (2000Hz): Super close! Danger!
* Super High Tone (3000Hz): STAIRS! Watch your step!

Parts I Used 
* Arduino 
* HC-SR04 Ultrasonic Sensor
* Passive Buzzer
* LED
* Battery & Switch
* Jumper Wires

How to Run It
1.  Open arduino_code_enhanced in the Arduino IDE.
2.  Plug in your Arduino.
3.  Upload the code!
4.  Important: Keep the stick still for the first 10 seconds so it can calibrate properly.
