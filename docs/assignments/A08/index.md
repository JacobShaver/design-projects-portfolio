# A8 – Gears

## Objective
For this assignment we were tasked to design a gearbox with given parameters. We had to use a pinion and gear with a ratio of 24:9, the output gear speed and torque are to be 1100RPM and 1.25in-lbf respectively, and the input shaft and output shaft diameters are to be 0.125in and 0.250in respectively with a length of 1in. The gearbox was to be able to be assembled and disassembled. 

## Analyze
To start this assignment I first needed to determine if the given diameters for the shafts were sufficient under the parameters. I strated by writing down all of my given values, the different assumptions I needed to make, and different important information that was notable.
![error](shaftunk.png)
As seen in the lower half of the above picture, before I started to solve for the shafts I first wrote down each unknown value that I needed to solve for. I also took note of every important equation that I COULD use while solving for my unknowns. 
## Decide
### Math for Shafts and Bearings
![error](shaftwork.png)

After analyzing important equations and unknown variables, I started to do the math which ended up being very "plug and play". I first found the input speed, then used that value to find the input torque, and I finally used the calculated input torque to find the input shear stress. I used the values I was given at the begging to determine my output shear stress. After finding these values, I compared them to the maximum allowable stress in both shaft types and the test passed with flying colors. This led me to the conclusion that the shaft diameters I was given were very suitable.

![error](bearingunk.png)
Once I found my shafts to be suitable I then needed to move on and design my journal bearings. This entailed choosing appropriate dimensions for the bearing, determining the max pressure, max velocity, max PV limit, and using these factors to determine what material I wanted to use. After choosing the material, I needed to use its max pressure to solve for thickness of the bearing. The way I interpreted this part of the assignment was that this found thickness was like a minimum thickness for the bearing, so when I choose a bearing from a supplier I know what my low-point is. I chose to use a quarter inch for my bearing length because that seemed to be the most rounded value that would successfully sit on my 1in shaft length along with the gear.

Taking all of this into account, I began writing out my unknowns, different equations I needed to utilize, and analyzing a free body diagram. After finding my max P, V and PV limit, I used a chart and cross referenced the supply site McMaster-Carr to chose bronze as the material for my bearings. I then used the default max pressure for bronze to determine my bearings minimum thickness. After solving for thickness and determining my material, I used McMaster-Carr to find the following bearings:

Pinion Bearing: https://www.mcmaster.com/9368T96/

Gear Bearing: https://www.mcmaster.com/9368T11/

### Concept for Gear Housing Unit
![error](gearhouseconc.png)

After determining what bearings I was using and that my shafts were a suitable size, I also needed to make a rough sketch for my gearbox housing. Seeing as this assignment required that the final design be able to disassemble, I had to make the housing in two parts, and determine how the two halves would fit together. The first half of the image above was me analyzing the different important dimensions of the gears, so that I could determine the minimum size of my housing cavity. The gear dimensions were given to me in the assignment on the McMaster-Carr website: 

Pinion: https://www.mcmaster.com/7880K19/

Gear: https://www.mcmaster.com/7880k24/

I decided to utilize two bearings on either side of the gears, so each gear wasn't prohibited by the housing. After determining all my dimensions I decided on the final rough sketch at the bottom of the page. I made sure to note that I wanted the thickness of the box to be about 0.15in on each side, and that I was using a snap fit mechanic to hold the top and bottom halves together.

## Communicate
### Imported CAD files from Mcmaster
![](pinioniso.png)

![](geariso.png)

![](pinionbeariso.png)

![](gearbeariso.png)
### Designed parts in CAD
#### Shafts
![](pinionshiso.png)

![](gearshiso.png)
#### Gear Housing 
![](gearhouse1.png)

![](gearhouse2.png)

![](gearhouse3.png)

![](gearhouse4.png)

![](gearhouse5.png)

![](gearhouse6.png)
#### Assembly for gearbox
![](assemiso.png)

![](assemexploded.png)

### Drawings for Each Part
![](pinionshaft.png)

![](gearshaft.png)

![](pinionbearing.png)

![](gearbearing.png)

![](gearhousebot.png)

![](gearhousetop.png)

![](finalassem.png)

### Lessons Learned

### Zip Files for All Parts/Drawings/Assembly
[A8 Part Files](A8partfiles.zip)

[A8 Drawing Files](A8drawfiles.zip)

[A8 Assembly files](Assemfiles.zip)
