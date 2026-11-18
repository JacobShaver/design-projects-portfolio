# A11 – Motor Selection

## Objective
This assignment has us continuing to work with our groups to further design the tensile tester. This portion has us selecting a motor, designing a motor mount, designing/selecting a coupling, designing a floating bearing mount, and finalizing our assembly. We were given very few requirements for making it, so creative freedom is in our hands. The requirements we do have are that it has to have two lead screws, it should be able to transmit 2kN of force, it should have a speed range of 1-50 mm/min, it has a safety factor of 4, and lastly it should have at least a 18 inch lead screw height, designed for a bench top. We were also given a picture of what a bench top tensile tester looks like as guidance for where our end product should land.  

PICTURE 1 - TENSILE TESTER

## Motor Selection - Landon Toepfer
I went looking online for DC motors, just looking to see if they had enough torque to be able to provide the load needed for the tester. After looking through a few I found one with a data sheet that showed it was able to provide enough torque at the bottom and top of our speed range. Its a drylin DC motor with gearbox from igus.com. The link is in our bill of materials. Below you will see what I took note of, specifically the datasheet graph that I used to determine if it was sufficient.  

PICTURE 2 - WORK PART 1

## Motor Mount Design - Landon Toepfer
Now that I found a motor I thought was good, I had to figure out how to mount it to the frame. Luckily the company supplying the frame also has mounting screws that go into the slots on the frame, so I knew how big those holes would be. I also knew the size of the holes in the motor, which are M3, and the profile of their locations given in the data sheet. I decided that the screws going into the motor were going to have to be flat head screws with a countersink hole in order for them to have no profile on the bottom of the mount. This is important because they would be pressed up against the frame. The top of the mount has M8 holes for the frame assembly screws. I then just had to use bearing stress analysis to ensure that the thickness I wanted was larger than the thickness needed for the plate to not break. I used two new equations. One was solving for the force at each hole, It takes into account the total torque and the distance from it to each hole. I had an off center motor shaft, but I assumed it was in the center for this equation. Then the bearing stress was just like any other stress equation, having force over area. The difference is the area is the diameter times the depth, which is a projection of the actual area being affected. I don't understand why necessarily but that how the area is determined. I then was able to solve for the thickness and for both sets of holes, I got way less than 1mm. So I went with my chosen thickness, which was determined from the dimensions of my motor and moved into designing my mount in Creo.  

PICTURE 2 - WORK PART 2

PICTURE 3 - MOTOR MOUNT PART

## Coupling Design/Selection - Landon Toepfer
For this portion we had to either design a coupling or find a coupling. Whether you chose to design one or not you needed to prove that the one you had could resist breaking under torque. So I went ahead and found a coupling on amazon that worked. Found the material it was using and made an estimate of its shear strength. Then I was able to solve for the shear applied to this shape. I used a polar moment of inertia of a hollow shaft, knowing the inner and outer diameters. I calculated for both sides, one for the 6mm motor shaft, and the other for the 10mm screw. I ended up only getting around 1 MPa for both sides. So I was able to say it was strong enough to not shear.  

PICTURE 4 - WORK PART 3

## 4
## 5
## 6

## Bearing Mount - Landon Toepfer
I then had to design a floating bearing mount. I started by looking at other designs of what that would look like. It seems like its a housing for a bearing. So I went and found a bearing that I could put the screw into. I also assumed that The bottom of the lead screw could be ground down to get rid of the threads. I assumed I would machine the threads off down to 8mm diameter. So that is the diameter I used to select a bearing. Then after selecting a bearing I had measurements to design a housing around it. I had to use a RC3 fit to locate the screw so I made a top entry hole with that fit class using a 8mm nominal size. I had to do some convergence between mm and inches but it wasn't a big issue. I then just made it attach to a flat plate with the same sized screw holes as the motor mount. I went ahead and made it up in CAD, downloaded the CAD file for the bearing and handed it off to Jacob to put in the assembly. Below you will see my design work.  

PICURE X - BEARING MOUNT DESIGN WORK

## Bill of Materials - Landon Toepfer
I just have to build off the table from the last assignment.  

| Item Number | Quantity | Name | Unit Price | Total Price | Purchase Link |
| --- | --- | --- | --- | --- | --- |
| 1 | 2 | Lead Screw | 23.67 | 47.34 | https://www.mcmaster.com/7549K72/ |
| 2 | 2 | Flange Nut | 73.36 | 146.72 | https://www.mcmaster.com/7549K16/ |
| 3 | 1 | Crosshead | - | - | - |
| 4 | 8 | Socket Head Screw | 10.43 (Pack of 25) | 10.43 | https://www.mcmaster.com/91251A550/ |
| 5 | 8 | Hex Nut | 3.60 (Pack of 50) | 3.60 | https://www.mcmaster.com/95479A111/ | 
| 6 | 1 | Frame | 143.40 (2m Worth) | 143.40 | https://www.grainger.com/product/80-20-T-Slot-Framing-System-Profiles-906T85 |
| 7 | 8 | Corner Bracket | 6.84 | 64.72 | https://www.grainger.com/product/80-20-Inside-Corner-Bracket-Inside-5JRP7 |
| 8 | 32 | Bracket Assembly Screw | 21.56 (Pack of 15) | 64.68 | https://www.grainger.com/product/80-20-Bolt-Assembly-M8-Size-5JRH6?opr=OAPD&analytics=relItems_5JRP7&position=1 | 
| 9 | 2 | Motor Mount | - | - | - | 
| 10 | 2 | Bearing Mount | - | - | - | 
| 11 | 2 | Motor | Unlisted (~80 estimated) | ~160 (allotted) | https://www.igus.com/product/drylin_E_AE_B_24_001 | 
| 12 | 12 | Motor M3 flat head screws | 7.34 (Pack of 100) | 7.34 | https://www.mcmaster.com/91294A132/ | 
| 13 | 2 | Bearing | 17.26 | 34.52 | https://www.mcmaster.com/1301N212/ | 
| 14 | 40 | Engineering Design Cost | 35/hr | 1400 | - | 

## Drawings
Here is the drawing of the motor mount:  

PICTURE OF MOUNT

Here is the drawing of the bearing mount:  

PICTURE OF MOUNT

Here is the drawing of the assembly:  

PICTURE OF ASSEMBLY

## Lessons Learned  

