# Obstacle Avoidance Voice Control Car Robot

This project is an Arduino-based robot that autonomously avoids obstacles and can be controlled via voice commands. It uses ultrasonic sensors for obstacle detection and a voice recognition module to interpret user instructions. The robot can move forward, backward, turn left, turn right, and stop based on commands received through the serial interface. It utilizes ultrasonic distance measurement to avoid obstacles, ensuring smooth operation.

## Features

- **Autonomous Navigation**: The robot avoids obstacles by detecting them with ultrasonic sensors.
- **Voice Control**: Voice commands are used to control the robot's movements.
- **Arduino-Based**: Built with Arduino, making it easily customizable and extendable.

## Components Used

- Arduino board (Arduino Uno)
- Ultrasonic sensor (for obstacle detection)
- Voice recognition module
- Motors and motor shield
- Chassis and wheels
- Jumper wires

## Functions

- **setup()**: Initializes serial communication, pin modes, and attaches the servo.
- **forward()**: Moves the robot forward.
- **backward()**: Moves the robot backward.
- **left()**: Turns the robot left.
- **right()**: Turns the robot right.
- **Stop()**: Stops all motor movements.
- **loop()**: Reads commands from the serial interface and executes corresponding movements.
- **ultrasonic()**: Measures distance using the ultrasonic sensor.

## Command List

The robot responds to the following commands via serial input:

- **move forward**: Moves the robot forward until an obstacle is detected.
- **move backward**: Moves the robot backward.
- **turn left**: Turns the robot left.
- **turn right**: Turns the robot right.
- **stop**: Stops all movements.

## How It Works

1. The ultrasonic sensor continuously detects the distance between the robot and nearby objects.
2. When an obstacle is detected, the robot adjusts its movement to avoid a collision.
3. The voice recognition module interprets commands to control movement such as forward, backward, left, or right.

## How to Use

1. Set up the robot with the necessary components.
2. Upload the Arduino code to the board.
3. Use the predefined voice commands to control the robot (e.g., "move forward," "turn left").
4. Watch the robot navigate and avoid obstacles autonomously.

## Requirements

- Arduino IDE
- Voice recognition module library for Arduino
- Ultrasonic sensor library for Arduino
