# Reverse Parking System using Arduino and Ultrasonic Sensor

## Description
An Arduino-based reverse parking detection system that 
uses an HC-SR04 ultrasonic sensor to measure the distance 
between a vehicle and obstacles. The system provides 
real-time audio and visual alerts to guide drivers 
during reversing, similar to modern car parking sensors.

## Problem Statement
Reversing a vehicle without visibility of rear obstacles 
is a common cause of minor accidents in parking areas. 
This low-cost system replicates commercial parking 
sensor functionality using Arduino and readily available 
components.

## Features
- Real-time distance measurement using HC-SR04 
  ultrasonic sensor
- LED indicators showing proximity zones:
  - 🟢 Green — Safe distance
  - 🟡 Yellow — Caution zone
  - 🔴 Red — Danger, stop immediately
- Buzzer alert with increasing frequency as 
  obstacle gets closer
- Continuous monitoring with instant response

## Hardware Used
| Component | Quantity | Purpose |
|-----------|----------|---------|
| Arduino Uno | 1 | Main microcontroller |
| HC-SR04 Ultrasonic Sensor | 1 | Distance measurement |
| LED (Green, Yellow, Red) | 3 | Visual proximity alert |
| Buzzer | 1 | Audio alert |
| Resistors | 3 | Current limiting for LEDs |
| Breadboard & Jumper Wires | - | Circuit connections |

## Distance Zones
| Distance | LED | Buzzer |
|----------|-----|--------|
| > 30 cm | Green ON | OFF |
| 15 - 30 cm | Yellow ON | Slow beep |
| < 15 cm | Red ON | Fast beep |

## Circuit Connection
- HC-SR04 TRIG → Arduino Pin 9
- HC-SR04 ECHO → Arduino Pin 10
- Green LED → Arduino Pin 4
- Yellow LED → Arduino Pin 3
- Red LED → Arduino Pin 2
- Buzzer → Arduino Pin 5

## Software & Tools
- Arduino IDE
- Serial Monitor for distance debugging

## How to Run
1. Connect components as per circuit diagram above
2. Open Arduino IDE
3. Upload `parking_sensor.ino` to Arduino Uno
4. Power the Arduino via USB or 9V battery
5. Move an object toward the sensor to test

## Subject
Engineering Society Project | 
Universiti Teknikal Malaysia Melaka (UTeM)
