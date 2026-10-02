# ESPFlight Release Process

This document defines the repository-level integrity requirements for future official ESPFlight releases.

## General rules

- Published tags are immutable. Never rewrite, delete-and-recreate, or force-move an official release tag.
- Version tags matching `v*` in Firmware, Hardware Reference, and Application are protected by active GitHub tag rulesets against deletion, update, and non-fast-forward changes.
- Release notes must identify the exact component version and compatibility baseline.
- Binary or fabrication assets must include SHA-256 checksums where practical.
- Release artifacts must be distributed only from official ESPFlight channels.
- A release must not be represented as validated beyond the tests that were actually completed.
- Release immutability is enabled for future Firmware, Hardware Reference, and Application GitHub Releases, per maintainer confirmation.

Historical v1.0 / v1.0.0 releases remain unchanged. Do not rewrite an existing release solely to retrofit signing, packaging, or immutability features that were enabled later.

## Verified commits and tags

Future official release commits and annotated release tags should be cryptographically signed and shown by GitHub as **Verified**.

The maintainer signing setup has been tested successfully with both an SSH-signed commit and an SSH-signed annotated tag.

Recommended release sequence:

1. Complete the release candidate and documentation.
2. Run required CI and validation checks.
3. Commit the final release state with signing enabled.
4. Create an annotated, signed version tag.
5. Verify that GitHub displays the release commit and tag as **Verified**.
6. Create the GitHub Release from that protected tag.
7. Attach release assets and checksums.
8. Publish the release only after asset names, hashes, version compatibility, and release notes are re-checked.
9. Confirm the published release is immutable under the repository's release settings.

The repository must not store private signing keys, Android keystores, recovery codes, tokens, passwords, or other release secrets.

## Firmware

Firmware release CI must compile the documented target with the pinned release toolchain and dependencies.

For the current v1.0.0 CI baseline these include:

- Arduino CLI 1.5.1
- ESP8266 Arduino Core 3.1.2
- ArduinoJson 6.21.6
- ESPAsyncTCP 2.0.0, resolved by exact commit in CI
- ESPAsyncWebServer 3.6.0, resolved by exact commit in CI
- Adafruit VL53L0X 1.2.5 for altitude-assist support
- LOLIN(WEMOS) D1 R2 & mini / ESP8266 build target

The Arduino CLI archive used by CI is verified by SHA-256 before execution.

Hardware and flight validation remain separate from CI compilation. A successful compile does not by itself validate arbitrary hardware, modified control logic, or flight behavior.

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

The existing Hardware Reference `v1.0` tag remains immutable. Packaging or metadata improvements belong on `main` or in a later release rather than in a rewritten historical tag.

The GitHub repository, protected release tag, and GitHub Release are the versioned source of truth for release provenance and licensing. External editing or mirror platforms do not replace the tagged repository license and notices.

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

Before a future public release, actively maintained release repositories should have a working confidential vulnerability-reporting route documented in `SECURITY.md`.

Sensitive vulnerability details must not be requested in public issues.

## Branch governance

All six ESPFlight default `main` branches are protected by active repository rulesets.

The current enforced baseline is:

- block force pushes;
- block branch deletion;
- require the Firmware compile status check on `espflight/firmware`;
- keep bypass privileges absent or deliberately limited;
- protect version tags separately in the release-bearing repositories.

Blanket pull-request enforcement is **not** currently enabled across the organization.

For safety-critical and release-critical work, a dedicated branch plus pull request is the preferred workflow because it exposes the relevant diff and allows required checks to complete before integration. Organization-wide mandatory PR enforcement may be enabled later if ESPFlight adopts a stricter multi-contributor review model.

These settings are repository administration controls and must be configured in GitHub settings when a connected integration does not expose the required administration APIs.
