
<div style="display: flex; align-items: center; gap: 15px;">
  <img src="assets/HEADSHOT.jpg" 
       alt="Headshot" 
       style="width: 70px; height: 70px; border-radius: 50%; object-fit: cover;">
  <font size="5"><b>4th Year UBC Integrated Engineering Student - Electrical & Mechanical</b></font>
</div>
----
Hi! Welcome to my Project Portfolio. I hope this helps in getting to know my skills a little better :) 

Browse my work by discipline:

<style>
.portfolio-links {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  margin: 30px 0;
}
.portfolio-links a {
  flex: 1;
  min-width: 220px;
  display: block;
  padding: 24px;
  border: 2px solid #2B547E;
  border-radius: 12px;
  text-decoration: none;
  color: #2B547E;
  background: #f5f9ff;
  transition: transform 0.15s ease, box-shadow 0.15s ease;
}
.portfolio-links a:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 14px rgba(0,0,0,0.15);
}
.portfolio-links .card-title {
  display: block;
  font-size: 1.5em;
  font-weight: bold;
  margin: 0 0 8px 0;
}
.portfolio-links p {
  margin: 0;
  color: #333;
}
</style>

<div class="portfolio-links">

<a href="/electrical/">
<span class="card-title">⚡ Electrical Work</span>
<p>Circuit design, PCB layout, firmware, wiring, and testing — Sarcomere Dynamics, UBC Thunderbots, and capstone electronics.</p>
</a>

<a href="/mechanical/">
<span class="card-title">⚙️ Mechanical Work</span>
<p>CAD, structural design, and mechanical integration — Tycrop Manufacturing, UBC Sailbot, and capstone mechanical design.</p>
</a>

</div>

----

### Quick links to teams & employers

**Electrical**
- [Sarcomere Dynamics](https://sarcomeredynamics.com/home) — Electrical Engineering Co-op (Jan 2026 - Aug 2026)
- [UBC Thunderbots](https://www.ubcthunderbots.ca/) — Electrical Team Member (Sept 2024 - July 2026)

**Mechanical**
- [Tycrop](https://tycrop.com/) — Mechanical Design Engineering Co-op (May 2025 - Dec 2025)
- [UBC Sailbot](https://www.ubcsailbot.org/) — Rudder Mechanical Team Member (Jan 2022 - Sept 2024)



<h2 style="color:#4682B4;"> Sarcomere Dynamics - Electrical Team </h2>

Electrical Engineering Co-op at [Sarcomere Dynamics](https://sarcomeredynamics.com/home) (Jan 2026 - Aug 2026)

<h2 style="color:#4682B4;"> UBC Thunderbots - Electrical Team </h2>

Electrical Team Member at [UBC Thunderbots](https://www.ubcthunderbots.ca/) (Sept 2024 - July 2026)
#### RoboCup 2026 Competition - Incheon, South Korea
- Selected as 1 of 3 members to compete in the SSL division at RoboCup 2026
- Conducted extensive high-voltage testing (240V capacitors, flyback converter) for the robot's kicking mechanism; diagnosing and resolving PCBA and chip failures via PCB and firmware modifications - restoring 6 power boards to be competition-ready.
- Supported with making design-phase modifications and on-site, on the fly adjustments across UI, IMU, motor driver, and power boards to ensure competition readiness.

<img src="/assets/TBOTS - DEBUGGING PT2.jpg" width="450"> <img src="/assets/TBOTS - DEBUGGING.jpg" width="450">
<img src="/assets/TBOTS - RoboCup Field.jpg" width="450"> <img src="/assets/TBOTS - ROBOT.jpg" width="337">


#### Kick Speed Tester - Altium Circuit Schematic & Layout
- Completed the circuit schematic for a kickspeed tester and am currently working on the PCB board layout for the phototransistor side of the kick speed tester arch shown below
- Kick speed tester contains two beams created by two emitters and two transistors. When the ball passes through the arch, the beams are broken and the time between them being broken is measured.

<img src="/assets/kickspeed_circuit_schem.png" width="450">
<img src="/assets/Screenshot 2024-11-12 120847.png" width="450"> <img src="/assets/Screenshot 2025-01-11 225837.png" width="450">

<img src="/assets/Screenshot 2025-01-21 205145.png" width="450"> <img src="/assets/Screenshot 2025-01-21 205001.png" width="450">

#### Various Projects
- Power Board - Helped with testing and troubleshooting board, updated board layout with new components, fixed trace connections, via stitching
- UI board - Updated ribbon cable pin order to match with Motor Driver board, updated connections to Raspberry Pi, fixed trace connections, integrated with MECH to determine best location for board placement/mounting of UI and Motor Driver boards
- Soldering various components onto Power, UI, Motor Driver, and IMU boards 

<img src="/assets/UI BOARD LAYOUT.png" width="450"> <img src="/assets/UI BOARD 3D VIEW.png" width="450">

<h2 style="color:#4682B4;"> IGEN 330 Capstone </h2>
#### Project Description
- Designed an autonomous robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

<img src="/assets/330 - Picture of Painted Line.jpg" height="400"> <video width="300" height="400" controls>  <source src="/assets/330 - Wall Painting Robot Video.mp4" type="video/mp4"> </video>

### Circuitry Design & Software
- Surface mount and through hole soldering of components
- Wiring and troubleshooting of electrical components including Raspberry Pi Pico, Arduino Mega, H-bridges, Lithium ion battery, Time-of-Flight (ToF) sensor, and limit switches
- Integrated motors with H-bridges and conducted extensive robot drive testing
- Wrote code for driving with omni wheels - troubleshooting motor driving, force distribution of driving against the wall, motor stalling
- Supported design and implementation of linear actuators and limit switches for vertical and horizontal positioning as well as motor driving for consistent paint dispensing

<img src="/assets/330 - circuit schematic.png" width="450">

<img src="/assets/330 - Electrical Components on Chassis.jpg" width="300"> <img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="300"> 
  
#### Mechanical Design
- Designed chassis, wheel and motor mounting, as well as custom wheel flange couples for omni wheel drive using CAD
- Created and iterated sensor mount geometry using CAD to maximize accuracy and consistency of results
- Developed CAD models for the paint dispensing system, including paint platform, rail attachment, and wheel stabilizer
- CAD designed paint applicator attachment and tested various application materials and geometries to achieve clean, consistent lines.
  
<img src="/assets/330 - Iso View (Sensors + Applicator).jpg" width="200"> <img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="300"> 

<h2 style="color:#4682B4;"> Tycrop Manufacturing - Mechanical Team </h2>

Mechanical Design Engineering Co-op at [Tycrop](https://tycrop.com/) (May 2025 - Dec 2025)


<h2 style="color:#4682B4;"> UBC Sailbot - Mechanical Team </h2>

Rudder Mechanical Team Member at [UBC Sailbot](https://www.ubcsailbot.org/) (Jan 2022 - Sept 2024)
#### Solidworks CAD Parts & Assembly
- Designed motor, shafts, & timing belt as well as compiled assembly

<img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/18be7fbe-1d6d-4935-bb8d-18311dc1d2e1" width="180"> <img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/dcda9d7b-4d81-40f5-aba7-b0ffed2962ce" width="300">

#### Structural Stress Calculations
- Completed stress calculations to determine minimum diameter of bolts required to avoid shear and tensile failure
  
<img src="/assets/zxFBD" width="310"><img src="/assets/zxcalcs.png" width="650">

<img src="/assets/zypic" width="280"><img src="/assets/zyFBD" width="390">
<img src="/assets/torsional" width="290">

<img src="/assets/zycalcs.png" width="230"><img src="/assets/zycalcs2.png" width="490"><img src="/assets/zycalcs3.png" width="250">


#### Integration with ELEC
- Decided on motors and encoders that satisfy the needs of both MECH & ELEC
- Here you can see some minimum torque calculations that we did based on the worm gear we chose in order to spec a motor. This allowed us to determine how frequently our motor would be drawing maximum current and whether that is viable with the amount of power that the ELEC team is accounting for
  
<img src="/assets/wormgearcalc" width="500"> <img src="/assets/wormgearcalc2" width="500">
<br/>
<br/>
<br/>

<h2 style="color:#4682B4;"> IGEN 230 Capstone </h2>

#### Project Description
- Used Piezoelectric discs to harvest and store energy using the tapping motion of keys on a numpad
#### Solidworks CAD Parts & Assembly
- Designed all parts, compiled assemblies, & ran motion studies

<img src="/assets/numpadbreakdown" width="312"> <img src="/assets/numpadexploded" width="297"> ![Untitled video - Made with Clipchamp](https://github.com/ko-vera/ko-vera.github.io/assets/91451073/953a51cf-c60d-465f-b170-7065d8c8f2f6) 
<br/>
<br/>
<br/>
 
<h2 style="color:#4682B4;"> IGEN 230 Line Following Robot - Individual Project </h2>


![Untitled video - Made with Clipchamp (3)](https://github.com/ko-vera/ko-vera.github.io/assets/91451073/81809f06-70ba-4e8b-8c00-bfcb03b5aecc) <img src="/assets/borottop" width="225"> <img src="/assets/borotside" width="225">

#### Circuitry
- Implemented H-Bridge Board 
  - Used H-Bridge to control direction &rarr; run motors forwards and backwards - this works by opening and closing the respective switches shown
  - Used PWM to control speed &rarr; when the phototransistor sees white (more light) &rarr; more current
  - There are two phototransistors on either side of the black line - when it sees white, there is more current & it moves forward, when one of them sees   black, it will turn
    
<img src="/assets/hbridgeboard.png" width="400"> <img src="/assets/hbridge.png" width="600">

<br/>


  
  


#### Coding Process

[Arduino Code](/assets/Line Following Robot Code.txt)

<img src="/assets/flowchart" width="600">


<!--<img src="/assets/code1" width="300"> <img src="/assets/code2" width="300"> <img src="/assets/code3" width="300">-->
<!--<img src="/assets/code4" width="300"> <img src="/assets/code5" width="300"> <img src="/assets/code6" width="300">-->

<br/>
<br/>
<br/>


  
