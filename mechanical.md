---
title: Mechanical Work
permalink: /mechanical/
---

[← Back to Home](/) · [Electrical Work →](/electrical/)

<style>
.toc-layout {
  display: flex;
  gap: 30px;
  align-items: flex-start;
  margin-top: 20px;
}
.toc-sidebar {
  flex: 0 0 220px;
  position: sticky;
  top: 20px;
  padding: 16px;
  border: 2px solid #2B547E;
  border-radius: 10px;
  background: #f5f9ff;
}
.toc-sidebar p {
  margin: 0 0 10px 0;
  font-weight: bold;
  color: #2B547E;
}
.toc-sidebar ul {
  margin: 0;
  padding-left: 18px;
}
.toc-sidebar li {
  margin-bottom: 8px;
}
.toc-content {
  flex: 1;
  min-width: 0;
}
@media (max-width: 768px) {
  .toc-layout {
    flex-direction: column;
  }
  .toc-sidebar {
    position: static;
    width: 100%;
    flex-basis: auto;
  }
}
</style>

<div class="toc-layout">

<nav class="toc-sidebar" markdown="1">

On this page:
- [Tycrop Manufacturing](#tycrop-manufacturing)
- [UBC Sailbot](#ubc-sailbot)
- [3rd Yr Capstone](#3rd-yr-capstone---autonomous-wall-painting-robot)

[← Back to Home](/)
</nav>

<div class="toc-content" markdown="1">
  
# ⚙️ Mechanical Work

## Tycrop Manufacturing

Mechanical Design Engineering Co-op at [Tycrop](https://tycrop.com/) (May 2025 - Dec 2025)

#### Solidworks CAD Sheet Metal Parts, Weldments, Drawings
- Designed complex SOLIDWORKS CAD models and assemblies for an exhaust/radiator system supporting large-scale natural gas power generation units
- Designed piping, valves, fans, tanks, and mounts using 3D sketching for asymmetrical piping layouts
- Earned CSWA (Certified SOLIDWORKS Associate)
- Developed system designs from customer P&ID and collaborated with the electrical team to integrate piping, instrumentation, and components within space and environmental constraints; developed, modified, and verified drawings for parts, assemblies, and weldments.

#### Material Selection & Design Choices
- Sized HSS beams through structural analysis to provide structural support for the exhaust/radiator system.
- Calculated thermal expansion of large-scale piping runs to inform mounting plate design and gasket/fastener selection, ensuring appropriate pipe movement under load.
- Researched and documented proprietary sound attenuation technology for future patent application, and recommended acoustic insulation materials optimized for thermal, chemical, and weight/thickness constraints.
- Collaborated directly with suppliers and external partner companies to outsource part fabrication, coordinating drawing revisions to align with partner-specific design and documentation standards.


## UBC Sailbot

Rudder Mechanical Team Member at [UBC Sailbot](https://www.ubcsailbot.org/) (Jan 2022 - Sept 2024)

#### Solidworks CAD Parts & Assembly

- Designed motor, shafts, & timing belt as well as compiled assembly

<img src="/assets/SAILBOT - rudderassem.png" width="350"> <img src="/assets/SAILBOT - timing belt.png" width="350">


#### Structural Stress Calculations

- Completed stress calculations to determine minimum diameter of bolts required to avoid shear and tensile failure

<img src="/assets/zxFBD" width="350"> <img src="/assets/zxcalcs.png" width="350">

<img src="/assets/zypic" width="350"> <img src="/assets/zyFBD" width="350"> <img src="/assets/torsional" width="350">

<img src="/assets/zycalcs.png" width="350"> <img src="/assets/zycalcs2.png" width="350"> <img src="/assets/zycalcs3.png" width="350">


#### Integration with ELEC

- Decided on motors and encoders that satisfy the needs of both MECH & ELEC
- Here you can see some minimum torque calculations that we did based on the worm gear we chose in order to spec a motor. This allowed us to determine how frequently our motor would be drawing maximum current and whether that is viable with the amount of power that the ELEC team is accounting for

<img src="/assets/wormgearcalc" width="350"> <img src="/assets/wormgearcalc2" width="350">


## 3rd Yr Capstone - Autonomous Wall Painting Robot

Mechanical Design

*(See the [Circuitry Design & Software](/electrical/#3rd-yr-capstone---autonomous-wall-painting-robot) side of this project on the Electrical page.)*

#### Project Description

- Designed an autonomous robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

<img src="/assets/330 - Picture of Painted Line.jpg" width="350">

#### Mechanical Design

- Designed chassis, wheel and motor mounting, as well as custom wheel flange couples for omni wheel drive using CAD
- Created and iterated sensor mount geometry using CAD to maximize accuracy and consistency of results
- Developed CAD models for the paint dispensing system, including paint platform, rail attachment, and wheel stabilizer
- CAD designed paint applicator attachment and tested various application materials and geometries to achieve clean, consistent lines.

<img src="/assets/330 - Iso View (Sensors + Applicator).jpg" width="350">
<img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="350">

----

[← Back to Home](/) · [Electrical Work →](/electrical/)
