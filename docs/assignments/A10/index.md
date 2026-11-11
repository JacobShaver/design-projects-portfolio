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
Once Landon finished the calculations to find the lead screw and flange nut, I needed to verify that the internal threads would support the load. To do this I used bending stress analysis and the equation associated with it in my class lecture notes. In order to verify the flange nut i needed to first find the bending stress using this analysis, and then compare it to its yield strength of 350MPa. This comparison would give me the safety factor of the flange nut, and as long as it was greater than the intend safety factor of 4 then the part would be verified. I used the information under the flange nut's McMaster listing to find the different constants I didn't know. As seen below I determined all of my constants like minor diameter or number of engaged threads and used them to find the internal thread bending stress to be 15.03MPa. I took the ratio of yield strength and bending stress to find the safety factor to be 23. This value was well above the needed factor of safety which verified that the flange nut would work for our design.

PICTURE 1, FLANGE NUT VERIFICATION WORK

## Crosshead Design - Jacob Shaver
After verifying the flange nut it was my task to design the crosshead. I needed to complete a strength and stiffness analysis to determine the minimum thickness of my cross head, and then make a detailed Multiview sketch of the final design concept. Some things I determined before I started include, what frame I would use, what the center distance between the two lead screws needed to be, and the clearance needed from the center of a lead screw to the edge of the crosshead. I used a example of a tensile tester given in the assignment to determine what kind of frame I wanted to use, which ended up being the 80mm X 40mm listed in the cost table. To determine all initial dimensions I somewhat guessed and checked using the example provided to me. Both analysis were to be done as if the cross head were a simple beam with to supports at either end.

### Strength Analysis
After figuring out what my dimensions needed to be, I began working on the strength analysis to determine thickness first. In order to simplify the inertia calculation, I decided to make the cross head a solid bar with the same material as the frame. As seen below I used all my determined values and the yield strength of aluminum found with MatWeb to solve for thickness of the bar. The minimum thickness under the strength analysis came out to 13.2mm. 

PICTURE 1, STRENGTH ANALYSIS WORK

### Stiffness Analysis
After optimizing the thickness for strength I need to do the same for stiffness. I used all the same values, except for a given max deflection of 0.1mm and the section modulus of 68GPa. As seen below, I used the deflection equation for a simple beam and rearranged it so that I could find the thickness of the beam. After calculations I found the minimum thickness to be 30.9mm.

PICTURE 2, STIFFNESS ANALYSIS WORK

### Final Design Concept
After completing both analysis, I found that the stiffness ended up determining the minimum thickness. Before I moved on to make a detailed drawing I made a note to treat the thickness as 32mm because its still greater than the minimum and it would add ease of manufacturing. Below is my finalized concept sketch for the crossbody and the notes that I took into account when designing it. I treated each hole as a clearance hole because the flange nut should control where the crosshead is on the lead screws, and the flange nut is to be fastened to the cross head by a nut and bolt.

PICTURE 3, DESIGN NOTES
PICTURE 4, MULTIVIEW DRAWING

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

### CAD Design of the Crosshead
After designing everything on paper it was time for me to begin designing the crosshead in CAD. We chose to use CREO PTC to do all CAD work on this assignment. 

As shown below, I started with a big box that had the length and width dimensions of 280 and 80 respectively. After making that I added two holes with a diameter of 12mm, the first of which was measured 40mm off the side like I planned and the other was 200mm off that hole. Both holes were made so that they lied at the center of the box's width. I then extruded the box to be at the thickness that I calculated earlier. 

PICTURE 1, CAD 1

After that I needed to add the holes for fastening the flange nut to the cross body. To achieve this I made a reference circle with a diameter that equaled the internal mount diameter on the flange. I then placed 4 circles with a matching diameter to the flange nut's and extruded it through the part. To make this change on both sides of the cross head, I used a reference plane placed i the middle to mirror the holes I made to the other side. This process can be seen in the two picture below.

PICTURE 2, CAD 2
PICTURE 3, CAD 3

After making all the dimensions to be around what they were in calculations I used the relations tab and parameters tab to assign each dimension based one the design parameters.

PICTURE 4, PARAMETRIC DESIGN

### Final assymbly
Before I started on the assembly of the tensile tester, I wanted Landon to optimize through FEA first so that the final design was reflected through this assembly. I used various center and coincident constraints to design the final tensile tester below. One important note was that Landon found the bolt and nut that we used to fasten the flange to the crosshead. 

PICTURE 10, FINAL ASSEMBLY

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
After Landon had optimized the crosshead through FEA, I worked on the drawing for the cross head. Below is how that drawing turned out.

PICTURE 1, DRAWING

## Lessons Learned - Team Thoughts

## Download our CAD Files

