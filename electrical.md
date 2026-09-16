---
title: Electrical Work
permalink: /electrical/
---

[← Back to Home](/) · [Mechanical Work →](/mechanical/)

# ⚡ Electrical Work

## Sarcomere Dynamics - Electrical Team

Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home) (Jan 2026 - Aug 2026)

## UBC Thunderbots - Electrical Team

Electrical Team Member at [UBC Thunderbots](https://www.ubcthunderbots.ca/) (Sept 2024 - July 2026)

#### RoboCup 2026 Competition - Incheon, South Korea

- Selected as 1 of 3 members to compete in the SSL division at RoboCup 2026
- Conducted extensive high-voltage testing (240V capacitors, flyback converter) for the robot's kicking mechanism; diagnosing and resolving PCBA and chip failures via PCB and firmware modifications - restoring 6 power boards to be competition-ready.
- Supported with making design-phase modifications and on-site, on the fly adjustments across UI, IMU, motor driver, and power boards to ensure competition readiness.

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/TBOTS - DEBUGGING PT2.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/TBOTS - DEBUGGING PT2.jpg>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/TBOTS - DEBUGGING.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/TBOTS - DEBUGGING.jpg>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/TBOTS - RoboCup Field.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/TBOTS - RoboCup Field.jpg>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/TBOTS - ROBOT.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/TBOTS - ROBOT.jpg>)

#### Kick Speed Tester - Altium Circuit Schematic & Layout

- Completed the circuit schematic for a kickspeed tester and am currently working on the PCB board layout for the phototransistor side of the kick speed tester arch shown below
- Kick speed tester contains two beams created by two emitters and two transistors. When the ball passes through the arch, the beams are broken and the time between them being broken is measured.

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/Screenshot 2024-11-12 120847.png)](</ko-vera/ko-vera.github.io/blob/main/assets/Screenshot 2024-11-12 120847.png>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/Screenshot 2025-01-11 225837.png)](</ko-vera/ko-vera.github.io/blob/main/assets/Screenshot 2025-01-11 225837.png>)

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/Screenshot 2025-01-21 205145.png)](</ko-vera/ko-vera.github.io/blob/main/assets/Screenshot 2025-01-21 205145.png>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/Screenshot 2025-01-21 205001.png)](</ko-vera/ko-vera.github.io/blob/main/assets/Screenshot 2025-01-21 205001.png>)

#### Various Projects

- Power Board - Helped with testing and troubleshooting board, updated board layout with new components, fixed trace connections, via stitching
- UI board - Updated ribbon cable pin order to match with Motor Driver board, updated connections to Raspberry Pi, fixed trace connections, integrated with MECH to determine best location for board placement/mounting of UI and Motor Driver boards
- Soldering various components onto Power, UI, Motor Driver, and IMU boards

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/UI BOARD LAYOUT.png)](</ko-vera/ko-vera.github.io/blob/main/assets/UI BOARD LAYOUT.png>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/UI BOARD 3D VIEW.png)](</ko-vera/ko-vera.github.io/blob/main/assets/UI BOARD 3D VIEW.png>)

## IGEN 330 Capstone - Circuitry Design & Software

*(See the [Mechanical Design](/mechanical/#igen-330-capstone---mechanical-design) side of this project on the Mechanical page.)*

#### Project Description

- Designed an autonomous robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Picture of Painted Line.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Picture of Painted Line.jpg>)

#### Circuitry Design & Software

- Surface mount and through hole soldering of components
- Wiring and troubleshooting of electrical components including Raspberry Pi Pico, Arduino Mega, H-bridges, Lithium ion battery, Time-of-Flight (ToF) sensor, and limit switches
- Integrated motors with H-bridges and conducted extensive robot drive testing
- Wrote code for driving with omni wheels - troubleshooting motor driving, force distribution of driving against the wall, motor stalling
- Supported design and implementation of linear actuators and limit switches for vertical and horizontal positioning as well as motor driving for consistent paint dispensing

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - circuit schematic.png)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - circuit schematic.png>)

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Electrical Components on Chassis.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Electrical Components on Chassis.jpg>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg>)

## IGEN 230 Line Following Robot - Individual Project

[![Untitled video - Made with Clipchamp (3)](https://private-user-images.githubusercontent.com/91451073/320383262-81809f06-70ba-4e8b-8c00-bfcb03b5aecc.gif)](https://private-user-images.githubusercontent.com/91451073/320383262-81809f06-70ba-4e8b-8c00-bfcb03b5aecc.gif) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/borottop)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/borottop) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/borotside)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/borotside)

#### Circuitry

- Implemented H-Bridge Board
  * Used H-Bridge to control direction → run motors forwards and backwards - this works by opening and closing the respective switches shown
  * Used PWM to control speed → when the phototransistor sees white (more light) → more current
  * There are two phototransistors on either side of the black line - when it sees white, there is more current & it moves forward, when one of them sees black, it will turn

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/hbridgeboard.png)](/ko-vera/ko-vera.github.io/blob/main/assets/hbridgeboard.png) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/hbridge.png)](/ko-vera/ko-vera.github.io/blob/main/assets/hbridge.png)

#### Coding Process

[Arduino Code](/assets/Line Following Robot Code.txt)

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/flowchart)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/flowchart)

----

[← Back to Home](/) · [Mechanical Work →](/mechanical/)
