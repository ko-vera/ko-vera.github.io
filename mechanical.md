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
- [Wall Painting Robot](#wall-painting-robot)
- [Energy Harvesting Keyboard](#energy-harvesting-keyboard)

[← Back to Home](/) · [Electrical Work →](/electrical/)

</nav>

<div class="toc-content" markdown="1">
  
# ⚙️ Mechanical Work

## Tycrop Manufacturing

Mechanical Design Engineering Co-op at [Tycrop](https://tycrop.com/) (May 2025 - Dec 2025)

## UBC Sailbot

Rudder Mechanical Team Member at [UBC Sailbot](https://www.ubcsailbot.org/) (Jan 2022 - Sept 2024)

#### Solidworks CAD Parts & Assembly

- Designed motor, shafts, & timing belt as well as compiled assembly

[![](https://private-user-images.githubusercontent.com/91451073/320323400-18be7fbe-1d6d-4935-bb8d-18311dc1d2e1.png)](https://private-user-images.githubusercontent.com/91451073/320323400-18be7fbe-1d6d-4935-bb8d-18311dc1d2e1.png) [![](https://private-user-images.githubusercontent.com/91451073/320323743-dcda9d7b-4d81-40f5-aba7-b0ffed2962ce.png)](https://private-user-images.githubusercontent.com/91451073/320323743-dcda9d7b-4d81-40f5-aba7-b0ffed2962ce.png)

#### Structural Stress Calculations

- Completed stress calculations to determine minimum diameter of bolts required to avoid shear and tensile failure

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zxFBD)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/zxFBD)[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zxcalcs.png)](/ko-vera/ko-vera.github.io/blob/main/assets/zxcalcs.png)

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zypic)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/zypic)[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zyFBD)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/zyFBD) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/torsional)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/torsional)

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zycalcs.png)](/ko-vera/ko-vera.github.io/blob/main/assets/zycalcs.png)[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zycalcs2.png)](/ko-vera/ko-vera.github.io/blob/main/assets/zycalcs2.png)[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/zycalcs3.png)](/ko-vera/ko-vera.github.io/blob/main/assets/zycalcs3.png)

#### Integration with ELEC

- Decided on motors and encoders that satisfy the needs of both MECH & ELEC
- Here you can see some minimum torque calculations that we did based on the worm gear we chose in order to spec a motor. This allowed us to determine how frequently our motor would be drawing maximum current and whether that is viable with the amount of power that the ELEC team is accounting for

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/wormgearcalc)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/wormgearcalc) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/wormgearcalc2)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/wormgearcalc2)

## Wall Painting Robot

*(See the [Circuitry Design & Software](/electrical/#igen-330-capstone---circuitry-design--software) side of this project on the Electrical page.)*

#### Project Description

- Designed an autonomous robot to detect a wall, locate the base trim, and accurately paint a line above the trim, eliminating the most difficult and time consuming part of painting your walls.

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Picture of Painted Line.jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Picture of Painted Line.jpg>)

#### Mechanical Design

- Designed chassis, wheel and motor mounting, as well as custom wheel flange couples for omni wheel drive using CAD
- Created and iterated sensor mount geometry using CAD to maximize accuracy and consistency of results
- Developed CAD models for the paint dispensing system, including paint platform, rail attachment, and wheel stabilizer
- CAD designed paint applicator attachment and tested various application materials and geometries to achieve clean, consistent lines.

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Iso View (Sensors + Applicator).jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Iso View (Sensors + Applicator).jpg>) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg)](</ko-vera/ko-vera.github.io/blob/main/assets/330 - Robot Side View (Chassis, Motors, Wheels).jpg>)

## Energy Harvesting Keyboard

#### Project Description

- Used Piezoelectric discs to harvest and store energy using the tapping motion of keys on a numpad

#### Solidworks CAD Parts & Assembly

- Designed all parts, compiled assemblies, & ran motion studies

[![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/numpadbreakdown)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/numpadbreakdown) [![](https://github.com/ko-vera/ko-vera.github.io/raw/main/assets/numpadexploded)](https://github.com/ko-vera/ko-vera.github.io/blob/main/assets/numpadexploded) [![Untitled video - Made with Clipchamp](https://private-user-images.githubusercontent.com/91451073/320353921-953a51cf-c60d-465f-b170-7065d8c8f2f6.gif)](https://private-user-images.githubusercontent.com/91451073/320353921-953a51cf-c60d-465f-b170-7065d8c8f2f6.gif)

----

[← Back to Home](/) · [Electrical Work →](/electrical/)
