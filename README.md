# Crossed Linear Guide 3D Printer

[English](./README.md) | [简体中文](./README.zh-CN.md)

A four-motor 3D printer inspired by the Ultimaker 2 linear-guide architecture and rebuilt around a crossed linear guide layout for higher rigidity and stronger material support.

## Overview

This repository shares the mechanical design files for a custom printer that extends the UM2-style motion idea with a more aggressive drive layout:

- Crossed linear guides for improved stiffness and positioning accuracy.
- Four independent motors for stronger motion control.
- Printed structural parts intended for engineering materials such as PA-CF.
- Open project files so the design can be studied, adapted, and improved.

## Important Note

This project is primarily a structure and design reference. You should expect to adjust dimensions, tolerances, electronics, firmware, and assembly details for your own machine and manufacturing constraints.

## Specifications

| Item | Specification |
| --- | --- |
| Structure | Linear-guide UM2-inspired custom design |
| Drive | Four independent motors |
| Recommended filament | PA-CF, print temperature around 320 C |
| Mainboard | Chitu commercial controller board |
| Firmware | Closed-source board firmware |
| Printed parts | Designed around nylon carbon-fiber parts |

## Recommended Materials

- Filament: Fusrock PA-CF
- Nozzle temperature: 320 C
- Yield strength reference: 190 MPa
- Motion parts: crossed linear guides
- Motors: NEMA 17 class steppers
- Controller: Chitu series board

Exact model numbers are not locked down in this repository. Treat them as a starting point and adapt to your own bill of materials.

## Repository Layout

```text
Crossed_linearguide_3Dprinter/
├── README.md
├── README.zh-CN.md
├── LICENSE
├── Picture/       # Project photos
├── Solidworks/    # SolidWorks source parts
├── STL/           # Exported printable STL files
└── Test model/    # Test model assets
```

## Included Assets

- `Picture/`: 5 project photos
- `Solidworks/`: 16 SolidWorks part files
- `STL/`: 17 exported STL files
- `Test model/`: 1 test model

Representative parts include:

- X/Y sliders and cover plates
- Endstop mounts for X, Y, and Z
- Screen enclosure parts
- Extruder and fan-related spacers
- USB mount pieces

## Assembly Outline

1. Print the structural parts, ideally in PA-CF or another strong engineering filament.
2. Assemble the X-axis linear guide and carriage parts.
3. Assemble the Y-axis structure and platform.
4. Install the Z-axis motion system and join the frame.
5. Wire the controller, motors, heaters, screen, and USB.
6. Configure the firmware and calibrate movement plus bed leveling.

## Printing Notes

For PA-CF:

- Nozzle: 320 C
- Bed: 90 to 110 C
- Print speed: 30 to 50 mm/s
- Use a hardened nozzle

For PLA prototyping:

- Nozzle: 200 to 220 C
- Bed: 50 to 60 C
- Print speed: 50 to 80 mm/s

## Project Photos

![Overall printer](./Picture/1.jpg)
*Overall printer view*

![X-axis detail](./Picture/2.jpg)
*X-axis linear-guide structure*

![Y-axis assembly](./Picture/3.jpg)
*Y-axis assembly*

![Z-axis and toolhead](./Picture/4.jpg)
*Z-axis and extruder area*

![Finished build](./Picture/5.jpg)
*Finished machine*

## Demo And Files

- [Demo video on Bilibili](https://www.bilibili.com/video/BV1EB4y197ZR)
- [STL files](./STL)
- [SolidWorks source files](./Solidworks)

## Contributing

Issues, improvements, remixes, and pull requests are welcome.

1. Fork the repository.
2. Create a branch for your change.
3. Commit your updates.
4. Push the branch.
5. Open a pull request.

## License

This project is licensed under the [MIT License](./LICENSE).

## Contact

- GitHub: [@BraveCowNoFear](https://github.com/BraveCowNoFear)
- Bilibili: [Project demo video](https://www.bilibili.com/video/BV1EB4y197ZR)

If this repository helps your build, a star is appreciated.
