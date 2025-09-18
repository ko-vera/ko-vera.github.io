

<!--<br/>-->
<!--<img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/cd6c7775-5e18-4cb7-b367-4364af5e81c0" width="70">-->
<font size ="5"> 4th Year UBC Integrated Engineering Student - Electrical & Mechanical</font>

----
Hi! Welcome to my Project Portfolio. I hope this helps in getting to know my skills a little better :) 

<h2 style="color:#4682B4;"> UBC Thunderbots - Electrical Team </h2>

Electrical Team Member at [UBC Thunderbots](https://www.ubcthunderbots.ca/) (Sept 2024 - Present)
#### Altium Circuit Schematic
- Completed the circuit schematic for a kickspeed tester and am currently working on the PCB board layout for the phototransistor side of the kick speed tester arch shown below
- Kick speed tester contains two beams created by two emitters and two transistors. When the ball passes through the arch, the beams are broken and the time between them being broken is measured.
  
<img src="/assets/Screenshot 2024-11-12 120847.png" width="450"> <img src="/assets/Screenshot 2025-01-11 225837.png" width="450">

<img src="/assets/Screenshot 2025-01-21 205145.png" width="450"> <img src="/assets/Screenshot 2025-01-21 205001.png" width="450">


<h2 style="color:#4682B4;"> IGEN 330 Capstone </h2>
#### Project Description
- Designed a robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

<!--<video width="640" height="360" controls>-->
  <source src="/assets/330 - Wall Painting Robot Video.mp4" type="video/mp4">

<img src="/assets/330 - Picture of Painted Line.jpg" width="450">

### Circuitry Design & Software
- Surface mount and through hole soldering of components
- Wiring and troubleshooting of electrical components including Raspberry Pi Pico, Arduino Mega, H-bridges, Lithium ion battery, Time-of-Flight (ToF) sensor, and limit switches
- Integrated motors with H-bridges and conducted extensive robot drive testing
- Wrote code for driving with omniwheels - troubleshooting motor driving, force distribution of driving against the wall, motor stalling
- Supported design and implementation of linear actuators and limit switches for vertical and horizontal positioning as well as motor driving for consistent paint dispensing

<img src="/assets/330 - Electrical Components on Chassis.jpg" width="450"> <img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="450">
  
#### Mechanical Design
- CAD designed custom wheel flange couples
- CAD designed and assembled chassis, wheel, and motor mounting
- CAD designed and iterated sensor mount to maximize accuracy and consistency of results
- CAD designed paint platform, rail attachment and wheel stabilization for paint dispensing
- CAD designed paint applicator attachment, tested various paint application materials and geometries which provided a clean and consistent line
  
<img src="/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg" width="450"> <img src="/assets/330 - Iso View (Sensors + Applicator).jpg" width="450">



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

<h2 style="color:#4682B4;"> CPEN 312 Labs </h2>

#### Lab 1
Binary input to 7-Segment Display using NAND logic gates
- Use of Multisim
- Transferring from schematic to board
  
#### Lab 2 & 3
8 Bit Binary Adder/Subtractor & Clock + Alarm Display
- Implementation of Arithmetic & Counters
- Coding in VHDL for creation of block diagram components
- Use of DE0-CV Board

#### Lab 4 & 5
Varying Number Displays & 32 bit Calculator
- Implementation of Microcomputer Arithmetic
- Coding in 8051 Assembly
- Use of DE0-CV Board

  
