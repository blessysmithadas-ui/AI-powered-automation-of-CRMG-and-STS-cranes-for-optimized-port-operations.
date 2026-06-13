Hardware Used

Overview
The prototype was developed using a combination of embedded controllers, vision systems, motor drivers, actuators, and power electronics to simulate the operation of an automated Ship-to-Shore (STS) crane. The hardware architecture was designed to support real-time container tracking, autonomous crane movement, and reliable communication between software and mechanical subsystems.

Processing and Control Units

Arduino Mega 2560
The Arduino Mega 2560 served as the primary hardware controller during the final phase of development. It received control instructions from the processing system and generated PWM signals for motor control.

Key Functions

Motor control
Motion coordination
Serial communication
Real-time execution of control commands

ESP32
The ESP32 microcontroller was used extensively during the initial development phases for manual and semi-automated crane control.

Key Functions
Joystick input processing
Motor control
Wireless communication capability
Rapid prototyping and testing
Vision System

High-Resolution Cameras
Three cameras were strategically positioned to monitor crane movements along different axes.

Camera Placement
Hoist Camera (Z-Axis)
Monitors vertical container movement.

Trolley Camera (X-Axis)
Tracks horizontal trolley positioning.

Gantry Camera (Y-Axis)
Monitors crane travel along the gantry rail.

Purpose
Real-time visual monitoring
Container detection
Position verification
Motion feedback
Motor Driver System
Custom BTS7970-Based H-Bridge Motor Driver

A custom-designed motor driver circuit was developed using BTS7970 half-bridge driver ICs to support high-current motor operation.

Key Features
Bidirectional motor control
PWM speed regulation
High current handling capability
Reliable operation under continuous load
Purpose
Drive gantry motors
Drive trolley motors
Drive hoist motors
Ensure precise motion control

A4988 Stepper Motor Driver
Used during the initial prototype phase for controlling stepper motors.
Purpose
Boom movement control
Precision positioning
Motion testing and validation

Actuation System

Johnson DC Geared Motors
Johnson DC geared motors were selected during the final implementation phase to provide reliable and accurate motion control.

Applications
Gantry Movement
Controls crane travel along the rail system.

Trolley Movement
Moves the trolley across the crane structure.

Hoist Movement
Handles container lifting and lowering operations.

Advantages
High torque
Smooth operation
Improved efficiency
Better speed control

Stepper Motors
Used during early prototype development for precision movement experiments and boom actuation.
Advantages
Accurate positioning
Repeatable motion
Easy integration with controllers

Servo Motor
A servo motor was integrated into the spreader mechanism.
Purpose
Simulate container locking
Simulate container unlocking
Precise angular positioning

Input Devices
Three-Axis Joystick
Used during the manual control phase of the project.
Functions
Gantry control
Trolley control
Hoist control
Spreader actuation

Purpose
To study crane behaviour before transitioning to autonomous operation.

Power Electronics
12V Switched Mode Power Supply (SMPS)
Provided the primary power source for the prototype.

Specifications
Output Voltage: 12V
Current Rating: 10A–20A
Purpose
Motor power supply
Driver circuit power supply
System-wide power distribution
Voltage Regulation Circuit

Custom voltage regulation circuitry was implemented to provide stable operating voltages for different hardware modules.
Output Levels
12V for motors
9V for controllers
5V for sensors and logic circuits
Components
7805 Voltage Regulator
7812 Voltage Regulator

Communication Interface
Serial Communication
Serial communication was used to transfer control commands from the processing system to the Arduino Mega.

Purpose
Real-time command transmission
Hardware synchronization
Control signal exchange
Prototype Summary

The hardware platform combines computer vision, embedded control systems, custom motor drivers, and industrial-style actuation mechanisms to demonstrate the feasibility of intelligent crane automation. The architecture was designed to support real-time monitoring, autonomous movement, and scalable deployment for future smart-port applications.
