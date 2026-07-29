# Mission Requirements — Icarus-Rocket v1

## 1. Primary Mission
Execute a successful flight to 1,000 m AGL, followed by a controlled 
propulsive vertical landing with target landing velocity of <3 m/s.

## 2. Performance Requirements

| ID    | Requirement                              | Target   | Notes                   |
|-------|----------------------------------------|----------|---------------------------|
| MR-01 | Apogee altitude                        | 1,000 m  | ±100 m                    |
| MR-02 | Drogue velocity                        | ~ 15 m/s | Drogue will be cutoff     |
| MR-03 | Touchdown velocity                     | < 3 m/s  | Legs built for 6 m/s      |
| MR-04 | Maximum tilt angle at touchdown        | < 15°    |                           |
| MR-04 | Maximum Flight Time                    | < 90 s   |                           |

## 3. Vehicle Requirements

| ID    | Requirement                          | Target       | Notes                       |
|-------|--------------------------------------|--------------|-----------------------------|
| VR-01 | Gross liftoff weight (GLOW)         | < 5 kg       | FAA Part 101 Class 2 limit  |
| VR-02 | Thrust-to-weight ratio (ascent)     | > 5:1        | For clean ascent            |
| VR-03 | Thrust-to-weight ratio (landing)    | > 2:1        | For hover/landing control   |
| VR-04 | Airframe diameter                   | <=100 mm     | Standard 4" tubing          |
| VR-05 | Total impulse                       | Class H-equiv| ~640 N·s                    |

## 4. Recovery Requirements

| ID    | Requirement                          | Target   | Notes                                          |
|-------|--------------------------------------|----------|------------------------------------------------|
| RR-01 | Recovery system type                 | Propulsive landing | DC Motor Testing, Solid Fuel Final   |
| RR-02 | Landing legs                         | 4x deployable | Carbon fiber/aluminum                     |
| RR-03 | TVC authority                        | ±8° pitch/yaw |                                           |


## 5. Avionics Requirements

| ID    | Requirement                          | Target         | Notes                  |
|-------|--------------------------------------|----------------|------------------------|
| AR-01 | Flight computer processor            | ARM Cortex-M7  | STM32H7 or equivalent  |
| AR-02 | IMU                                  | 6-axis, ≥1 kHz | For state estimation   |
| AR-03 | Barometric altitude resolution       | < 0.5 m        |                        |
| AR-04 | GPS update rate                      | ≥ 10 Hz        | For navigation         |
| AR-05 | Datalog rate                         | ≥ 100 Hz       | Black box logging      |
| AR-06 | Radio telemetry                      | Required       | Live downlink to GS    |

## 6. Safety & Regulatory

- Comply with **FAA Part 101** (Class 1 or 2 model rocket)
- Launch from approved site with proper waivers
- Maintain ignition control at all times
- Recovery system must be tested before any flight > 500 m

## 7. Verification Plan
Each MR/VR/AR/RR requirement will be verified by:
- **Analysis** (simulation, math)
- **Test** (sub-scale flight, static fire, drop test)
- **Inspection** (CAD review, mass measurement)

## 8. Open Questions
- Final motor selection (DC motor for testing) 
- Optimal control law for landing burn (PID vs. LQR vs. MPC)
- Sensor placement and vibration isolation strategy
