<div align="center">

# ESPFlight

### Open-source flight control ecosystem for ESP-based DIY quadcopters

<p>
  Build affordable aircraft, understand flight control, and develop with open-source tools.
</p>

<p>
  <a href="https://espflight.com">
    <img alt="Website" src="https://img.shields.io/badge/Website-espflight.com-0EA5E9?style=for-the-badge&logo=googlechrome&logoColor=white">
  </a>
  <a href="https://github.com/espflight">
    <img alt="GitHub Organization" src="https://img.shields.io/badge/GitHub-Organization-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="mailto:info@espflight.com">
    <img alt="Email" src="https://img.shields.io/badge/Contact-info%40espflight.com-14B8A6?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
</p>

<p>
  <img alt="Project Status" src="https://img.shields.io/badge/Status-Active_Development-F59E0B?style=flat-square">
  <img alt="Platform" src="https://img.shields.io/badge/Platform-ESP8266-00979D?style=flat-square&logo=espressif&logoColor=white">
  <img alt="Mobile App" src="https://img.shields.io/badge/Mobile-Android-3DDC84?style=flat-square&logo=android&logoColor=white">
  <img alt="Project Type" src="https://img.shields.io/badge/Project-Open_Source-22C55E?style=flat-square&logo=opensourceinitiative&logoColor=white">
</p>

<br>

**Firmware · Mobile Controller · Documentation · Reference Hardware**

</div>

---

## About ESPFlight

**ESPFlight** is an open-source ecosystem for building, controlling, testing, and learning about lightweight DIY quadcopters based on ESP microcontrollers.

The project aims to make flight-control development more accessible to makers, students, embedded developers, educators, and drone enthusiasts through:

* Understandable source code
* Affordable and widely available hardware
* Practical documentation
* Mobile-based flight control
* Real-world testing
* Reproducible reference builds

ESPFlight is not intended to replace large professional autopilot platforms.

Instead, it focuses on providing a simpler and more approachable path for learning, building, experimenting, and developing compact ESP-based aircraft.

---

## Ecosystem

<table>
<tr>
<td width="50%" valign="top">

### 🚁 ESPFlight Firmware

The core flight-controller firmware for supported ESP-based quadcopters.

**Primary responsibilities:**

* Real-time flight control
* IMU data processing
* Attitude estimation
* PID stabilization
* Motor mixing and output
* Receiver input processing
* Arming and disarming safety
* Communication-loss protection
* Battery monitoring
* Flight-state management

</td>
<td width="50%" valign="top">

### 📱 ESPFlight Lite

A lightweight Android application for controlling and monitoring supported ESPFlight aircraft.

**Primary goals:**

* Simple setup
* Responsive touch controls
* Essential flight information
* Reliable communication
* Landscape-optimized interface
* Clear connection status
* Accessible configuration
* No unnecessary advanced features

</td>
</tr>

<tr>
<td width="50%" valign="top">

### 📚 Documentation

Practical guides for building, configuring, testing, and understanding an ESPFlight quadcopter.

**Planned documentation:**

* Getting started
* Wiring diagrams
* Firmware installation
* IMU calibration
* PID configuration
* Motor testing
* Failsafe behavior
* Troubleshooting
* Flight-control concepts
* Software architecture

</td>
<td width="50%" valign="top">

### 🔧 Reference Hardware

Tested hardware configurations and reference designs for reproducible ESPFlight builds.

**Planned resources:**

* Component lists
* Wiring references
* Supported configurations
* Frame recommendations
* Motor and propeller setup
* Power-system guidance
* Assembly instructions
* Safety checklists
* Reference flight builds

</td>
</tr>
</table>

---

## Project Status

> [!IMPORTANT]
> ESPFlight is currently under active development and is not yet considered production-ready.

A working firmware version has completed real-world flight tests on the current reference quadcopter.

The project is now being reviewed, simplified, documented, and prepared for its first public release.

### Current focus

```text
Firmware stabilization
        ↓
Failsafe and safety review
        ↓
Code cleanup and documentation
        ↓
ESPFlight Lite integration
        ↓
Reference hardware documentation
        ↓
First public release
```

### Initial release objectives

* Stable firmware baseline
* Reliable communication-loss failsafe
* Battery monitoring and protection
* ESPFlight Lite Android application
* Firmware installation instructions
* Configuration documentation
* Documented reference quadcopter
* Developer and hardware examples

Repositories and release packages will be published when they are sufficiently tested and documented.

---

## Planned Repositories

| Repository           | Description                                |       Status      |
| :------------------- | :----------------------------------------- | :---------------: |
| `espflight-firmware` | Core ESPFlight flight-controller firmware  | 🚧 In development |
| `espflight-lite`     | Lightweight Android controller application | 🚧 In development |
| `espflight-docs`     | Documentation, tutorials, and build guides |     📝 Planned    |
| `espflight-hardware` | Reference hardware and wiring designs      |     📝 Planned    |
| `espflight-examples` | Educational and development examples       |     📝 Planned    |

> Repository names and structure may evolve before the first stable public release.

---

## Project Principles

<table>
<tr>
<td width="33%" valign="top">

### 🧪 Tested Features

Flight-critical features should be tested on real hardware before being presented as stable.

</td>
<td width="33%" valign="top">

### 🧩 Modular Design

Firmware, applications, documentation, and hardware should remain organized and maintainable.

</td>
<td width="33%" valign="top">

### 📖 Readable Code

The source code should help developers understand how the flight-control system works.

</td>
</tr>

<tr>
<td width="33%" valign="top">

### 💡 Accessible Development

The project should remain approachable for students, makers, and embedded developers.

</td>
<td width="33%" valign="top">

### 💰 Affordable Hardware

ESPFlight should remain suitable for low-cost DIY builds using available components.

</td>
<td width="33%" valign="top">

### 🛡️ Safety First

Arming, motors, failsafe, battery monitoring, and communication loss are core requirements.

</td>
</tr>
</table>

---

## Who Is ESPFlight For?

ESPFlight is intended for:

* DIY drone builders
* Electronics enthusiasts
* Embedded developers
* Students and educators
* Mobile application developers
* Makers learning flight-control systems
* Developers experimenting with ESP microcontrollers
* Researchers working with lightweight experimental aircraft

Basic experience with electronics, microcontrollers, soldering, and embedded programming is recommended.

---

## Technology Direction

ESPFlight is being developed around a modular ecosystem:

```text
┌──────────────────────────────────────────────────────┐
│                  ESPFlight Ecosystem                 │
├───────────────────────┬──────────────────────────────┤
│                       │                              │
│  ESPFlight Firmware   │      ESPFlight Lite          │
│                       │                              │
│  • Flight control     │      • Touch controls        │
│  • PID stabilization  │      • Flight information    │
│  • IMU processing     │      • Configuration         │
│  • Motor management   │      • Status monitoring     │
│  • Safety systems     │      • Android interface     │
│                       │                              │
├───────────────────────┴──────────────────────────────┤
│                                                     │
│       Documentation · Hardware · Examples           │
│                                                     │
└─────────────────────────────────────────────────────┘
```

---

## Contributing

ESPFlight is currently being prepared for public collaboration.

Contribution guidelines, coding standards, issue templates, and development documentation will be published with the relevant repositories.

Future contributions may include:

* Firmware improvements
* Bug reports
* Android development
* Documentation
* Translation
* Hardware testing
* Safety reviews
* Example projects
* Reference builds

> [!NOTE]
> Flight-critical changes should be tested carefully and clearly marked as experimental until their behavior has been validated on real hardware.

---

## Safety Notice

> [!WARNING]
> ESPFlight is an experimental open-source project. Quadcopters can cause injury, property damage, battery fires, or loss of control if assembled, configured, modified, or operated incorrectly.

Always:

* Remove propellers during bench testing
* Secure the aircraft before motor tests
* Verify motor order and rotation direction
* Use suitable batteries and power components
* Keep people and animals away from the test area
* Test failsafe behavior before the first flight
* Perform initial flights in a large open area
* Follow local aviation laws and regulations
* Treat untested flight-critical changes as experimental

The project maintainers and contributors are not responsible for damage, injury, or loss resulting from the use of ESPFlight software, documentation, or hardware designs.

---

## Follow the Project

<div align="center">

<p>
  <a href="https://espflight.com">
    <img alt="Visit ESPFlight Website" src="https://img.shields.io/badge/Visit_Our_Website-0EA5E9?style=for-the-badge&logo=googlechrome&logoColor=white">
  </a>
  <a href="https://github.com/espflight">
    <img alt="Explore ESPFlight on GitHub" src="https://img.shields.io/badge/Explore_on_GitHub-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="mailto:info@espflight.com">
    <img alt="Contact ESPFlight" src="https://img.shields.io/badge/Contact_ESPFlight-14B8A6?style=for-the-badge&logo=gmail&logoColor=white">
  </a>
</p>

<br>

### Build. Learn. Fly. Improve.

**An accessible path into DIY flight-control development.**

<br>

<sub>ESPFlight is under active development.</sub>

</div>
