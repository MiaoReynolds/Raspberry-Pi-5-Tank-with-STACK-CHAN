# Raspberry Pi 5 Tank with STACK-CHAN

This repository describes a robotics platform that combines:

- an **ESP32-based tank** as the motion controller
- a **Raspberry Pi 5** as the high-level master controller
- **STACK-CHAN** as the interactive user interface

At the current stage, this repository is project documentation only and does not contain implementation code yet.

## Project Overview

The goal is to build a modular smart tank system where low-level motor control is handled by ESP32, while Raspberry Pi 5 provides higher-level orchestration and AI-capable logic. STACK-CHAN serves as the interaction layer for expressive, human-friendly communication.

## Tank Body (Images 1-8)

The following photos document the ESP32 tank body, chassis layout, and assembly details.

### 1) Tank Image 1
![Tank Image 1](./1.jpg)

### 2) Tank Image 2
![Tank Image 2](./2.jpg)

### 3) Tank Image 3
![Tank Image 3](./3.jpg)

### 4) Tank Image 4
![Tank Image 4](./4.jpg)

### 5) Tank Image 5
![Tank Image 5](./5.jpg)

### 6) Tank Image 6
![Tank Image 6](./6.jpg)

### 7) Tank Image 7
![Tank Image 7](./7.jpg)

### 8) Tank Image 8
![Tank Image 8](./8.jpg)

## ESP32 Soldering Helper Tool (Images 12-14)

These images show a small helper tool used during ESP32 soldering and board preparation.

### 12) Tool Image 12
![Tool Image 12](./12.jpg)

### 13) Tool Image 13
![Tool Image 13](./13.jpg)

### 14) Tool Image 14
![Tool Image 14](./14.jpg)

## System Architecture

- **ESP32 Tank Layer**
  - Real-time motion control
  - Motor driver interfacing
  - Basic actuator and sensor signal handling

- **Raspberry Pi 5 Master Layer**
  - Mission and state management
  - Multi-module coordination
  - Future AI, vision, and voice integration

- **STACK-CHAN Interaction Layer**
  - Conversational front-end
  - Character-style interaction and feedback
  - User-facing command and status interface

## CAD Files and Print Count

| CAD File | Purpose | Print Quantity |
| --- | --- | --- |
| `Tank_body_48mm_V4.2.step` | Main tank body; contains two TT motors. | 1 |
| `tank_body_cover_V4.3.step` | First-layer top cover; mounts ESP32-C3 and L9110. | 1 |
| `tank_body_cover_RPi.step` | Second-layer top cover for Raspberry Pi 5 and battery module. Same function as `tank_body_cover_RPi_V1.1.step`, with a different height for wiring space options. | 1 |
| `tank_body_cover_RPi_V1.1.step` | Second-layer top cover for Raspberry Pi 5 and battery module. Same function as `tank_body_cover_RPi.step`, with a different height for wiring space options. | 1 |
| `sprocket_tank track 4_10teeth_V2.1.step` | Driving sprocket. | 2 |
| `sprocket_tank track 4_10teeth_V2.2.step` | Passive sprocket. | 2 |
| `Sprocket and track V4.1.step` | Tank track. | 2 |
| `ESP32_soldering_holder_v1.1.step` | ESP32 soldering holder tool. | 1 |

## Hardware Scope

The hardware setup for this project is centered around:

- Raspberry Pi 5 (master controller)
- ESP32 development board (tank-side controller)
- Tank chassis with dual DC motors
- Motor driver board (for example TB6612 or L298N)
- Power system (battery pack and power regulation)
- STACK-CHAN-compatible hardware modules
- Optional peripherals: camera, ultrasonic sensor, IMU, servos

## Additional Assembly Parts

- **M3 heat-set threaded inserts (female)**
  - Height: `6 mm`
  - Outer diameter: `3.5 mm`
  - Installation: press in with a flat-tip soldering iron
- **M3 bolts (`35-38 mm`)**
  - Flat-head type is recommended to avoid touching the bottom surface of the Raspberry Pi
- **M2.5 brass standoffs and bolts** (as needed)
  - For mounting the Raspberry Pi and battery module
- **`18650` battery**: `1`
- **Dupont wires**: several pieces (as needed)

## Project Status

- Documentation phase
- Hardware architecture defined
- Software implementation pending

## Roadmap (Planned)

- Define Pi5 <-> ESP32 communication protocol
- Implement tank motion command pipeline
- Integrate STACK-CHAN interaction flows
- Add sensor fusion and autonomous behaviors
- Add vision and voice-assisted control features

## Contributing

Issues and pull requests are welcome.
