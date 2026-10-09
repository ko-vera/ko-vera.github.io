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
- [3rd Yr Capstone](#rd-yr-capstone---autonomous-wall-painting-robot)

[← Back to Home](/)
</nav>

<div class="toc-content" markdown="1">
  
# ⚡ Electrical Work

## Sarcomere Dynamics
Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home), a robotic hands startup (Jan 2026 - Aug 2026)

#### Power Management Board Redesign
- The boost IC on our original power management board burned out during testing. After a month of chasing switching noise on RoboCup power boards ([below](#ubc-thunderbots)), I knew where to look first and traced the likely cause to a large switching loop.
- Redesigned the board in two weeks, from schematic and component selection to PCB layout in Altium: an 11.1V input to 5V (Raspberry Pi) and 24V (Sarcomere grippers) outputs for a portable demo unit.
- Tightened the switching loop through MOSFET placement, chose capacitors using datasheet DC bias curves so they hold their capacitance at operating voltage, and sized trace widths and via counts per IPC-2221 for the 7A/3A outputs.

#### Artus Dex - New Product Bring-Up & Validation Testing

- **Bring-up:** brought up and flashed newly assembled motor driver/encoder boards (STM32CubeIDE), resolving failures on 15+ boards and CAN bus faults with oscilloscope probing and reflow/substitution testing.
- **Test jig:** designed the wrist/finger validation jig (built with the mechanical team), integrating a load cell, thermistors, CAN motor drivers, and a programmable power supply over MODBUS RTU/RS485 and CAN. Automated Python tests ran across 5 wrist loads (100–500 g), remotely and overnight.
- **Fixes:** ranged from replacing a breadboard that was dropping CAN messages with a soldered board and sturdier mount, to calibrating the encoders across the full range of motion and tuning the controls for uneven tendon tension.
- **Result:** quantified hand's movement accuracy and force output, implemented impedance control so the wrist and fingers yield to external contact and return to position, critical for safe human-robot interaction.

#### Artus Lite - Firmware & User API Refactor
- Refactored the Artus Lite's communication architecture in C/C++ firmware and the Python user API, replacing a proprietary raw-byte command format with MODBUS across UART, RS485, and Wi-Fi TCP to match the rest of the gripper line.
- Used FreeRTOS to run three concurrent tasks with SPI mutex locking, and built a state machine that saves calibration data and the last grasp position to an SD card so the hand restores itself after power loss.
- Added firmware updates through the user API, so actuator boards no longer need to be physically connected for field updates.

<img src="/assets/SARC - ARTUSLITE.png" width="300" alt="Artus Lite robotic hand">


## UBC Thunderbots
Electrical Team Member at [UBC Thunderbots](https://www.ubcthunderbots.ca/) Design Team (Sept 2024 - July 2026)

#### RoboCup 2026 Competition - Incheon, South Korea
Selected as 1 of 3 members to compete in the Small Size League (SSL) at RoboCup 2026.

- **Debugging:** compared charge and discharge waveforms against the datasheet, probed the controller pins, and chased switching noise that was false-triggering the ICs
- **Fixes:** firmware fault detection to safely discharge the capacitors on failure, getting 6 boards competition-ready, enough to field our full team; supported on-the-fly fixes across the UI, IMU, motor driver, and power boards.
- **Carrying it forward:** the switching noise lessons went straight into my [power board redesign at Sarcomere](#power-management-board-redesign).

<img src="/assets/TBOTS - DEBUGGING PT2.jpg" width="355" alt="Debugging power boards at RoboCup 2026"> <img src="/assets/TBOTS - DEBUGGING.jpg" width="355" alt="Team workstations at RoboCup 2026">
<img src="/assets/TBOTS - RoboCup Field.jpg" width="355" alt="RoboCup SSL field"> <img src="/assets/TBOTS - ROBOT.jpg" width="266" alt="UBC Thunderbots robot on the field">

#### Kick Speed Tester - Altium Schematic & Layout
- Led the schematic, component selection, and PCB layout in Altium for a kick speed tester, with ESP32 auto-flash circuitry for programming over USB.
- The tester is an arch with two beams created by two emitters and two phototransistors. When the ball passes through the arch, it breaks the beams, and the time between the two breaks gives the kick speed.

<img src="/assets/kickspeed_circuit_schem.png" width="355" alt="Kick speed tester schematic"> <img src="/assets/kickspeed_arch_cad.png" width="356" alt="Kick speed tester arch CAD">

<img src="/assets/kickspeed_pcb_2D.png" width="365" alt="Kick speed tester PCB layout"> <img src="/assets/kickspeed_pcb_3D.png" width="350" alt="Kick speed tester PCB 3D view">

#### Motor Dynamometer
- Co-designed a custom dynamometer (load cell, amplifier, ESP32) to characterize motor performance under load, measuring force against phase current, and wrote Python scripts for real-time data logging, plotting, and analysis.

#### Other Board Work
- Power Board - Helped with testing and troubleshooting the board, updated the layout with new components, fixed trace connections, and added via stitching
- UI Board - Updated ribbon cable pin order to match the Motor Driver board, updated connections to the Raspberry Pi, fixed trace connections, and worked with MECH to choose mounting locations for the UI and Motor Driver boards
- Soldered components onto Power, UI, Motor Driver, and IMU boards

<img src="/assets/UI BOARD LAYOUT.png" width="355" alt="UI board layout"> <img src="/assets/UI BOARD 3D VIEW.png" width="355.8" alt="UI board 3D view">

## 3rd Yr Capstone - Autonomous Wall Painting Robot
Circuitry Design & Software

*(See the [Mechanical Design](/mechanical/#rd-yr-capstone---autonomous-wall-painting-robot) side of this project on the Mechanical page.)*

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

<!-- ---
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
- [3rd Yr Capstone](#rd-yr-capstone---autonomous-wall-painting-robot)

[← Back to Home](/)
</nav>

<div class="toc-content" markdown="1">
  
# ⚡ Electrical Work

## Sarcomere Dynamics
Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home) (Jan 2026 - Aug 2026)

#### Hardware - BMS Circuit Design & PCB
- Redesigned the circuit, specified components, and laid out a PCB for a battery management system (BMS) converting an 11.1V input to 5V (Raspberry Pi) and 24V (grippers in the Sarcomere product line) for a portable demo unit; sized trace widths and via counts per IPC-2221 to meet 7A/3A output requirements, and optimized MOSFET placement to minimize switching loop inductance.

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

## 3rd Yr Capstone - Autonomous Wall Painting Robot
Circuitry Design & Software

*(See the [Mechanical Design](/mechanical/#rd-yr-capstone---autonomous-wall-painting-robot) side of this project on the Mechanical page.)*

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

[← Back to Home](/) · [Mechanical Work →](/mechanical/) -->
