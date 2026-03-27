#Automatic Solar Panel Orientation System (Wireless Control)
Overview

This project implements a wireless-controlled system for automatic solar panel positioning. A microcontroller-based setup receives control commands transmitted from a remote computer via RF modules. The received signal is decoded and used to drive a servo motor, adjusting the panel’s angle relative to the light source. After execution, the system enters a low-activity waiting state until the next command is received.

#Key Features
Wireless communication between two systems using RF modules
Real-time signal reception and decoding on microcontroller
Servo motor control for precise angular positioning
Event-driven architecture (idle → receive → execute → idle)
Lightweight embedded implementation suitable for low-power systems
System Workflow
Command is sent from a transmitting computer
RF module transmits the signal wirelessly
Receiver module passes data to the microcontroller
Microcontroller decodes the signal
Servo motor adjusts the solar panel angle accordingly
System returns to standby mode awaiting next command
#Tech Stack
C / C++
Microcontroller platform (e.g., STM32 / Arduino-based)
RF communication modules (e.g., nRF24L01 / 433 MHz)
Servo motor control (PWM)
