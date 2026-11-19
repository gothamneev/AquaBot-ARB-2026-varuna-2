# AquaBot-ARB-2026 varuna 2

**Autonomous Surface Trash-Collecting & Water Quality Monitoring USV**

An autonomous, zero-metal Unmanned Surface Vehicle (USV) developed for **Robofest Gujarat 6.0 (GUJCOST)** by the Department of Electronics and Communication Engineering, **Government Engineering College, Bharuch**.

![AquaBot ARB-2026 V2 CAD Preview](AquaBot_ARB2026_V2_Preview.png)

AquaBot ARB-2026 combines automated floating debris collection with real-time 6-parameter water quality profiling in lakes, rivers, and urban waterways.

---

## 3D CAD Model (`AquaBot_ARB2026_V2_Pro.stl`)

> **Interactive Preview:** Click on `AquaBot_ARB2026_V2_Pro.stl` in this repository to inspect and rotate the 3D catamaran model directly in GitHub's built-in 3D viewer.

### V2 Catamaran Pro Specifications
| Parameter | Specification |
| :--- | :--- |
| **Overall Dimensions (L × W × H)** | 450.0 × 264.0 × 145.0 mm |
| **Hull Architecture** | Twin-pontoon catamaran (Foam-Core ABS / GFR-PP) |
| **Propulsion** | Dual under-pontoon ducted BLDC thrusters (differential steering) |
| **Collection Mechanism** | Twin-servo articulated Nylon 66 mesh scoop arm |
| **Storage Hopper** | ~0.85 L self-draining slatted HDPE rear bin (120° tilt-dump) |
| **3D Print Recommendation** | PETG or ABS, 4 walls, 20% Gyroid infill, 0.2 mm layer height |

---

## Hardware & Electronics Architecture

* **Controllers:** Teensy 4.1 / Raspberry Pi 4B (high-level vision, navigation & logging) + ESP32-WROOM-32D (low-latency motor/servo control & telemetry)
* **Vision & Navigation:**
  * Raspberry Pi Camera Module v3 Wide (Sony IMX708)
  * u-blox NEO-M8N GPS Module (GNSS Coverage Path Planning)
  * MPU-6050 6-DOF IMU (wave-tilt compensation & roll safety)
  * Waterproof JSN-SR04T / HC-SR04 Ultrasonic Sensors (obstacle avoidance & bin fill level)
* **Water Quality Diagnostic Array:**
  * Atlas Scientific EZO-pH, EZO-DO (Dissolved Oxygen), and EZO-EC (Conductivity/TDS)
  * Turbidity Sensor, DS18B20 Waterproof Temperature Probe, and IR Oil Sheen Sensor (SEN0137)
* **Actuation & Power:**
  * Dual BLDC Motors with 30A BLHeli ESCs
  * High-torque MG996R Servo Motors & DC Gear Motor (BTS7960 Driver)
  * 3S 5000mAh 11.1V LiPo Battery with Power Distribution Board (PDB) and inline fuses

---

## Team — Government Engineering College, Bharuch (GTU)

* **Mentor:** Prof. Priyanka Patel
* **Team Members:**
  * Dandekar Divyansh Manish
  * Shiv Viralkumar Shah
  * Kuril Neev Ajaykumar
  * Sharma Girishkumar Hariom
