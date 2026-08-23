# 5V Power Module for UAV Avionics

High-efficiency, wide-input 5V DC-DC power module designed for UAV avionics, supporting 3S–12S LiPo battery input using the LT8645SHV-2 synchronous buck converter.

## Overview

Flight-critical avionics — flight controllers, GPS, telemetry modules, and onboard sensors — need clean, stable power regardless of battery state or LiPo cell count. This module was designed to deliver a regulated 5V rail across a wide input range, with protection and monitoring features built in to keep avionics powered reliably through the full flight envelope.

## Key Features

- **Wide input range** — supports 3S–12S LiPo battery configurations
- **High-efficiency conversion** — built around the LT8645SHV-2 synchronous buck converter
- **Reverse-polarity protection** — prevents damage from incorrect battery connection
- **Under-voltage lockout (UVLO)** — disables output below a safe input threshold
- **Soft-start** — controlled ramp-up to avoid inrush current stress
- **Power-good monitoring** — provides a status signal for downstream system health checks
- **Low-EMI, low-ripple layout** — optimized PCB layout to minimize output ripple and electromagnetic interference
- **Thermal optimization** — layout tuned for improved thermal performance under sustained load

## Design Details

| Parameter | Value |
|---|---|
| Input voltage range | 3S–12S LiPo (~11.1V–50.4V) |
| Output voltage | 5V regulated |
| Converter IC | LT8645SHV-2 (synchronous buck) |
| Protection | Reverse-polarity, UVLO, soft-start |
| Monitoring | Power-good signal |
| Target loads | Flight controller, GPS, telemetry, onboard sensors |

## Tools Used

- **KiCad** — schematic capture and PCB layout
- **LTspice** — circuit simulation and power stage verification

## Design Process

1. Schematic capture around the LT8645SHV-2 buck converter topology
2. Component selection for wide input range and target efficiency
3. LTspice simulation to verify power stage behavior, ripple, and transient response
4. PCB layout optimized for low EMI, low output ripple, and thermal performance
5. Protection circuit integration (reverse-polarity, UVLO, soft-start, power-good)

## Repository Contents

```
├── schematics/     # KiCad schematic files
├── pcb/             # KiCad PCB layout files
├── simulation/      # LTspice simulation files
├── gerbers/          # Fabrication-ready Gerber files
└── docs/             # Datasheets, design notes, test results
```

*(Adjust the folder structure above to match what you actually push.)*

## Status

Designed as part of UAV avionics hardware development at TiHAN-IIT Hyderabad.

## Contact

- **Raju Gudala**
- Email: rajugudala730@gmail.com
- LinkedIn: [raju-gudala](https://www.linkedin.com/in/raju-gudala)
- Portfolio: [raju-gudala.github.io](https://raju-gudala.github.io/)
