# ESPFlight Release Process

This document defines the repository-level integrity requirements for future official ESPFlight releases.

## General rules

- Published tags are immutable. Never rewrite, delete-and-recreate, or force-move an official release tag.
- Release notes must identify the exact component version and compatibility baseline.
- Binary or fabrication assets must include SHA-256 checksums where practical.
- Release artifacts must be distributed only from official ESPFlight channels.
- A release must not be represented as validated beyond the tests that were actually completed.

## Verified commits and tags

Future official release commits and tags should be cryptographically signed and shown by GitHub as **Verified**.

Maintainers should configure Git commit/tag signing locally or through an approved signing mechanism before creating the next release tag.

Recommended release sequence:

1. Complete the release candidate and documentation.
2. Run required CI and validation checks.
3. Commit the final release state with signing enabled.
4. Create an annotated, signed tag for the release.
5. Verify that GitHub displays the release commit/tag as Verified.
6. Create the GitHub Release from that immutable tag.
7. Attach release assets and checksums.
8. Re-check download hashes and compatibility information after publication.

The repository must not store private signing keys, Android keystores, recovery codes, tokens, or passwords.

## Firmware

Firmware release CI must compile the documented target with the pinned release dependencies.

For the v1.0.0 baseline these include:

- ESP8266 Arduino Core 3.1.2
- ArduinoJson 6.21.6
- ESPAsyncTCP 2.0.0
- ESPAsyncWebServer 3.6.0
- Adafruit VL53L0X 1.2.5 for altitude-assist support

Hardware/flight validation remains separate from CI compilation.

## Hardware

Future Hardware Reference releases must include:

- complete applicable license text;
- NOTICE;
- versioned editable design source snapshot;
- fabrication outputs;
- BOM;
- Pick-and-Place data when applicable;
- checksums;
- assembly and pin/interface documentation.

The existing Hardware Reference `v1.0` tag remains immutable. Packaging improvements belong in a later release rather than a rewritten tag.

## Application

Official application packages must remain signed with the controlled Android signing key.

Release documentation should publish:

- application version;
- package ID;
- SHA-256 of the APK;
- compatibility baseline;
- Android signing-certificate fingerprint when the maintainer publishes it.

Never commit the Android keystore or its passwords to a repository.

## Security gate

Before a future public release, every actively maintained repository should have a working private vulnerability-reporting route documented in `SECURITY.md`.

Sensitive vulnerability details must not be requested in public issues.

## Branch governance

Default branches should be protected by repository rules or branch protection. The intended baseline is:

- block force pushes;
- block branch deletion;
- require pull requests for safety-critical or release-critical changes;
- require applicable status checks before merge;
- keep administrator bypass limited and intentional.

These settings are repository administration controls and must be configured in GitHub settings when the connected integration does not expose administrative mutation APIs.
