# Mass Budget — Icarus-Rocket v1

## Structure
| Component                  | Mass (g) | Source           |
|----------------------------|----------|------------------|
| Airframe (upper stage)     | 350      | CAD estimate     |
| Airframe (lower stage)     | 400      | CAD estimate     |
| Coupler                     | 80       | CAD estimate     |
| Nose cone                   | 200      | CAD estimate     |
| Landing legs (4x)          | 240      | CAD estimate     |
| **Subtotal Structure**     | **1270** |                  |

## Propulsion
| Component                  | Mass (g) | Source           |
|----------------------------|----------|------------------|
| Motor (loaded)             | 800      | Manufacturer spec|
| Motor mount + retainer     | 100      | CAD estimate     |
| **Subtotal Propulsion**    | **900**  |                  |

## Avionics
| Component                  | Mass (g) | Source           |
|----------------------------|----------|------------------|
| Flight computer            | 25       | TBD              |
| IMU                        | 5        | TBD              |
| Barometer                  | 3        | TBD              |
| GPS                        | 15       | TBD              |
| Radio + antenna            | 30       | TBD              |
| Battery (LiPo 3S 1500mAh)  | 130      | TBD              |
| Wiring + connectors        | 50       | Estimate         |
| **Subtotal Avionics**      | **258**  |                  |

## Recovery
| Component                  | Mass (g) | Source           |
|----------------------------|----------|------------------|
| TVC gimbal + servos (2x)   | 90       | CAD estimate     |
| Airbrake servos (3x)       | 60       | CAD estimate     |
| Airbrake panels            | 120      | CAD estimate     |
| **Subtotal Recovery**      | **270**  |                  |

## Payload / Misc
| Component                  | Mass (g) | Source           |
|----------------------------|----------|------------------|
| Parachute (backup)         | 50       | TBD              |
| Misc hardware              | 100      | Estimate         |
| **Subtotal Misc**          | **150**  |                  |

---

## **TOTAL ESTIMATED MASS: ~2,850 g (2.85 kg)**

### Margin
Add **20% margin** for unknown components: **~3.4 kg final estimate**

### FAA Class Check
- Class 1: ≤ 1500 g propellant, ≤ 320 N·s impulse, ≤ 4 oz (113 g) recovery charge
- Class 2: any of the above exceeded but still safe
- Class 3: requires certification
- **Decision:** Target Class 2 for development, well under Part 101 limits
