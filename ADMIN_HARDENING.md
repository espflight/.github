# ESPFlight GitHub Administration Hardening

This file records repository-administration settings that cannot be enforced by repository content alone.

It is intended to keep the target configuration explicit and auditable.

## Default-branch protection

Apply a repository ruleset or branch-protection rule to `main` for:

- `espflight/firmware`
- `espflight/hardware`
- `espflight/docs`
- `espflight/application`
- `espflight/espflight`
- `espflight/.github`

Minimum baseline:

- block force pushes;
- block branch deletion;
- require pull requests for release-critical and safety-critical changes;
- require applicable status checks before merge;
- for Firmware, require the `Firmware CI / Compile ESPFlight Firmware v1.0.0 baseline` check;
- keep administrator bypass limited and intentional.

## Private vulnerability reporting

Enable GitHub Private Vulnerability Reporting for actively maintained repositories where GitHub supports it, with highest priority on:

- Firmware
- Application
- Hardware Reference

After enabling it, verify that the repository Security page exposes **Report a vulnerability** and update `SECURITY.md` only if the user-facing wording needs to change.

Do not request exploit details, credentials, signing keys, or flight-control attack steps in a public issue.

## Firmware repository topics

The public v1.0 firmware baseline targets ESP8266 / LOLIN(WEMOS) D1 R2 & mini.

Until an ESP32 target is officially implemented and validated, remove the `esp32` repository topic from `espflight/firmware`.

The `esp8266` topic should remain.

## Signed release identity

Before the next official release:

1. Configure Git commit/tag signing for the release maintainer.
2. Verify a test signed commit appears as **Verified** on GitHub.
3. Create future official release tags as annotated signed tags.
4. Confirm the release commit and tag display as **Verified** before publishing assets.
5. Never store private signing keys or Android keystores in GitHub repositories.

See `RELEASE_PROCESS.md` for the project-wide release sequence.

## Hardware editable-source snapshot

Before the next Hardware Reference baseline, export the native/editable EasyEDA project for that exact revision and commit it under `hardware/design/`.

The original v1.0 source package does not contain such an export, so no reconstructed or guessed file should be substituted for it.

## Reason this file exists

Branch rulesets, repository topics, private vulnerability reporting, and signing-key configuration are GitHub administration/account controls. They are not activated merely by committing YAML or Markdown files and must be changed through GitHub administration surfaces or an integration with explicit administration-write support.
