# Nurture Nest – Interactive Plant Care System

Nurture Nest is an interactive plant-care system that combines environmental sensing, visual feedback, and automated watering to create an engaging and responsive plant companion. The system monitors soil moisture, water level, temperature, and humidity, and responds through LED expressions, touch interaction, and pump control.

<img width="368" height="375" alt="Screenshot 2026-01-21 at 5 38 42 PM" src="https://github.com/user-attachments/assets/c71c8bc4-2f12-42da-aa59-0c5e79eae268" />

## Overview
This project integrates multiple sensors and actuators on an Arduino platform to create a responsive embedded system that emphasizes human-centered interaction. It combines functional plant care with expressive visual feedback to encourage user engagement and awareness of environmental conditions. In addition to maintaining plant health through automated watering, the system uses an LED matrix to display expressive states based on sensor data and user interaction. A capacitive touch sensor enables direct interaction, triggering visual responses and reinforcing a user-centric, emotionally expressive design.  
The design is divided into three main layers: an upper layer that holds the plant
and growing medium, a middle layer that houses the electronics and wiring, and a
lower layer that serves as the water reservoir for automated irrigation.

<img width="193" height="297" alt="Screenshot 2026-01-21 at 5 27 06 PM" src="https://github.com/user-attachments/assets/66e66a50-9620-4339-8799-afa477303bd8" /><img width="449" height="191" alt="Screenshot 2026-01-21 at 5 27 17 PM" src="https://github.com/user-attachments/assets/9d689f43-c2eb-4615-9811-eb6f55e3de03" />


## System Features
- Soil moisture sensing with automated pump control
- Water level monitoring
- Temperature and humidity sensing using a DHT11 sensor
- Capacitive touch input for user interaction
- 8×8 NeoPixel LED matrix for expressive visual feedback
- Relay-controlled water pump

## Visual Feedback Logic
The LED matrix displays different expressions based on system state:
- **Happy**: Adequate water level and normal temperature
- **Sad (Blue/Yellow)**: Low water level or unfavorable temperature
- **Angry**: Low water level combined with high temperature
- **Affection/Love**: Triggered through repeated touch interaction
  
<img width="657" height="144" alt="Screenshot 2026-01-21 at 5 36 37 PM" src="https://github.com/user-attachments/assets/e17e5ba7-b529-4ea3-a61c-e2db084093c8" />

## How It Works
Sensor data is continuously read within the main loop. Soil moisture values are compared against a defined threshold to activate or deactivate the water pump via a relay. Environmental conditions and touch input determine which bitmap expression is displayed on the LED matrix. All actions run in real time to maintain responsive interaction.

## Hardware Components
- Arduino microcontroller
- Capacitive touch sensor
- Soil moisture sensor
- Water level sensor
- DHT11 temperature and humidity sensor
- NeoPixel 8×8 LED matrix
- Relay module and water pump

## How to Run
1. Install the required Arduino libraries: Adafruit GFX, Adafruit NeoMatrix, Adafruit NeoPixel, CapacitiveSensor, DHT Sensor Library
2. Connect all sensors and components according to the circuit diagram.
3. Upload the Arduino sketch to the board using the Arduino IDE.
4. Power the system and observe automatic responses and visual feedback.

## Circuit Design
The circuit design supports real-time sensing, visual feedback, and automated watering within a compact embedded system.

<img width="497" height="233" alt="Screenshot 2026-01-21 at 5 26 52 PM" src="https://github.com/user-attachments/assets/1816dd93-2c28-4446-bc75-941d688f9860" />

