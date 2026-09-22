---
title: Electrical Work
permalink: /electrical/
---

[← Back to Home](/) · [Mechanical Work →](/mechanical/)

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
  border-radius: 7px;
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
- [Sarcomere Dynamics](#sarcomere-dynamics)
- [UBC Thunderbots](#ubc-thunderbots)
- [Autonomous Wall Painting Robot](#autonomous-wall-painting-robot)

[← Back to Home](/)
</nav>

<div class="toc-content" markdown="1">
  
# ⚡ Electrical Work

## Sarcomere Dynamics
Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home) (Jan 2026 - Aug 2026)

#### Hardware - BMS Circuit Design & PCB
- Designed the circuit, specified components, and laid out a PCB for a battery management system (BMS) converting an 11.1V input to 5V (Raspberry Pi) and 24V (grippers in the Sarcomere product line) for a portable demo unit; sized trace widths and via counts per IPC-2221 to meet 7A/3A output requirements, and optimized MOSFET placement to minimize switching loop inductance.

#### Firmware & Software - Artus Lite Firmware & User API Refactoring
- Led refactoring of communication architecture in C/C++ for the Artus Lite robotic hand, including MODBUS slave implementation (command parsing, register mapping, response frame generation) to improve modularity and standardize with the broader robotic gripper codebase.
- Reworked the Python user API’s MODBUS master implementation to align with the refactored slave-side protocol and standardize communication across the gripper product line, including support for communication across UART, RS485, and Wi-Fi TCP to ensure reliable end-to-end communication.
- Used FreeRTOS to manage inter-task communication across three concurrent tasks, including system scheduling and SPI mutex locking/blocking for resource management.
- Built a state machine to manage SD card read/write operations for storing actuator calibration data (end stops & range of motion) as well as last known grasp position, enabling the hand to restore to a known state after power loss.
- Developed functionality for firmware to be pushed through the user API, removing the need to physically connect individual actuator boards for field updates.
- Performed system-level debugging and integration between legacy and refactored architectures, ensuring compatibility and reliable operation.

<img src="/assets/SARC - ARTUSLITE.png" width="300">

#### Testing - Artus Dex - New Product Bring Up & Driving Control
- The Artus Dex is an upcoming product which highlights motorized driving for the opening of the fingers.
- Tested and tuned control for Artus Dex robotic fingers and wrist through PID tuning and Python scripting; board bring up; diagnosed firmware, software, and hardware issues using data trend analysis, mechanical failure mode analysis, and oscilloscope inspection of CANBUS signals.
- Implemented impedance control so the wrist and fingers yield to external interference and return to position – critical for safe human-robot interaction.
  


## UBC Thunderbots
Electrical Team Member at [UBC Thunderbots](https://www.ubcthunderbots.ca/) Design Team (Sept 2024 - July 2026)

#### RoboCup 2026 Competition - Incheon, South Korea

- Selected as 1 of 3 members to compete in the SSL division at RoboCup 2026
- Conducted extensive high-voltage testing (240V capacitors, flyback converter) for the robot's kicking mechanism; diagnosing and resolving PCBA and chip failures via PCB and firmware modifications - restoring 6 power boards to be competition-ready.
- Supported with making design-phase modifications and on-site, on the fly adjustments across UI, IMU, motor driver, and power boards to ensure competition readiness.

<img src="/assets/TBOTS - DEBUGGING PT2.jpg" width="355"> <img src="/assets/TBOTS - DEBUGGING.jpg" width="355">
<img src="/assets/TBOTS - RoboCup Field.jpg" width="355"> <img src="/assets/TBOTS - ROBOT.jpg" width="266">

#### Kick Speed Tester - Altium Circuit Schematic & Layout

- Completed the circuit schematic for a kickspeed tester and am currently working on the PCB board layout for the phototransistor side of the kick speed tester arch shown below
- Kick speed tester contains two beams created by two emitters and two transistors. When the ball passes through the arch, the beams are broken and the time between them being broken is measured.


<img src="/assets/kickspeed_circuit_schem.png" width="355"> <img src="/assets/kickspeed_arch_cad.png" width="356">

<img src="/assets/kickspeed_pcb_2D.png" width="365"> <img src="/assets/kickspeed_pcb_3D.png" width="350">

#### Various Projects

- Power Board - Helped with testing and troubleshooting board, updated board layout with new components, fixed trace connections, via stitching
- UI board - Updated ribbon cable pin order to match with Motor Driver board, updated connections to Raspberry Pi, fixed trace connections, integrated with MECH to determine best location for board placement/mounting of UI and Motor Driver boards
- Soldering various components onto Power, UI, Motor Driver, and IMU boards

<img src="/assets/UI BOARD LAYOUT.png" width="355"> <img src="/assets/UI BOARD 3D VIEW.png" width="355.8">

## Autonomous Wall Painting Robot
3rd Yr Capstone - Circuitry Design & Software

*(See the [Mechanical Design](/mechanical/#capstone-autonomous-wall-painting-robot) side of this project on the Mechanical page.)*

#### Project Description

- Designed an autonomous robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

<video src="/assets/330 - Wall Painting Robot Video.mp4" width="300" controls></video>
<img src="/assets/330 - Picture of Painted Line.jpg" width="350">

#### Circuitry Design & Software

- Surface mount and through hole soldering of components
- Wiring and troubleshooting of electrical components including Raspberry Pi Pico, Arduino Mega, H-bridges, Lithium ion battery, Time-of-Flight (ToF) sensor, and limit switches
- Integrated motors with H-bridges and conducted extensive robot drive testing
- Wrote code for driving with omni wheels - troubleshooting motor driving, force distribution of driving against the wall, motor stalling
- Supported design and implementation of linear actuators and limit switches for vertical and horizontal positioning as well as motor driving for consistent paint dispensing

<img src="/assets/330 - circuit schematic.png" width="350"><img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="350">


----

[← Back to Home](/) · [Mechanical Work →](/mechanical/)
