# A10 – Lead Screw Translating System

## Objective
This assignment has us working in groups to complete a design for a lead screw tensile testing system. We were able to select our groups so I was able to work with my friend that I have been doing most assignments along side throughout the semester. We were given very few requirements for making it, so creative freedom is in our hands. The requirements we do have are that it has to have two lead screws, it should be able to transmit 2kN of force, it should have a speed range of 1-50 mm/min, it has a safety factor of 4, and lastly it should have at least a 18 inch lead screw height, designed for a bench top. We were also given a picture of what a bench top tensile tester looks like as guidance for where our end product should land.  

PICTURE 1, TENSILE TESTER

## Lead Screw Design - Landon Toepfer
So the start of this process for determining what size of lead screw I need to use is ensuring that the screw is thick enough to withstand tensile stress across its area. This was a simple stress problem where I have to solve for area with yield stress known and applied load known. I didn't know what the material of the lead screw was to start so I had to look at our provided resources to see what the supplier was going to use. Turns out it 1018 low carbon steel so I was able to find the yield strength using matweb.com. Moving on, the applied load on each lead screw was going to be half of the total load, so 1kN. I also needed to include the safety factor so I had to turn yield strength into allowable yield stress. After doing that, I plugged in the area for a circle with a diameter variable and I plugged in the load of 1000 N, and lastly the allowable stress. Then solving for diameter I got 3.71mm which means most lead screws will be more than enough.  

PICTURE 2, LEAD SCREW WORK PART 1

Then I had to determine the rotational speed needed to obtain the linear speed specified in the assignment. This was a simple problem of turning mm/min into rev/min (RPM). The way I needed to do this was knowing the lead of the screw or the distance traveled per rotation. I found this by again going to the supplier website and finding an example value of what that might be. Luckily they have "Travel Distance per Turn" listed as a specification. I went ahead and picked the smallest one of 2mm and used that to solve for RPM. The equation is as simple as dividing linear speed of mm/min by the lead of mm/rev to get angular speed of RPM. I ended up getting the range converted into 0.5 RPM - 25 RPM. Considering that the assignment says our tensile tester would not be electronically powered but mechanically powered, I figured this speed is achievable with a hand crank of sorts.  

PICTURE 3, LEAD SCREW WORK PART 2

Lastly I needed to be able to show how the load applied can be achieved with a given amount of torque applied through our lead screw. I did this by first selecting a lead screw and an accompanying flanged nut in order to solve for torque using the geometry. We were given a warm up problem in class that helps demonstrate the concept of tangential force (torque) to vertical load (P) which you'll see in my work. I order to solve this equation I needed to find what all the variables are for the particular screw. The L is the lead which is 2mm, the C is the circumference of the minor diameter of the screw, and the P is the 1000N. I also needed to find the coefficient of friction between the steel and the bronze nut. So I was able to find that in the machinery's handbook as 0.15 +- 20% so I used the upper limit of that 20 percent at 0.18. I also need to use the torque equation to substitute out the F. After doing all of that I was able to solve for torque. I ended up getting 1114 N-mm.  

PICTURE 4, LEAD SCREW WORK PART 3  

## Flange Nut Strength Verification - Jacob Shaver

## Crosshead Design - Jacob Shaver

## Cost Tabulation - Landon Toepfer
Part of this assignment was counting the total price needed to fully assemble this if need be. This including giving each type of part needed a number, a quantity, a name, a unit price, a total price spent on it, and providing a purchase link. We ended up having 8 total part types. Our combined total landed on 400.41. The crosshead itself did not have a cost because it was not going to be purchased from a supplier so the price was to be determined.  

| Item Number | Quantity | Name | Unit Price | Total Price | Purchase Link |
| --- | --- | --- | --- | --- | --- |
| 1 | 2 | Lead Screw | 23.67 | 47.34 | https://www.mcmaster.com/7549K72/ |
| 2 | 2 | Flange Nut | 73.36 | 146.72 | https://www.mcmaster.com/7549K16/ |
| 3 | 1 | Crosshead | - | - | - |
| 4 | 8 | Socket Head Screw | 10.43 (Pack of 25) | 10.43 | https://www.mcmaster.com/91251A550/ |
| 5 | 8 | Hex Nut | 3.60 (Pack of 50) | 3.60 | https://www.mcmaster.com/95479A111/ | 
| 6 | 1 | Frame | 143.40 (2m Worth) | 143.40 | https://www.grainger.com/product/80-20-T-Slot-Framing-System-Profiles-906T85 |
| 7 | 4 | Corner Bracket | 6.84 | 27.36 | https://www.grainger.com/product/80-20-Inside-Corner-Bracket-Inside-5JRP7 |
| 8 | 8 | Bracket Assembly Screw | 21.56 (Pack of 15) | 21.56 | https://www.grainger.com/product/80-20-Bolt-Assembly-M8-Size-5JRH6?opr=OAPD&analytics=relItems_5JRP7&position=1 | 

## Parametric Modeling - Jacob Shaver

## FEA Optimization on Crosshead - Landon Toepfer
This assignment required us to do FEA analysis and optimization on the crosshead itself because we are both in 2157 so we have extra work. I started this by adding a 1000N load on either side where the holes for the nut are because that is were the lead screws force would be coming through. Then I added a constraint on the center hole that I added, which you would thread the tensile sample into. It wasn't apparent how the samples were being tested and there is more than one type of sample shape so I went ahead and looked up a common thread for a tensile sample. I ended on a 1/2 - 13 UNC thread which is common to have in the load cell of a tensile sampler. Moving on, I set my material of the body to 6061 aluminum. I also set my minimum element size to 10mm and went ahead with my first analysis. Here's a picture of my setup.  

PICTURE 1, MODEL SETUP

After the first analysis I got my maximum Stress to be 27 MPa but it was just around the rim of the center hole. The majority of the structure was experiencing at most 10 MPa. The deflection results were really good as the maximum deflection was 0.04 mm which is basically nothing. I did need to continue doing analysis on it so that my results converged. Below are my first results.  

PICTURE 2, FIRST STRESS
PICTURE 3, FIRST DEFLECTION

After the second analysis with my max element size of 5mm, I got my max stress to be 31 MPa with the same location with the majority of the structure really only experiencing 10 MPa. The max deflection again was around 0.04 mm. My stress results didn't converge so I went ahead and just did it again with my element size being 3mm. Below are my second results.  

PICTURE 4, SECOND STRESS
PICTURE 5, SECOND DEFLECTION

After the third test I got my max stress to be 35 MPa around the hole and still only being 10 MPa throughout the structure. The deflection max was still 0.04 mm. With these results I can move into making some conclusions to build off of. Below are the third set of results.  

PICTURE 6, THIRD STRESS
PICTURE 7, THIRD DEFLECTION

So my maximum stress was located on the rim of the center hole, it was 35 MPa which gives a safety factor of 7.8. The max deflection was 0.04043 mm in the end which is acceptable. Generally speaking the crosshead was very strong but it had no rounding or chamfering and was just a big block so there was a lot of excess weight so I decided to making rounding, chamfering, and material removal my main focus of optimizing the design. I started by removing the middle on either side of the center hole. I also thinned the part in the middle. I then rounded the outer edges and the inside of the cuts made in the center. I then added a 1 mm chamfer to all of the holes. I figured this was a great optimization and went to retest my design. I ended up getting a max stress of 132 MPA which sounds bad but its just a stress concentration on the rim of the middle hole again. The hole structure only experiences around 25 MPa at max, with the most being near the center. The max deflection did increase and now is 0.0732 mm which is still a very small amount. The starting mass was 1.821 kg and it ended with 1.400 kg. This means I saved about 22% of material and barely reduced the strength of the part. It also is a highly machinable design. Overall, I would consider the process an optimization success. Below are my results after the optimization. 
PICTURE 8, STRESS FINAL
PICTURE 9, DEFLECTION FINAL


## Crosshead Drawing - Jacob Shaver

## Lessons Learned - Team Thoughts

