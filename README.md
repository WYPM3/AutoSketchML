# AutoSketchML
AutoSketchML is an arduino system that requires a prompt - email system in order to function. The premise of this system is to train new arduino developers whose experience with the code may be primitive. 

It uses the prompt and the email address of the user in order to generate the arduino code via a trained AI Agent. Data logs such as sensor strength and battery strength is collected and stored on a PHPMyAdmin server as to allow for the AI Agent to be trained automatically. Furthermore, it uses an AI generated instruction list that is sent to the users email address in order to instruct them how to do the hardware involved in creating this program. A keyboard is required in order to type the email and prompt but a raspberry Pi with Wifi access can be used as a replacement for a desktop computer. 

The way the system can detect what pin is activated is through a hardcoded system where if a pin is activated then the database will recieve that package and process it through a Boolean hierarchy where the components given by the Super Starter Kit for the UNO R3 project are given a specific pin to occupy. If the request of the user exceeds the quantity of pins on the hub board then the AI Agent systematically includes the method for setting up a breadboard in the auto-generated instructions.

In Order to setup your PHPMyAdmin server, you must download both XAMPP or any other server hosting platform and PHPMyAdmin. local/host databases are free for any users that want to use it for home use but online comes with more data security risks so be careful.

Instructions for LCD and button setup:

Power & Contrast: 
LCD Pin 1 → GND
LCD Pin 2 → 5V
LCD Pin 3 → Middle pin of 10k potentiometer
Pot side pin → 5V 
Pot other side pin → GND
Control Pins:
LCD Pin 4 (RS) → Arduino D12
LCD Pin 5 (RW) → GND
LCD Pin 6 (E) → Arduino D11 Data Pins (4-bit mode)
LCD Pin 11 (D4) → Arduino D5
LCD Pin 12 (D5) → Arduino D4 
LCD Pin 13 (D6) → Arduino D3
LCD Pin 14 (D7) → Arduino D2
Backlight:
LCD Pin 15 (LED+) → 5V (or 220Ω resistor → 5V)
LCD Pin 16 (LED-) → GND

Up Button:
Button pin → GND (with 5V Ohmic resistor)
parallel Button pin → Arduino D8

Down Button:
Button pin → GND (with 5V Ohmic resistor)
parallel Button pin → Arduino D9











