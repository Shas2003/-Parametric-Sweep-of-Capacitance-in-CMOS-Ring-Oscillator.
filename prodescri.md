#  CMOS Ring Oscillator Using 90nm Technology

This project focuses on the design, implementation, and simulation of a high-speed CMOS ring oscillator using 90nm CMOS technology. Ring oscillators are widely used in integrated circuit (IC) design for clock generation, delay characterization, and process variation monitoring. This design explores the influence of transistor sizing, supply voltage, and stage count on the oscillation frequency and waveform behavior.

---

##  Project Description

A **5-stage CMOS ring oscillator** was designed using standard digital design principles. Ring oscillators are formed by connecting an odd number of inverters in a closed loop, allowing the signal to continuously propagate and regenerate without external input. Each stage introduces a delay, and the overall loop delay determines the oscillation frequency.

In this design:
- An **odd number of inverter stages (5)** ensures oscillation.
- Each inverter was built using **CMOS logic**, with appropriately sized NMOS and PMOS transistors for balanced performance.
- A **DC supply voltage of 1.2 V** was used to align with 90nm CMOS technology standards.
- A **buffer inverter** was added at the output to minimize loading effects and ensure clean waveform observation.

---

##  Technical Specifications

| Parameter                | Value                             |
|--------------------------|-----------------------------------|
| **Technology Node**      | 90nm CMOS                         |
| **Number of Stages**     | 5 (odd number → oscillation)      |
| **NMOS Sizing**          | W = 1.5 µm, L = 0.1 µm            |
| **PMOS Sizing**          | W = 3.0 µm, L = 0.1 µm            |
| **V<sub>DD</sub> (Supply Voltage)** | 1.2 V                   |
| **Expected Frequency**   | ~10–100+ MHz (depending on load)  |
| **Output Swing**         | Full rail-to-rail (~0 V to 1.2 V) |
| **Simulation Type**      | Transient Analysis                |
| **Simulation Tool**      | [e.g., Cadence Virtuoso] |

---

##  Simulation Outcome

- The circuit successfully exhibited stable periodic oscillations, confirming the design's functionality.
- The output waveform showed clean, near rail-to-rail transitions.
- The frequency of oscillation was derived from the measured waveform period and aligned with expectations based on inverter delay and stage count.
- Simulation time step was optimized (≤ 100 ps) to capture rapid transitions and accurate waveform dynamics.

---

##  Applications

-  On-chip clock generation
-  Performance benchmarking of standard cells
-  Delay and timing analysis
-  Process-voltage-temperature (PVT) variation monitoring
-  Calibration structures in analog/digital mixed-signal ICs

---

##  References

- **Weste & Harris**, *CMOS VLSI Design: A Circuits and Systems Perspective*
- **Jan M. Rabaey**, *Digital Integrated Circuits: A Design Perspective*
- Technical papers and design manuals provided in 90nm PDK documentation

