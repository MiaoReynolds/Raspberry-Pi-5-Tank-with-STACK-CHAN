# Raspberry Pi 5 Tank with STACK-CHAN

This repository describes a robotics platform that combines:

- an **ESP32-based tank** as the motion controller,
- a **Raspberry Pi 5** as the high-level master controller,
- and **STACK-CHAN** as the interactive user interface.

At the current stage, this repository is project documentation only and does not contain implementation code yet.

## Project Overview

The goal is to build a modular smart tank system where low-level motor control is handled by ESP32, while Raspberry Pi 5 provides higher-level orchestration and AI-capable logic. STACK-CHAN serves as the interaction layer for expressive, human-friendly communication.

## System Architecture

- **ESP32 Tank Layer**
  - Real-time motion control
  - Motor driver interfacing
  - Basic actuator and sensor signal handling

- **Raspberry Pi 5 Master Layer**
  - Mission/state management
  - Multi-module coordination
  - Future AI/vision/voice integration

- **STACK-CHAN Interaction Layer**
  - Conversational front-end
  - Character-style interaction and feedback
  - User-facing command and status interface

## Hardware Scope

The hardware setup for this project is centered around:

- Raspberry Pi 5 (master controller)
- ESP32 development board (tank-side controller)
- Tank chassis with dual DC motors
- Motor driver board (for example TB6612 or L298N)
- Power system (battery pack and power regulation)
- STACK-CHAN-compatible hardware modules
- Optional peripherals: camera, ultrasonic sensor, IMU, servos

## Project Status

- Documentation phase
- Hardware architecture defined
- Software implementation pending

## Roadmap (Planned)

- Define Pi5 <-> ESP32 communication protocol
- Implement tank motion command pipeline
- Integrate STACK-CHAN interaction flows
- Add sensor fusion and autonomous behaviors
- Add vision/voice-assisted control features

## Contributing

Issues and pull requests are welcome.
