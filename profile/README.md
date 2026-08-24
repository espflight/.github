# ESPFlight

### Open flight platform for ESP-based drones

**ESPFlight is not a drone brand. It is the platform behind drone brands.**

**Build it. Brand it. Sell it.**

ESPFlight is a flight-control platform and ecosystem designed for makers, developers, small manufacturers, and companies that want to build their own ESP-based drone products without starting every layer from zero.

The platform brings together open flight-controller firmware, an open hardware reference, a companion application, a documented communication layer, and practical documentation — while leaving the final product, hardware identity, brand, pricing, and customer relationship in the hands of the maker.

> Open platform. Independent products. Shared growth.

---

## What ESPFlight provides

| Layer | Role | Model |
| --- | --- | --- |
| **ESPFlight Firmware** | Flight control, stabilization, safety state, telemetry, configuration, and device-side communication | **Open source — MPL-2.0** |
| **ESPFlight Hardware Reference** | A known starting point for compatible flight-controller hardware | **Open hardware — CERN-OHL-W-2.0** |
| **ESPFlight Application** | The official companion experience for control, telemetry, setup, and tuning | **Free to use — closed source** |
| **ESPFlight Protocol & Documentation** | The shared contract that helps compatible hardware and software work together | **Documented platform interface** |

ESPFlight is intended to be a reusable foundation, not a fixed product design.

---

## Build your own product

A maker or company can start from ESPFlight, adapt the hardware to a different size or layout, integrate it into a new drone, manufacture the result, and sell that product under its **own brand**.

For example:

```text
SkyMaker Mini
Compatible with ESPFlight
```

The product remains a **SkyMaker** product. ESPFlight is the technology platform underneath it.

Subject to the applicable open-source and open-hardware license terms, independent makers may:

- use ESPFlight for personal or commercial projects;
- modify the open firmware and hardware reference;
- manufacture compatible hardware;
- create their own product form factor and design;
- sell products built on the platform;
- use their own brand, packaging, pricing, and sales channels.

A maker does **not** need to become an ESPFlight Partner simply to build or sell an independent product using the open components according to their licenses.

---

## No official ESPFlight kit

ESPFlight itself is **not intended to manufacture or sell an “Official ESPFlight Kit” or an “Official ESPFlight Hardware” product line**.

The goal is for ESPFlight to remain neutral infrastructure for independent hardware brands rather than competing with those brands as a hardware manufacturer.

Even if the founder of ESPFlight produces hardware through a separate brand, that hardware brand remains an **independent manufacturer on the ESPFlight platform**. It does not become “Official ESPFlight Hardware” merely because of common ownership or founder involvement.

---

## The official application

The **ESPFlight Application** provides a common companion experience across compatible ESPFlight-based drones.

The application is intended to cover the everyday platform experience, including areas such as:

- flight control;
- connection and flight-state feedback;
- telemetry;
- configuration;
- PID tuning;
- supported assisted-flight functions;
- future device identity and ecosystem features.

The application is **free to use and closed source**, separate from the open firmware and hardware licenses.

The long-term model is to keep the essential flight experience accessible while allowing optional advanced software features and services to support continued platform development.

ESPFlight aims to make the official application the **best and easiest experience**, not to make openness depend on application lock-in.

---

## Independent products and ESPFlight branding

Open technology and brand rights are intentionally separate.

Independent products can accurately describe their relationship with ESPFlight using wording such as:

- **Compatible with ESPFlight**
- **Based on ESPFlight**
- **Built with ESPFlight**
- **Works with ESPFlight Application**

These descriptions must be truthful and must not imply certification, endorsement, partnership, or official status that has not been granted.

The following are reserved for specifically authorized relationships under the ESPFlight Brand Policy:

- **Powered by ESPFlight**
- **ESPFlight Partner**
- official Partner badges or certification-style marks
- use of the ESPFlight logo in ways that imply official product status or endorsement

Read the full **ESPFlight Trademark & Brand Policy** at:

**https://espflight.com/brand-policy/**

---

## Optional Partner Program

The ESPFlight Partner Program is designed for makers and manufacturers who want a **closer commercial relationship** with the platform.

Partnership is optional. It is a benefit — not permission to use the open platform.

Depending on the published Partner terms, authorized Partners may receive benefits such as:

- closer compatibility guidance;
- product-level technical communication;
- ecosystem visibility;
- Partner recognition;
- launch or directory opportunities;
- authorized use of specific ESPFlight Partner branding.

Independent building and selling remain available without Partner status under the applicable licenses.

---

## Licensing

### Firmware

ESPFlight Firmware is licensed under the **Mozilla Public License 2.0 (MPL-2.0)**.

This allows commercial use, modification, and redistribution subject to the terms of the license. MPL-covered files and modifications to those files remain subject to MPL-2.0 when distributed.

Full license and ESPFlight summary:

**https://espflight.com/licenses/firmware/**

### Hardware

The ESPFlight Hardware Reference is licensed under **CERN Open Hardware Licence Version 2 — Weakly Reciprocal (CERN-OHL-W-2.0)**.

This allows makers and companies to study, modify, manufacture, and commercially use the covered hardware design subject to the terms of the license.

Full license and ESPFlight summary:

**https://espflight.com/licenses/hardware/**

### Brand

The firmware and hardware licenses do **not** grant unrestricted rights to the ESPFlight name, logo, Partner marks, or reserved relationship wording.

Brand use is governed separately by the:

**ESPFlight Trademark & Brand Policy**  
https://espflight.com/brand-policy/

If a summary in this README conflicts with an applicable license, the full license text controls.

---

## Platform philosophy

ESPFlight is built around a simple idea:

> The shared technology should be open enough for other people to build real products on top of it, while each maker remains free to create a distinct product and business of their own.

A healthy ESPFlight ecosystem looks like this:

```text
ESPFlight platform
      ↓
Independent makers and companies
      ↓
Different boards, drones, products, and brands
      ↓
More compatible devices and users
      ↓
A stronger application, community, and ecosystem
      ↓
More development flowing back into the platform
```

Success is not every drone carrying the ESPFlight name.

Success is many independent products being able to say, accurately:

**Compatible with ESPFlight.**

---

## Project principles

### Platform first

Build reusable infrastructure instead of one locked hardware product.

### Open at the foundation

Keep the flight-controller firmware and reference hardware inspectable, adaptable, and commercially usable under their published licenses.

### Independent brands

The name on the product belongs to the maker who designed, manufactured, and sells it.

### Compatibility without lock-in

Provide a coherent official experience while keeping the platform architecture understandable and extensible.

### Safety before claims

Flight-critical behavior should be tested on real hardware before being described as stable or production-ready.

### Honest project status

Experimental, incomplete, tested, and stable functionality should be identified clearly as the platform evolves.

---

## Project status

ESPFlight is under active development and is being prepared as a public platform.

Firmware, hardware-reference resources, documentation, application downloads, and ecosystem links will be published through the ESPFlight website and GitHub organization as each component is ready for public use.

For the latest public information, visit:

- **Website:** https://espflight.com
- **GitHub:** https://github.com/ESPFlight
- **Documentation:** https://espflight.com/docs/

---

## Safety

ESPFlight controls real motors and flying hardware. Incorrect configuration, hardware faults, software defects, radio/network loss, battery problems, or improper testing can cause injury or property damage.

Always test new hardware and firmware cautiously, keep propellers removed during bench testing where appropriate, verify failsafe behavior, and follow applicable local laws and safety requirements.

Do not treat experimental functionality as production-ready unless it has been validated for your specific hardware and use case.

---

## Contributing

As the public repositories are released, contributions may include:

- firmware improvements;
- hardware-reference improvements;
- documentation;
- bug reports;
- compatibility testing;
- protocol feedback;
- examples and educational material.

Repository-specific contribution instructions will live with each project.

---

## ESPFlight

**Build it. Brand it. Sell it.**  
**Open platform. Independent products. Shared growth.**

https://espflight.com
