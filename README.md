# Solar Plane V5
![Side view of the fully assembled plane](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Side%20view.png)
![Explosion view of solar plane V5](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Explosion%20animation.gif)

## Introduction:
The SPV5 project is a radio-controlled solar powered plane created by me in my spare time over the course of 6 months. It has a wingspan of 1.82m.

It features 14 SunPower C60 solar cells, a Genasun MPPT charge controller, a high efficiency low KV motor and a largely 3D printed structure.

At the end of the project a prototype of the plane was test flown, but crashed due to a side gust during launch. Despite this, it features some interesting engineering.

## Parts worthy of discussion:

### Fuselage:
![Side view of the fuselage internals, showing the electronics](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Fuselage%20internals.png)

The fuselage shell contains most of the electrical components.
These are mounted on a carbon fibre rail system using neodymium magnets (to ensure easy servicing). The rails are securely attached to the main structural beam which connects the fuselage, wings and tail together. A placeholder for the motor at the front is also present. 

### Electronics:
![Aa PCB 3D model with two yellow connectors, labeled "ESC" and "BATT"](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/MPPT%20Manager%20board.png)
Sunpower C60 cells are wired in a 7S2P configuration, and provide 4.2v to the MPPT boost charge controller. The charge controller is connected to a custom adapter PCB designed by a friend via an IPC cable. The battery and ESC are subsequently connected to it. There is also a RPi Pico microcontroller that can be used to log charge controller errors, although that was never implemented.  

![Planform view of the plane, showing 14 solar cells.](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Planform.png)
The 14 C60 cells generate a theoretical peak power of 50W. The cells are embedded in the wing at a depth of 0.15mm, meaning that they have minimal aerodynamic impact. The wing is also laminated with epoxy resin, providing a very smooth surface finish.


### Planform $ calculations:
![Screenshot of web tool used for calculation](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Planform%20calculations.png)
The planform design is made in a web tool called [cgCalc](https://www.ecalc.ch/cgcalc.php?deeplink=Solar%20Plane%20V5;mm;mono;175;175;175;175;175;175;0;0;0;0;0;910;0;0;0;0;9;47;47;22.5;18.7;1;0;0;5;8;25.2;0;7;81;3;2;0;0.80;100;100;100;100;100;100;0;0;0;0;0;200;0;0;0;0;800;25;7.5;0;20;165;30;). It was used to iteratively arrive at a design that has space for solar panels, while also having a high theoretical efficiency and being simple enough to be feasible to complete in the limited time frame. 


### Aerodynamic components:
The wings, horizontal & vertical stabilizers and control surfaces are 3D printed out of LW-PLA. It is a filament that activley foams during printing, resulting in parts with half the density of normal filaments. Strength suffers significantly, though. Tensile strength drops by a factor of over 7. This means it is only used for weakly structural parts, such as the outer skin of the wings, as well as ribs. 

![Image showing cad model of fuselage, prepared for printing](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Print-prep%20fuselage%20shell.png)
Image of the fuselage shell, optimized for vase mode.

The internal structure of the LW-PLA components is optimized to be printed in vase mode. This allows for a high surface quality despite printing with activley foaming material. This optimization step is quite computationally intensive to process and render, so it is split out to a different file. 

![Image showing wireframe cad model of wing. All the internal ribs are visible](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Wing%20wire%20view.png)

As seen above, the internal structure of the LW-PLA parts is complex. The skin, ribs, spar and stringers are combined into a single part. This reduces mass, manufacturing complexity, and gives good skin surface quality as there is little space between ribs. To further add to the surface quality, and protect the solar cells, the wings are coated with a thin layer of epoxy resin. The foam texture of the LW-PLA is great at bonding with epoxy, so no preparation is needed except a light sanding. 


### Structural elements:

![Wide view of all the structural frame elements of the plane](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Frame-all.png)

Pultruded carbon fibre tubes act as the "frame" of the plane. Where the tubes interesect, they are joined by 3D prints. 

![Closeup of the wing joint](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Frame-interconnector.png)

The wings are detachable and their internals are asymmetric, meaning that the spars from the left wing protrude into the right and vice versa. This makes the fuselage more streamlined, as well as reducing the mass of the frame significantly. 

The aerofoil shaped green part above is the wing insert. It is glued directly to the LW-PLA structure, and bolted into the red part, which is known as the "interconnector". That single bolt prevents both wings from sliding out. The interconnector connects to the yellow component, which is glued to the tail tube. 

The fuselage mounting rails are similarly mounted to the tail tube, via the two parts at the front. These can also be decoupled via a single bolt. 

![Closeup of the front structure of the plane](https://github.com/Val4evr/Solar-Plane-V5/blob/main/Images/Frame-front.png)

The mounting rails terminate at the motor mount plate, and transfer the thrust to the frame. The wing plugs are optimized for strength along the load axis. 








 



