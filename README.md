# Smart-Room-Monitoring-and-Obstacle-Detection-System
Repository Description

An IoT-based Smart Room Monitoring and Obstacle Detection System using ESP8266 NodeMCU, Arduino Uno, HC-SR04 Ultrasonic Sensor, Servo Motor, L298N Motor Driver, Dual DC Motors, and I2C LCD Display. The system provides real-time obstacle detection, autonomous navigation, Wi-Fi connectivity, live monitoring, and manual robot control through a web dashboard.

README.md
Smart Room Monitoring and Obstacle Detection System

Overview

This project is an IoT-enabled smart robotic system designed for indoor room monitoring and autonomous obstacle detection. The system combines the processing capabilities of an Arduino Uno with the wireless communication features of the ESP8266 NodeMCU to create an intelligent monitoring platform.

The Arduino Uno handles real-time sensor readings and motor control, while the ESP8266 manages Wi-Fi communication, LCD updates, and interaction with a web-based dashboard. An HC-SR04 ultrasonic sensor mounted on a servo motor scans the surroundings to detect obstacles and determines the safest direction for movement.

Features
Autonomous obstacle detection
Smart obstacle avoidance
Servo-based environmental scanning
Wi-Fi connectivity using ESP8266
Manual and automatic navigation modes
Real-time distance monitoring
LCD display for system status
Dual DC motor control
Web dashboard integration
Modular hardware architecture
Expandable IoT platform
Hardware Components
ESP8266 NodeMCU
Arduino Uno
HC-SR04 Ultrasonic Sensor
SG90 Servo Motor
L298N Motor Driver
2 × DC Geared Motors
I2C 16×2 LCD Display
External 5V Voltage Regulator
12V Battery
Chassis with Wheels
Jumper Wires
Hardware Architecture

The project is divided into three main subsystems:

1. ESP8266 (NodeMCU) Subsystem

Responsibilities:

Connect to Wi-Fi

Control Servo Motor

Drive I2C LCD Display

Send and receive commands

Display system status

Interface with dashboard

2. Arduino Uno Subsystem

Responsibilities:

Read ultrasonic sensor

Calculate obstacle distance

Control L298N Motor Driver

Drive left and right motors

Execute obstacle avoidance logic

3. Power Distribution
   
12V Battery

External 5V Regulator

Common Ground

Stable power supply for all modules

Pin Configuration

ESP8266

Component	Pin

LCD SDA	D2 (GPIO4)

Servo Signal	D5 (GPIO14)

Arduino Uno

Component	Pin

HC-SR04 Trigger	D9

HC-SR04 Echo	D10

L298N IN1	D2

L298N IN2	D3

L298N IN3	D4

L298N IN4	D5

ENA	D6 (PWM)

ENB	D7 (PWM)

Project Workflow

Power on the system.

ESP8266 connects to the configured Wi-Fi network.

Arduino continuously reads the ultrasonic sensor.

Distance is calculated in centimeters.

Servo rotates the ultrasonic sensor to scan left, center, and right.

If no obstacle is detected, the robot moves forward.

If an obstacle is detected, the robot stops, scans both directions, selects the safest path, and continues moving.

Sensor data and system status are displayed on the LCD and sent to the web dashboard.

Users can also manually control the robot using the dashboard.

Technologies Used

Hardware

ESP8266 NodeMCU

Arduino Uno

HC-SR04

Servo Motor

L298N Motor Driver

I2C LCD

Software

Arduino IDE

C++

ESP8266 Libraries

I2C LCD Library

Servo Library

Dashboard (Optional)

React.js

Node.js

Express.js

WebSocket

SQLite

Tailwind CSS

Future Enhancements

Temperature and humidity monitoring

Gas leakage detection

Fire detection

Mobile application

Camera integration

AI-based object recognition

Voice assistant support

MQTT cloud communication

Firebase integration

Cloud data analytics

Applications

Smart homes

Office monitoring

Indoor surveillance

Warehouse automation

Educational robotics

Research and development

IoT learning projects

Autonomous navigation systems




Repository Structure


Smart-Room-Monitoring/
│
├── Arduino/
│   ├── ArduinoCode.ino
│
├── ESP8266/
│   ├── NodeMCU_Code.ino
│
├── Circuit/
│   ├── Circuit_Diagram.png
│
├── Dashboard/
│   ├── frontend/
│   ├── backend/
│
├── Images/
│
├── Documentation/
│
├── README.md
│
└── LICENSE


License

This project is developed for educational and research purposes. Feel free to modify and extend it for your own IoT and robotics applications.
