# AeroChakra CP-REV-A — Cyber-Physical Digital Twins

Interactive real-time physics-informed digital twins for the **AeroChakra CP-REV-A** horizontal-axis cyclorotor propulsion module and the complete 4-module UAV flight architecture.

Developed for the **Pushpak Advanced UAV Propulsion Challenge (Grand Challenge 2 - Stage 1)**.

---

## 🚀 Live Interactive Deployments

- **🌐 Master Digital Twin Portal:**  
  [https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/](https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/)
- **⚙️ Propulsion Module Digital Twin:**  
  [https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/module_twin.html](https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/module_twin.html)
- **🛸 Full UAV Cyber-Physical Digital Twin:**  
  [https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/uav_twin.html](https://krishna1980moorthy-cmyk.github.io/cycloprop-digital-twin/uav_twin.html)

---

## 📊 Key Engineering Parameters (CP-REV-A Baseline)

| Parameter | Specification | Status |
|---|---|---|
| **Hover Thrust** | 10.042 ± 0.082 N continuous | ✅ COMPLIANT (≥ 10.00 N) |
| **All-Up Flying Mass** | 394.16 g (319.91g dry + 74.25g 4S LiPo) | ✅ COMPLIANT (≤ 407.90 g ceiling) |
| **Thrust-to-Weight (T/W)** | 2.598 (Nominal) / 2.779 (Peak Burst) | ✅ COMPLIANT (> 2.500) |
| **Operating Speed** | 2369 RPM (Hover) / 2450 RPM (Burst) | ✅ VERIFIED |
| **Airfoil Profile** | NACA 0015 (c = 35 mm, L = 150 mm) | ✅ COMPLIANT |
| **Thrust Vectoring** | ±90.0° continuous in-plane steering | ✅ COMPLIANT (< 15 ms latency) |
| **Power Consumption** | 149.1 W shaft / 172.5 W electrical | ✅ VERIFIED |

---

## 🛠️ Architecture

1. **Propulsion Module Digital Twin (module_twin.html)**:
   - Discretized Blade-Element Momentum Theory (BEMT) solver with Leishman-Beddoes dynamic stall delay.
   - Symmetrical dual-eccentric vectoring ring kinematics.
   - Forced downwash convective cooling model for Sunnysky V2216 brushless motor.
   - Live 3D/Canvas rendering of the 4-bladed rotor drum and force vectors.

2. **Full UAV Vehicle Digital Twin (uav_twin.html)**:
   - 4-module synchronized aerodynamic interaction and wake coupling.
   - Multi-axis flight control allocation matrix.
   - Real-time telemetry streaming and health monitoring.
