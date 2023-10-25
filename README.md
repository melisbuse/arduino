# arduino
FİREALARM-EXPLANATİON 
What is needed ?
Arduino Uno 
Breadboard 
YG1006 flame sensor 
1x Led 
1x Resistor
1x Buzzer 

 Components explanation
What is a flame sensor?
A flame detector is a type of sensor that can detect and respond to the presence of a flame.
What is Arduino?
Arduino is a physical programming platform which is used to develop interactive project and it has some parts like microcontroller, digital pins, analog pins, crystal oscillator etc. to make it real.
What is a buzzer?
Buzzer is a kind of voice device that converts audio model into sound signal.
what is a resistor?
A resistor is an electrical component that limits or regulates the flow of electrical current in an electronic circuit
what is BreadBoard ?
A thin plastic board used to hold electronic components (transistors, resistors, chips, etc.) that are wired together. Used to develop prototypes of electronic circuits, breadboards can be reused for future jobs.

code explanation
int led = 8; and int buzzer = 9; declare two integer variables named led and buzzer, which represent the pin numbers where an LED and a buzzer are connected to the microcontroller.

int alev_sensoru = A0; declares an integer variable named alev_sensoru, which represents the analog pin (A0) where the flame sensor is connected.

In the setup function, pinMode(led, OUTPUT); and pinMode(buzzer, OUTPUT); set the led and buzzer pins as output pins, indicating that they will be used to send electrical signals to the LED and buzzer.

The loop function continuously runs and does the following:

int alinan_deger = analogRead(alev_sensoru); reads an analog value from the flame sensor connected to the alev_sensoru pin (A0) and stores it in the variable alinan_deger.

if (alinan_deger < 750) checks if the value obtained from the flame sensor is less than 750. This condition is used to detect the presence of a flame or high temperature.

If the condition is met, it turns on the LED and buzzer by setting their output pins to HIGH using digitalWrite(led, HIGH); and digitalWrite(buzzer, HIGH);. This means the LED will light up, and the buzzer will produce a sound.

If the condition is not met (flame or high temperature is not detected), it turns off the LED and buzzer by setting their output pins to LOW using digitalWrite(led, LOW); and digitalWrite(buzzer, LOW);. This means the LED turns off, and the buzzer stops making a sound.
