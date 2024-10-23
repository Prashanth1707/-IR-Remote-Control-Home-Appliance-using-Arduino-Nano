# IR-Remote-Control-Home-Appliance-using-Arduino-Nano
This project allows you to remotely control home appliances using an IR remote and an Arduino Nano. With this setup, you can manage up to 4 devices (such as lights, fans, etc.), and the system saves the appliance states to EEPROM, ensuring they are restored after a power reset.

## Project Overview
This project utilizes an IR remote to control home appliances connected through a relay module to an Arduino Nano. The system decodes the IR signals, turning the appliances on or off based on the buttons pressed. States of appliances are stored using EEPROM so that even after a power failure, the system will restore the last known state of each appliance.

## Features
    Remote Control: Use any standard IR remote to control multiple appliances.
    Supports Up to 4 Appliances: Expandable to control additional appliances if needed.
    EEPROM Memory: Saves the state of each appliance, restoring the last state after a power cycle.
    Easy Setup: Simple connections between the Arduino Nano, IR receiver, and relay module.
## Hardware Used
    Arduino Nano: (or any other Arduino board)
    IR Receiver: (e.g., TSOP1738)
    4-channel Relay Module
    IR Remote: (any standard TV remote or similar)
    Appliances: (lights, fans, etc.)
    Jumper Wires
    Breadboard (optional for prototyping)
## Software Required
    Arduino IDE: Download from here.
    IRremote Library: Install it from the Arduino Library Manager.
    In the Arduino IDE, go to Sketch > Include Library > Manage Libraries and search for IRremote.
    
## Wiring Diagram
Here is a basic overview of the connections:

    Arduino Pin   	Component	         Description
        A0          IR Receiver	       IR Signal Pin
        2	          Relay 1	           Appliance 1 Control
        3	          Relay 2	           Appliance 2 Control
        4	          Relay 3	           Appliance 3 Control
        5	          Relay 4	           Appliance 4 Control
        5V	        Relay Module VCC	 5V Power to Relay
        GND	        Relay Module GND	 Ground 
     
## Circuit Diagram
![image](https://github.com/user-attachments/assets/ea4ffd84-a317-49d2-9160-f830d72ad3ae)


## Installation and Setup
  ### Clone this Repository:
    git clone https://github.com/your-username/IR-Remote-Control-Home-Appliance.git
  ### Open the Arduino IDE:

    Open the .ino file from this repository.
  ### Install the IRremote Library:

    In the Arduino IDE, go to Sketch > Include Library > Manage Libraries and search for IRremote. Install it.
 
## How to Use
  Setup Your Appliances:

  Connect the appliances to the relays according to the circuit diagram.
## Use the IR Remote:

  Point your IR remote at the IR receiver and press the corresponding buttons.
  The relays will switch the connected appliances on or off.
  Example button mappings:
  
  Button 1: Toggle Load 1
  Button 2: Toggle Load 2
  Button 3: Toggle Load 3
  Button 4: Toggle Load 4
## Components Required
    Arduino Nano
    IR Receiver (TSOP1738 or similar)
    4-channel Relay Module
    IR Remote
    Appliances (e.g., lights, fans)
    Jumper wires
    Breadboard (optional)
