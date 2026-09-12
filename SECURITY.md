# ESPFlight Security Policy

ESPFlight welcomes responsible reports of security issues that could affect users, connected controllers, the ESPFlight Application, or the integrity of official release files.

## Supported public baseline

The current v1.0 platform baseline is:

- ESPFlight Firmware v1.0.0
- ESPFlight Hardware Reference v1.0
- ESPFlight Application v1.0.0
- ESPFlight Protocol 2

Security fixes may be released in later patch or minor versions when required.

## Network security note

ESPFlight Protocol 2 is designed for use on a private, trusted local Wi-Fi network.

The v1 control and telemetry transport does **not** provide encrypted or authenticated protection against hostile clients on the same network. This is a documented limitation of the v1 baseline rather than an undisclosed security guarantee.

Do not operate ESPFlight flight-control links on untrusted or hostile networks.

## Reporting a vulnerability

Please do not publish sensitive exploit details, credentials, private keys, signing material, or a working attack against flight-control behavior in a public issue.

If GitHub's **Report a vulnerability** / private vulnerability reporting option is available for the affected repository, use that channel.

If a private reporting option is not available, open a minimal public issue stating that you need a private channel for a security report, but **do not include sensitive technical details or exploit steps** in that issue.

For ordinary bugs that do not require confidential handling, use the relevant repository's Issues section.

## What to include

When reporting privately, include where possible:

- affected ESPFlight component and version;
- hardware and network context;
- impact and realistic attack conditions;
- reproduction steps or proof of concept;
- whether physical access or same-network access is required;
- suggested mitigation, if known.

Remove unrelated personal data and never include Wi-Fi passwords, private signing keys, Android keystores, or other secrets.

## Safety-sensitive reports

Issues involving unauthorized motor control, ARM / DISARM behavior, failsafe bypass, command injection, telemetry/control ownership, or unsafe recovery behavior should be treated as both security- and safety-sensitive.

Do not continue powered flight testing if the behavior could create an uncontrolled or unpredictable condition.

## Scope

ESPFlight's open Firmware and Hardware Reference can be modified and integrated into independent systems. Security characteristics of third-party modifications, networks, hardware, products, or repackaged software are outside the control of the ESPFlight project.

Only official ESPFlight Application packages distributed through ESPFlight channels should be treated as official releases.

Official website: https://espflight.com

---

**Learn it. Build it. Change it. Create your own.**
