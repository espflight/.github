# ESPFlight GitHub Administration Hardening

This file records repository-administration controls that cannot be enforced by repository content alone and documents the current hardening baseline.

## Current status — 2026-10-02

The following hardening state is now established:

- active default-branch rulesets on all six ESPFlight repositories;
- branch deletion blocked;
- force pushes blocked;
- Firmware configured with its required compile status check;
- release-tag rulesets active on Firmware, Hardware Reference, and Application for tags matching `v*`;
- release-tag deletion, update, and non-fast-forward changes blocked with no bypass actors;
- release immutability enabled for future Firmware, Hardware Reference, and Application GitHub Releases, per maintainer confirmation;
- GitHub Private Vulnerability Reporting enabled for Firmware, Application, and Hardware Reference, per maintainer confirmation;
- the misleading `esp32` topic removed from `espflight/firmware`;
- SSH commit and annotated-tag signing configured for the release maintainer;
- a test SSH-signed commit verified successfully by GitHub;
- a test SSH-signed annotated tag verified successfully by GitHub;
- temporary signing-test refs removed after verification;
- the editable EasyEDA source snapshot preserved under `hardware/design/`;
- the EasyEDA `R13` PCB component metadata corrected on `main` without changing the authoritative v1.0 Gerber, BOM, or Pick-and-Place fabrication baseline.

Ruleset state above was read back through the GitHub API where the connector exposes it. Administration settings that are not exposed through the connector remain recorded from maintainer confirmation.

## Default-branch protection baseline

The protected repositories are:

- `espflight/firmware`
- `espflight/hardware`
- `espflight/docs`
- `espflight/application`
- `espflight/espflight`
- `espflight/.github`

Current enforced minimum:

- block force pushes;
- block branch deletion;
- require the applicable Firmware CI status check on `espflight/firmware`;
- keep bypass privileges absent or intentionally limited.

Pull-request enforcement for all changes is not currently part of the v1.0 baseline. It may be enabled later if ESPFlight adopts a stricter multi-contributor review workflow.

## Release tag protection

Active tag rulesets exist on:

- `espflight/firmware`
- `espflight/hardware`
- `espflight/application`

They target:

`refs/tags/v*`

The enforced rules are:

- deletion blocked;
- update blocked;
- non-fast-forward changes blocked;
- no bypass actors.

Creation is intentionally allowed so new signed release tags can be created. Once a matching version tag exists, it is protected from later mutation.

## Release immutability

The maintainer confirmed that release immutability is enabled for future releases in:

- Firmware
- Hardware Reference
- Application

This setting applies to future release publication behavior. Historical v1.0 / v1.0.0 releases are not rewritten merely to retrofit newer release-protection features.

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

The current `main` branch preserves the editable EasyEDA source at:

`hardware/design/ESPFlight_Hardware_Reference_v1.0_EasyEDA_Source.zip`

On 2026-10-02 the PCB metadata for `R13` inside that editable snapshot was corrected to match the authoritative v1.0 BOM. The PCB geometry, routing, schematic, and official v1.0 fabrication files were not replaced.

The published `v1.0` tag remains immutable and was not rewritten.

Future Hardware Reference releases must include the corresponding editable source snapshot as part of the release baseline before publication.

## Administration note

Branch rulesets, tag rulesets, repository topics, private vulnerability reporting, release immutability, and signing-key configuration are GitHub administration/account controls. They are not activated merely by committing YAML or Markdown files.

When these settings change in the future, update this file so the documented governance baseline matches the actual GitHub configuration.
