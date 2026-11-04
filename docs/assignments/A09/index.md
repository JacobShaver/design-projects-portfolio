# A9 – Pulleys

## Objective
This assignment tasked me with designing a pulley system under a certain situation. We need to use a combination of different concepts used throughout this course. which include but are not limited to friction, static analysis, and dynamic analysis.

## Analyze
Before I started my analysis I needed to make sure that the pulley system would be made with the following parameters in mind:
- The axis' need a center distance of 4-6 inches
- Both pulleys must have a diameter of 3 inches
- The operating speed must be 1000-2000rpm
- The belt tension must be 4-6 lbf
- The pulley material may be aluminum, ABS, or steel
- The design must satisfy a minimum safety factor of 3

## Decide
The image below shows the different values and materials I decided to use for the assignment. I essentially chose to throw all my values right in the middle of the ranges because that's what felt right. I also determined some important things before starting like the total length the belt needed to be to go around both pulleys with my determined center distance. 

![error](Analyze.png)

## Communicate
### Belt Design
After determining all the different aspects of the assignment I began by designing the minimum diameter of the belt. One important value that I determined from class slides was that the coefficient of friction for rubber to steel connection was 0.60. To get to the size of the belt I needed to find F1, F2, and cross-sectional area in that order. After finding area I could determine the minimal cross-sectional diameter and the circumference. This entire process is in the image below. 

![error](part1.png)

After finding all this information I needed to find an actual belt on McMaster. I knew that my actual diameter wouldn't be a standardized sizing so I went with the smallest possible match that still was greater than my theoretical minimum. I decided to use a belt diameter of 5/16", and the listing I found ranged from a length of 10"-1200", and it increased in increments of 1/4". This was perfect because I could get stock that met my minimum diameter requirements, and I could order a size that was as close as possible to my desired length. 

Belt link: https://www.mcmaster.com/9462T58/

### Shaft Desin
After designing the belt I needed to design the shaft by finding the minimum dimensions when torque is applied. I used Matweb to determine the yield strength for 1060 hardened steel, which ended up being 93000 psi. To design the geometry I used the maximum allowed stress under the torque applied. The image below shows my entire work process. 

![error](part2.png)

I decided to base the actual size of my shaft to be based on my bearing, which is in the next section. This is because my bearing will be some standard size, and its much easier to match some shaft stock size to the bearing rather than manufacturing my own shaft and bearing. The main consideration is to make sure the stock shaft I choose is still larger than the minimum that I determined. 

### Journal Bearing Design
After designing my shaft I then began to work on the bearing size, and material confirmation. To do this I needed to find Pressure, Velocity, and PV rating. The work to do that is in the below image. 

![error](part3.png)

After finding those values I cross referenced them to the same chart I used in assignment 8, and I determined that my material should be a pourous bronze. I came to choose this material because it seemed to be the most accesible, and it had the most size choices while still fitting the calculated PV limit.

