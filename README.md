# ArcForge

Operator-first robotics software for ROS 2.

ArcForge is a cross-platform robotics platform designed to simplify the deployment, operation, and validation of ROS 2-based systems. Built for Windows, macOS, and Linux, ArcForge provides visual tooling that helps operators and developers configure hardware, validate system readiness, monitor telemetry, and conduct missions without requiring deep ROS expertise.

## Why ArcForge?

ROS 2 is powerful, but many robotics teams still rely on command-line tools, custom scripts, and fragmented workflows to configure and operate vehicles.

ArcForge aims to provide a modern desktop experience for robotics operators by bringing configuration, validation, telemetry, simulation, and mission workflows into a unified platform.

Key goals:

- Reduce setup complexity
- Improve operator awareness
- Increase deployment reliability
- Detect configuration mistakes before field operations
- Make ROS 2 more accessible to non-software specialists

---

## Current Modules

### ArcFlight

Ground control and mission operations for aerial systems.

Features include:

- Live telemetry monitoring
- Flight HUD
- Mission planning
- Route planning
- Preflight readiness validation
- Vehicle health monitoring
- Telemetry recording and replay
- Hardware profile validation

---

### ArcGround

Ground vehicle operations built on the ArcForge Runtime.

Features include:

- Shared operational interface
- Vehicle telemetry
- Readiness validation
- Mission workflows
- Support for ROS 2-based UGV platforms

---

### ArcSim

Simulation and replay environment for training, testing, and validation.

Features include:

- Telemetry replay
- Scenario testing
- Disturbance injection
- Operator training workflows
- Mission review and analysis

---

## Hardware Validation

One of ArcForge's core capabilities is design-versus-detected hardware validation.

ArcForge compares the vehicle configuration defined by the operator against hardware discovered at runtime and highlights mismatches before deployment.

Examples include:

- Missing sensors
- Incorrect hardware selections
- Communication failures
- Profile mismatches
- Unsupported configurations

This helps identify problems before they become field failures.

---

## Operator Trust Systems

ArcForge is designed to explain system state instead of failing silently.

Rather than simply displaying:

> Disconnected

ArcForge attempts to identify and communicate:

- Which subsystem failed
- Why a command was blocked
- Which service is unavailable
- Why telemetry is stale
- What readiness requirement is unmet
- Which capability is unsupported

The goal is to improve operator confidence and reduce troubleshooting time.

---

## Platform Architecture

ArcForge is built around a shared runtime architecture that supports multiple vehicle domains.

Current platform direction:

- Shared ArcForge Runtime
- ROS 2 integration
- Cross-platform desktop application
- Hardware-agnostic deployment model
- Air and ground vehicle support
- Simulation and replay support
- Future multi-vehicle orchestration capabilities

---

## Technology Stack

- Electron
- React
- TypeScript
- ROS 2
- MAVROS
- rosbridge
- Pixhawk ecosystem support
- Raspberry Pi companion computers

---

## Project Status

ArcForge is currently under active development.

The platform is being tested with:

- PX4 and Pixhawk-based systems
- Raspberry Pi companion computers
- ROS 2 Humble and Jazzy
- Ground vehicle prototypes
- Telemetry replay and simulation workflows

Additional documentation, screenshots, demo videos, and public releases will be added as development continues.

---

## Screenshots

Coming soon.

---

## Roadmap

Near-term priorities:

- ArcGround field testing
- LiDAR integration
- Expanded simulation capabilities
- Runtime hardening
- Reproducible deployment workflows
- Enhanced operator trust systems
- Additional hardware support

---

## Contact

For questions, feedback, or collaboration opportunities, please open an issue or contact the project maintainer through GitHub.

---

ArcForge: Robotics software that helps operators understand what their systems are doing, why they are doing it, and whether they are ready to perform the mission.
