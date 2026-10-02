# ESPFlight GitHub Administration Hardening

This file records repository-administration controls that cannot be enforced by repository content alone and documents the current hardening baseline.

## Current status — 2026-10-02

The maintainer confirmed the following GitHub administration changes were completed manually on 2026-10-02:

- active rulesets on the default `main` branch for all six ESPFlight repositories;
- branch deletion blocked;
- force pushes blocked;
- Firmware configured with its required CI status check;
- GitHub Private Vulnerability Reporting enabled for Firmware, Application, and Hardware Reference;
- the `esp32` topic removed from `espflight/firmware`;
- SSH commit and annotated-tag signing configured for the release maintainer;
- a test signed commit verified successfully by GitHub;
- a test signed annotated tag verified successfully by GitHub;
- the temporary signing-test branch and tag removed after verification;
- the original editable EasyEDA source snapshot for Hardware Reference v1.0 added under `hardware/design/`.

Administration settings above were confirmed by the maintainer because the repository connector does not expose administration-write access for all of these controls.

## Default-branch protection baseline

The protected repositories are:

- `espflight/firmware`
- `espflight/hardware`
- `espflight/docs`
- `espflight/application`
- `espflight/espflight`
- `espflight/.github`

Current minimum baseline:

- block force pushes;
- block branch deletion;
- require the applicable Firmware CI status check on `espflight/firmware`;
- keep bypass privileges limited and intentional.

Pull-request enforcement for all changes is not currently part of the v1.0 baseline. It may be enabled later if ESPFlight adopts a stricter multi-contributor review workflow.

## Private vulnerability reporting

GitHub Private Vulnerability Reporting is enabled, per maintainer confirmation, for:

- Firmware
- Application
- Hardware Reference

`SECURITY.md` remains the public security-policy entry point.

Do not request exploit details, credentials, signing keys, or flight-control attack steps in a public issue.

## Firmware repository topics

The public v1.0 firmware baseline targets ESP8266 / LOLIN(WEMOS) D1 R2 & mini.

The maintainer confirmed that the misleading `esp32` repository topic was removed on 2026-10-02.

The `esp8266` topic should remain until the supported target matrix changes.

## Signed release identity

SSH signing is configured for the release maintainer.

GitHub verification was successfully tested for:

- a signed commit;
- an annotated signed tag.

Future official releases should:

1. use a signed release commit;
2. create an annotated signed release tag;
3. confirm both display as **Verified** on GitHub before publishing release assets;
4. never store private signing keys, passphrases, Android keystores, or other release secrets in GitHub repositories.

See `RELEASE_PROCESS.md` for the project-wide release sequence.

## Hardware editable-source snapshot

The original editable EasyEDA source snapshot for Hardware Reference v1.0 is now preserved on the current `main` branch under:

`hardware/design/ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip`

The published `v1.0` tag remains immutable and was not rewritten.

Future Hardware Reference releases must include the corresponding editable source snapshot as part of the release baseline before publication.

## Administration note

Branch rulesets, repository topics, private vulnerability reporting, and signing-key configuration are GitHub administration/account controls. They are not activated merely by committing YAML or Markdown files.

When these settings change in the future, update this file so the documented governance baseline matches the actual GitHub configuration.
