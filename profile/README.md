<div align="center">

# ESPFlight

### Open-source flight control ecosystem for ESP-based DIY quadcopters

Build. Learn. Fly. Improve.

[Website](https://espflight.com) · [Contact](mailto:info@espflight.com)

</div>

---

## What is ESPFlight?

**ESPFlight** is an open-source ecosystem for building, controlling, testing, and learning about lightweight DIY quadcopters based on ESP microcontrollers.

The goal is to make flight-control development more accessible to makers, students, developers, and drone enthusiasts through understandable source code, affordable hardware, practical documentation, and real-world testing.

ESPFlight is not intended to compete directly with large professional autopilot platforms. It focuses on a simpler and more approachable experience for compact experimental quadcopters.

---

## The ESPFlight Ecosystem

ESPFlight is being developed as a collection of connected projects:

### ESPFlight Firmware

The core flight-controller firmware for ESP-based quadcopters.

The firmware focuses on:

* Real-time flight control
* IMU-based attitude estimation
* PID stabilization
* Motor control and mixing
* Receiver and control input processing
* Arming and disarming safety
* Connection-loss protection
* Battery monitoring
* Modular and readable source code

### ESPFlight Lite

A lightweight Android application for controlling and monitoring supported ESPFlight quadcopters.

ESPFlight Lite is designed to provide the essential flight-control experience without unnecessary advanced features.

Its main goals are:

* Simple setup
* Clear flight information
* Responsive touch controls
* Reliable communication with the flight controller
* A clean interface optimized for landscape use

### Documentation

The documentation project will provide practical resources for building and understanding an ESPFlight quadcopter, including:

* Getting-started guides
* Wiring diagrams
* Firmware installation
* Configuration instructions
* IMU calibration
* PID tuning
* Safety recommendations
* Troubleshooting
* Software architecture
* Flight-control concepts

### Reference Hardware

ESPFlight will also provide reference hardware designs and tested component configurations.

The objective is to help users reproduce a known working setup instead of selecting every component through trial and error.

---

## Project Status

ESPFlight is currently under active development.

A working version of the firmware has completed real-world flight tests on the current reference quadcopter. The codebase is now being reviewed, simplified, documented, and prepared for its first public release.

The first public releases will focus on:

1. A stable firmware baseline
2. ESPFlight Lite for Android
3. Installation and configuration documentation
4. A documented reference quadcopter build
5. Examples for developers and makers

Repositories and release packages will be published when they are sufficiently tested and documented.

---

## Project Principles

ESPFlight is guided by several core principles:

### Practical over theoretical

Features should be tested on real hardware before being presented as stable.

### Understandable code

The source code should remain readable and useful for people who want to learn how a flight controller works.

### Affordable hardware

The platform should remain suitable for low-cost DIY builds and widely available components.

### Safety by design

Arming, failsafe behavior, battery monitoring, communication loss, and motor control must be treated as core system requirements.

### Modular development

Firmware, mobile applications, documentation, and hardware designs should remain organized as separate but connected projects.

### Honest documentation

Experimental, incomplete, and tested features must be identified clearly.

---

## Planned Repositories

The ESPFlight organization is expected to include the following repositories:

| Repository           | Purpose                                    | Status         |
| -------------------- | ------------------------------------------ | -------------- |
| `espflight-firmware` | Core flight-controller firmware            | In development |
| `espflight-lite`     | Lightweight Android controller application | In development |
| `espflight-docs`     | Documentation and build guides             | Planned        |
| `espflight-hardware` | Reference hardware and wiring designs      | Planned        |
| `espflight-examples` | Educational and development examples       | Planned        |

Repository names and structure may evolve before the first public release.

---

## Who Is ESPFlight For?

ESPFlight is intended for:

* DIY drone builders
* Electronics enthusiasts
* Students and educators
* Embedded developers
* Mobile application developers
* Makers learning flight-control systems
* Researchers experimenting with lightweight ESP-based aircraft

Basic experience with electronics, microcontrollers, soldering, and embedded programming is recommended.

---

## Contributing

ESPFlight is currently being prepared for public collaboration.

Contribution guidelines, coding standards, issue templates, and development documentation will be published with the relevant repositories.

Future contributions may include:

* Firmware improvements
* Bug reports
* Documentation
* Translation
* Hardware testing
* Android development
* Example projects
* Safety reviews

Please avoid submitting untested flight-critical changes without clearly identifying them as experimental.

---

## Safety Notice

ESPFlight is an experimental open-source project.

Quadcopters can cause injury, property damage, battery fires, and loss of control if assembled, configured, or operated incorrectly.

Always:

* Remove propellers during bench testing
* Test motor direction and output carefully
* Use a suitable power source
* Secure the aircraft before motor tests
* Keep people and animals away from the test area
* Perform the first flights in a large open space
* Follow local laws and aviation regulations
* Treat all flight-critical changes as experimental until tested

The project maintainers and contributors are not responsible for damage, injury, or loss resulting from the use of ESPFlight software, documentation, or hardware designs.

---

## Contact

* Website: [espflight.com](https://espflight.com)
* Email: [info@espflight.com](mailto:info@espflight.com)
* GitHub: [github.com/espflight](https://github.com/espflight)

---

<div align="center">

### ESPFlight

**An accessible path into DIY flight-control development.**

</div>
