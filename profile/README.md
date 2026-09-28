<p align="left">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="tiefer-logo-white.svg">
    <img src="tiefer-logo.svg" alt="Tiefer" width="260">
  </picture>
</p>

### See deeper. AI that runs on the satellite.

Tiefer builds AI software that runs on Earth observation satellites, from Baku, Azerbaijan.

**[tiefer.space](https://tiefer.space)**

Instead of storing every image and sending gigabytes of raw data to the ground hours later, the satellite analyses its own images in orbit. Tiefer filters out cloudy and empty frames, detects events such as wildfires, oil spills, vessels and floods on board, and sends a small alert packet through the first available link.

## How it works

| Stage | What happens on board |
|---|---|
| **Filter** | Every frame is checked for cloud and quality as it is captured. Useless frames are compressed and kept, not sent |
| **Detect** | Computer vision models look for the events that matter |
| **Alert** | A small packet with location, event type, confidence and an image chip goes to the ground |
| **Update** | Models in orbit are replaced or improved with small, signed updates |

On the ground, **Tiefer Lab** trains and tests models in a virtual orbit simulator and on flight-like hardware, and **Tiefer Ground** runs the same models at the ground station.

## Principles

- Nothing is deleted blindly. Filtered frames are kept on board.
- Observed and inferred are always labelled apart, with a confidence value.
- Every model update is signed, versioned and can be rolled back.
- Performance figures are measured and published with their method.
- Tiefer is not used to track individuals. See our [acceptable use policy](https://github.com/tiefer-labs/.github/blob/main/ACCEPTABLE_USE.md).

## Open source

| Repository | What it is | Licence |
|---|---|---|
| [web](https://github.com/tiefer-labs/web) | Our website, written in Go | MPL 2.0 |
| [.github](https://github.com/tiefer-labs/.github) | This profile and our community policies | MPL 2.0 |

A public benchmark repository will follow with our first measured results. The Tiefer name and logo are trademarks and are not covered by the code licence.

## Status

Early stage. We are looking for our first partners: satellite operators, space agencies, integrators and hosted-compute platforms, starting in Azerbaijan and the wider region. Write to us at [hello@tiefer.space](mailto:hello@tiefer.space).

Found a security issue? Please follow our [security policy](https://github.com/tiefer-labs/.github/blob/main/SECURITY.md).
