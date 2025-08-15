<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/images/visorbearer-heading-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="docs/images/visorbearer-heading-light.png">
  <img alt="Visorbearer Title and Description" src="docs/images/visorbearer-heading-dark.png">
</picture>

## Design

- 32-key Hummingbird-ish layout with splay and inverted thumb cluster
- Discreet 2x 4-segment RGB LED indicators
   - Connection bar: Bluetooth profiles and modifier keys
   - Battery bar: percentage and charging status
   - Powered by two TI LP5012 drivers with low-power mode
- Hot-swap Kailh Choc v1 switches in Choc (18x17mm) spacing
   - <details> <summary>Limited support for Choc v2</summary>
      The PCB is not compatible with earlier Choc v2 switches that have an extra third stabilizing pin. Some recent releases that omit the third pin are compatible, including but not limited to: Lofree POM Phantom/Ghost/Specter/Hades, Kailh Hide Mountain/White Rain/Deep Sea Mini Islet/Deep Sea Mini Whale. Additionally, there are no choc-spaced but MX-stemmed keycaps available off the shelf, so you will need to 3D print keycaps for Choc v2.
   </details>
- Seeed Studio XIAO nRF52840 **Plus** controller on ZMK firmware
- 3D-printed case and switch plate with switch puller grooves

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/images/visorbearer-dimensions-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="docs/images/visorbearer-dimensions-light.png">
  <img alt="Visorbearer keyboard dimensions" src="docs/images/visorbearer-dimensions-dark.png">
</picture>

## Build Guide

> [!WARNING]
> Revision 2 PCB has not been tested yet.


## Acknowledgments

- Aesthetics
   - [GEIGEIGEIST/TOTEM](https://github.com/GEIGEIGEIST/TOTEM)
   - [weteor/Grumpy](https://github.com/weteor/Grumpy)
- Layout
   - [bennytrouser/NostrumX](https://github.com/bennytrouser/NostrumX)
   - [davidphilipbarr/hypergolic](https://github.com/davidphilipbarr/hypergolic)
   - [davidphilipbarr/paroxysm](https://github.com/davidphilipbarr/paroxysm)
   - [hazels-garage/bad-wings](https://github.com/hazels-garage/bad-wings/tree/master/v2)
- LED indicator
   - [GEIGEIGEIST/KLOTZ](https://github.com/GEIGEIGEIST/KLOTZ)
   - [caksoylar/zmk-rgbled-widget](https://github.com/caksoylar/zmk-rgbled-widget): LED code
- Case
   - [duckyb/urchin](https://github.com/duckyb/urchin): Snap fit design
- And the lovely folks on the Fingerpunch discord who were along for the ride!