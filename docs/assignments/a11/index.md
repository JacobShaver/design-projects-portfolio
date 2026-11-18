# A11 – Motor Selection

## Bracket design / frame confirmation - Jacob Shaver
For this portion of the assignment, I was tasked to complete a strength analysis to confirm my desired bracket dimensions. The way that I did this was by finding bending stress on the bracket, bearing stress on the bracket's holes, and shear stress on each bolt in the bracket. I then took these values and compared them to the yield strength of the bracket, which I assumed to be the same material as my frame. To start the design process I first needed some bracket dimensions, and I decided to use the L-bracket found on the website below.

Bracket Component link: https://www.grainger.com/product/80-20-Inside-Corner-Bracket-Inside-5JRP7

PICTURE 1: BRACKET DIMENSIONS

I used these dimensions to find all my stress values. Once I determined the values I went through and compared each to the yield strength of 172.37MPa and found a set of safety factors. My confirmation was, if all the safety factor exceeded my desired value of 4 then the bracket would hold. All of the stresses produced a very high safety factor with my lowest being 95.

PICTURE 2: STRENGTH ANALYSIS

## Verification of Top Bar Through FEA - Jacob Shaver

Next I needed to confirm that the top of my frame would hold under the force from the leadscrews, and the torque from the motor. I did FEA through Creo PTC which had me first set up part fixtures and loads/moments. Most of this process was fine; however, when it came to implementing the torque reactions I had to get creative and turn it into a force couple because i couldn't figure out how to directly input the torque into the analysis. 

PICTURE 1: FEA 1

### FEA Analysis 1 & 2

Once I set up the fixtures and loads, I created a mesh with an element size of 30mm to start and ran the first analysis. I moved the element size down to 20mm and ran a new static analysis, so that I could compare the results and test for convergence. 

For my stress the high-end was extremely high; however, this was a singularity and wouldn't reflect what would actually happen in the real world. Instead of taking that value, I used a tool in Creo to directly analyze the stress all over the part and came up with a max stress of 8.6MPa for the 30mm element analysis and 7.6 for the other. As you can see in the picture below, essentially the entire part was dark blue which showed me I consistently was on the low-end of my stress range. Between both analysis the stress did not end up converging. I used my determined max stresses and the material of the bar to determine my safety factor. Between the two analysis the safety factor also diverged.

PICTURE 2: FEA 2 STRESS

For my displacement, my max was extremely low on both analysis, which was a good sign. The max seemed to be concentrated at the center of the bar, while the ends were almost completely unaffected. Between the two analysis the displacement did converge. This interaction can be seen below.

PICTURE 3: FEA 3 DISPLACEMENT

### FEA Analysis 2 & 3

Since the first two analysis did not converge, I did a third analysis with even finer elements and compared it to the second. Between the second and third analysis, the only values that converged was the safety factor. Despite that my values were still well within a desirable range for displacement and max stress.

PICTURE 4: FEA 4 STRESS

PICTURE 5: FEA 5 DISPLACEMENT

### Proposed Changes in the design

PICTURE 6: FINAL CONVERGENCE TESTS

After analyzing the max displacement and max stress along with their locations, I think the spot to change is at the ends of the beam. One change that would lower some of the weight is to remove some material in the middle of the beam where it connects to the vertical one. Otherwise I think the original design is pretty good already and sufficient for what we need it to do. 

## Verification of Side Bars Through FEA - Jacob Shaver

After running FEA on the top bar I needed to do the same for the vertical supporting bars. Because of symmetry, I knew the reactions in both vertical bars would be near-exact so I only did FEA on one. To do this I made fixtures where the bar would be held to another with a bracket, an axial compressive load on the top face, and a transverse load from the motor reactions on the top end of the vertical bar. This can be seen below.

PICTURE 1: FEA 1

### FEA Analysis 1 & 2

After setting up the required fixed points and load points, I began the study by using a mesh of 20mm. Once I ran that study I did another with a mesh of 15mm.

Once more, the high-end for my stress was leagues higher than my yield strength; however, this was a singularity that wouldn't directly reflect the real world. This is why I did the same thing as earlier and used a tool to find my max stress on the bar. The values for analysis one ended up being 0.8113MPa for the first and 0.8077MPa for the second. These two values converged when tested. I sued these and compared them to the yield strength to find the safety factors, which were extremely high and converged. 

PICTURE 2: FEA 2 STRESS

For the displacement results, the max values were very low again. The max deflection was located at the upper left corner of the beam. Even though the max values were desirable, they did not end up converging.

PICTURE 3: FEA 3 DISPLACEMENT

### FEA Analysis 2 & 3

Since my displacement didn't converge I ran another pass with even finer element size of 10mm and compared it to the second analysis. Between these two analysis, the stress and the safety factor converged but the displacement still didn't. However, my values were still well within what we needed for the frame to be stable under the set conditions. 

PICTURE 4: FEA 4 STRESS

PICTURE 5: FEA 5 DISPLACEMENT

### Proposed Changes in the design

PICTURE 6: FINAL CONVERGENCE TESTS

After analyzing the max displacement and max stress along with their locations, I think the spot to change is at the middle of the beams. One change that would lower some of the weight is to remove some material in the middle of the beam where it isn't being connected to another beam. This would greatly cutdown on the weight of the beam, and as long as too much isn't removed, it shouldn't lower the safety factor too greatly. Otherwise I still believe the original design is pretty good already and sufficient for what we need it to do. 

## Final Assembly and Assembly Drawing - Jacob Shaver

Below is the final assembly with all designed parts, and the drawing to go along with it.

PICTURE 1: ASSEMBLY SS
PICTURE 2: ASSEMBLY DRAWING SS
