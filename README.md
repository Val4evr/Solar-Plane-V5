# Solar Plane V5
![Explosion view gif of solar plane V5](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Explosion%20animation.gif)

# Introduction:
The SPV5 project is a radio-controlled solar powered plane created by me in my spare time over the course of 6 months. 

It features Sunpower C60 solar cells, a Genasun MPPT charge controller, a high efficiency low KV motor and a largely 3D printed structure.

At the end of the project the plane was test flown, but crashed almost immediately after launch. Despite this, it features some interesting engineering.

# Parts worthy of discussion:

## Fuselage:
![Side view of the fuselage internals, showing the electronics](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Fuselage%20internals.png)

The fuselage shell contains most of the electrical components.
These are mounted on a carbon fibre rail system using neodymium magnets (to ensure easy servicing). The rails are securely attached to the main structural beam which connects the fuselage, wings and tail together. A placeholder for the motor at the front is also present. 

## Electronics:
![Picture of a PCB 3D model with two yellow connectors, labeled "ESC" and "BATT"](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/MPPT%20Manager%20board.png)
Sunpower C60 cells are wired in a 7S2P configuration, and provide 4.2v to the MPPT boost charge controller. The charge controller is connected to a custom adapter PCB designed by a friend via an IPC cable. The battery and ESC are subsequently connected to it. There is also a RPi Pico microcontroller that can be used to log charge controller errors, although that was never implemented.    

## Planform / aero:

## 3D printed elements


## Structural elements

![Wide view of all the structural frame elements of the plane](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Frame-all.png)

Because the fuselage shell, wings and tail have very little structural integrity of their own, the plane is held together using pultruded carbon fibre tubes. At intersection points, 3D prints hold the rods together. 



 



