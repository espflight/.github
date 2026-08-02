<div align="center">

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/espflight/.github/blob/main/profile/README.md">
        <strong>🇬🇧 English ✓</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/espflight/.github/blob/main/profile/README.de.md">
        <strong>Deutsch</strong>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/espflight/.github/blob/main/profile/README.fa.md">
        <strong>فارسی</strong>
      </a>
    </td>
  </tr>
</table>

<h1>ESPFlight</h1>

<h3>
Open-source flight-control ecosystem for lightweight ESP-based DIY quadcopters
</h3>

<p>
<strong>Build. Learn. Fly. Improve.</strong>
</p>

<br>

<a href="https://espflight.com">
  <img alt="ESPFlight Website" src="https://img.shields.io/badge/Website-espflight.com-0284C7?style=for-the-badge&logo=googlechrome&logoColor=white">
</a>
<a href="https://github.com/espflight?tab=repositories">
  <img alt="ESPFlight Repositories" src="https://img.shields.io/badge/GitHub-Repositories-181717?style=for-the-badge&logo=github&logoColor=white">
</a>
<a href="mailto:info@espflight.com">
  <img alt="ESPFlight Email" src="https://img.shields.io/badge/Contact-Email-0F766E?style=for-the-badge&logo=gmail&logoColor=white">
</a>

<br>

<img alt="Project Status" src="https://img.shields.io/badge/Status-Preparing_for_Public_Release-F59E0B?style=flat-square">
<img alt="Reference Target" src="https://img.shields.io/badge/Reference_Target-ESP8266-00979D?style=flat-square&logo=espressif&logoColor=white">
<img alt="Mobile Platform" src="https://img.shields.io/badge/Mobile_App-Android-3DDC84?style=flat-square&logo=android&logoColor=white">

<br>

<p>
<strong>Firmware · Android Controller · Documentation · Reference Build</strong>
</p>

</div>

## About ESPFlight

**ESPFlight** is an open-source ecosystem for building, controlling, testing, and understanding lightweight DIY quadcopters based on ESP microcontrollers.

The project combines flight-controller firmware, a dedicated Android application, practical documentation, and a tested reference build to provide an accessible path into DIY flight-control development.

ESPFlight is designed for makers, students, educators, embedded developers, and drone enthusiasts who want to understand how a flight-control system works and experiment with affordable hardware.

---

## The Ecosystem

### 🚁 ESPFlight Firmware

The core flight-controller firmware responsible for processing pilot commands and maintaining stable flight.

Current development areas include:

* IMU data processing
* Attitude estimation
* PID stabilization
* Motor mixing and output
* Receiver input processing
* Flight-state management
* Arming and disarming logic
* Communication-loss failsafe
* Battery-voltage monitoring
* Low-voltage response
* Modular flight-control architecture

### 📱 ESPFlight Lite

A lightweight Android application designed specifically for supported ESPFlight quadcopters.

Its primary functions include:

* Touch-based flight controls
* Wi-Fi communication
* Connection monitoring
* Essential flight telemetry
* Battery and signal information
* Flight-time display
* PID configuration
* Landscape-optimized controls
* English and Persian interface support

ESPFlight Lite focuses on the essential tools required to configure, control, and monitor a supported aircraft.

### 📚 Documentation

The ESPFlight documentation will provide practical instructions for:

* Building the reference quadcopter
* Wiring electronic components
* Installing the firmware
* Configuring the flight controller
* Calibrating the IMU
* Testing motors safely
* Understanding arming and failsafe behavior
* Tuning PID values
* Troubleshooting common problems
* Understanding the source-code architecture

### 🔧 Reference Build

ESPFlight will document a known working hardware configuration based on the aircraft used during development and flight testing.

The reference build is intended to provide:

* Tested component selection
* Wiring diagrams
* Motor and propeller configuration
* Power-system guidance
* Assembly instructions
* Firmware configuration
* Pre-flight safety checks
* Initial flight-testing procedures

---

## Project Status

> [!IMPORTANT]
> ESPFlight is under active development and is currently being prepared for its first public release.

A working development version of the firmware has completed real-world flight tests on the current ESP8266-based reference quadcopter.

Current work focuses on reviewing flight-critical code, completing the failsafe system, simplifying the project structure, improving documentation, and preparing ESPFlight Lite for the public firmware release.

### Current progress

* [x] Working flight-control firmware
* [x] Successful real-world flight testing
* [x] ESPFlight Lite Android controller
* [ ] Complete the communication-loss failsafe review
* [ ] Complete the low-voltage behavior review
* [ ] Clean and organize the firmware source code
* [ ] Prepare installation and configuration guides
* [ ] Document the reference quadcopter
* [ ] Publish the first public release

No public release date has been announced.

---

## Planned Repositories

| Repository           | Purpose                              |     Status     |
| :------------------- | :----------------------------------- | :------------: |
| `espflight-firmware` | Core flight-controller firmware      | In development |
| `espflight-lite`     | Lightweight Android controller       | In development |
| `espflight-docs`     | Documentation and build guides       |     Planned    |
| `espflight-hardware` | Reference build and wiring resources |     Planned    |
| `espflight-examples` | Educational and development examples |     Planned    |

Repository names and organization may evolve before publication.

---

## Project Principles

### Tested before stable

Flight-critical behavior should be tested on real hardware before being described as stable.

### Safety as a core requirement

Arming, motor output, communication loss, battery voltage, and failsafe behavior are fundamental parts of the system.

### Understandable source code

The codebase should remain readable enough to help developers understand how the flight controller works.

### Modular development

Firmware, applications, documentation, and hardware resources should remain organized as separate but connected projects.

### Affordable and accessible hardware

ESPFlight should remain suitable for lightweight DIY builds using commonly available components.

### Honest project status

Experimental, incomplete, tested, and stable features should always be identified clearly.

---

## Intended Audience

ESPFlight is being developed for:

* DIY drone builders
* Electronics enthusiasts
* Students and educators
* Embedded-system developers
* Android developers
* Makers learning flight-control concepts
* Developers experimenting with ESP microcontrollers

Experience with electronics, soldering, microcontrollers, and embedded programming is recommended.

---

## Contributing

ESPFlight is currently being prepared for public collaboration.

Contribution guidelines, coding standards, issue templates, and testing requirements will be published with the relevant repositories.

Future contributions may include:

* Firmware development
* Android development
* Bug reports
* Documentation
* Translation
* Hardware testing
* Safety reviews
* Example projects

> [!NOTE]
> Flight-critical modifications should be clearly marked as experimental until their behavior has been validated through controlled testing.

---

## Safety Notice

> [!WARNING]
> ESPFlight is experimental software. Quadcopters can cause injury, property damage, battery fires, or loss of control when assembled, configured, modified, or operated incorrectly.

Before testing:

* Remove all propellers during bench tests
* Secure the aircraft before testing motors
* Verify motor order and rotation direction
* Use suitable batteries and power components
* Test arming and failsafe behavior without propellers
* Keep people and animals away from the test area
* Conduct initial flights in a large open area
* Follow applicable aviation and safety regulations

Use ESPFlight entirely at your own risk.

---

<div align="center">

## ESPFlight

**An accessible path into DIY flight-control development.**

<br>

<a href="https://espflight.com">
  <img alt="Visit ESPFlight" src="https://img.shields.io/badge/Visit-espflight.com-0284C7?style=for-the-badge&logo=googlechrome&logoColor=white">
</a>

<br><br>

<sub>ESPFlight is under active development.</sub>

</div>
