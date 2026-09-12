# Contributing to ESPFlight

Thank you for your interest in ESPFlight.

ESPFlight is an open platform for learning, building, experimenting with, and developing ESP-based drones. Contributions that improve the open Firmware, Hardware Reference, documentation, testing, safety, or developer experience are welcome.

## Where to contribute

Choose the repository that matches the change:

- **Firmware:** https://github.com/espflight/firmware
- **Hardware Reference:** https://github.com/espflight/hardware
- **Documentation:** https://github.com/espflight/docs
- **Platform identity / licensing documents:** https://github.com/espflight/espflight

The ESPFlight Application is proprietary software. Its public repository is used for release information, downloads, documentation, and issue tracking; the application source code is not published there.

## Before opening an issue

Please:

1. Check the relevant documentation and existing issues.
2. Confirm which ESPFlight version you are using.
3. Reproduce the problem using the validated platform baseline where practical.
4. Remove passwords, Wi-Fi credentials, signing keys, private network information, and other secrets from logs or screenshots.

For ESPFlight v1.0, the validated baseline is:

- Firmware v1.0.0
- Hardware Reference v1.0
- Application v1.0.0
- Protocol 2

Build path: https://github.com/espflight/docs/blob/main/BUILD_V1.0.md

## Bug reports

A useful bug report should include:

- affected component and version;
- hardware configuration;
- clear reproduction steps;
- expected behavior;
- actual behavior;
- relevant logs or screenshots with secrets removed;
- whether the issue occurs during bench testing or powered flight.

For flight-control, motor, failsafe, power, or sensor issues, describe the test conditions carefully. Do not continue powered testing when behavior is unsafe or unpredictable.

## Feature requests

Describe the problem or use case first, then the proposed feature. Explain how it fits ESPFlight's role as an open learning and development platform rather than a closed finished product.

## Pull requests

Keep changes focused and explain:

- what changed;
- why it changed;
- how it was tested;
- any compatibility or safety implications;
- documentation that also needs updating.

Do not mix unrelated changes in one pull request.

Changes that alter communication protocols, pin assignments, control behavior, safety logic, power assumptions, or hardware interfaces should clearly document compatibility impact.

## Licensing and branding

Contributions to a repository are subject to that repository's applicable license and contribution context.

ESPFlight branding is separate from the open-source, open-hardware, and documentation licenses. The ESPFlight name, logo, visual identity, and other protected brand assets remain subject to the ESPFlight Brand Policy:

https://espflight.com/brand-policy/

Independent projects and products should use their own branding and must not imply official endorsement by ESPFlight unless explicitly authorized.

## Safety

ESPFlight controls real motors and flying hardware. Treat all changes that can affect motor output, flight state, sensing, communication, battery handling, or failsafe behavior as safety-relevant.

Bench-test without propellers where appropriate and follow applicable local laws and safety requirements.

---

**Learn it. Build it. Change it. Create your own.**
