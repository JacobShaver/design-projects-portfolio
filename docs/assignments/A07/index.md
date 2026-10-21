# A7 – Bracket FEA

## Objective
For this assignment I was tasked to complete a finite-element-analysis(FEA) on my bracket and link from A06. I had to use the results from the FEA to make different design changes with the intent to make a lightweight, high strength, and high stiffness bracket and link. 

## Analyze

Before I ever started to preform a FEA on any part, I first needed to understand what kind of workflow I would need. From my class lecture I knew there was an "inner loop" to preform FEA under a course and medium mesh. If those results didn't converge within 7% of each other I was to use a fine mesh and take those values down. Once that loop was complete I had an "outer loop" which consisted of making design changes based on my results and repeating the inner loop. I had to repeat this outer loop a minimum of 3 times. From my assignment I found a flow chart of the process seen below in figure 1. This is the chart I refered to throughout the process of this assignment. 

![error](workflow.png)
(Figure 1)

## Decide
### Bracket FEA / Design changes
After I figured out my workflow, I began setting up to start the FEA of my bracket. To do this, I set the inside of the bracket where the T-bar will slide in to be fixed. I also set the force to be a distributed load across the bar that overhangs under the head of the bracket(Feature A). The force was set to be 600lbf, which I chose in A05.

![error](b_design1.png)
(Figure 2)

After using a course mesh initially, I found that in Figure 2 the displacement and the max stress were far beyond what I had originally used to find the dimensions of the bracket. This told me that I had obviously made some mistake along the way when I was initially designing the bracket. Nonetheless, after using the course mesh I then used a medium mesh and compared the values found. Comparing them showed me that the values didn't converge, so I used a fine mesh and took note of the final values that the study produced. The results were a max stress of about 50000psi located at the intersection of feature A & B(red area), a max deflection of 0.29in located at the very end of feature A(red area), a safety factor of 0.8, a weight of 7.26lbs, and the top of the bracket was almost completely unaffected.

![error](b_design2.png)
(Figure 3)

After my results from the first FEA, I decided to change two major things. The first was the addition of filleted edges to reduce the weight a little; however, I didn't fillet any edge that was critically affected under the load. The second was to extend the width of feature B because I made the educated assumption that it was the root of my strength problem. The results of these changes can be seen in figure 3. For this FEA I was only able to get the displacement values to converge from the course to medium mesh. Since max stress and safety factor don't converge, I needed to use a fine mesh to determine my most accurate values. The results were a max stress of about 19400psi located at the intersection of feature A & B(red area), a max deflection of 0.065in located at the very end of feature A(red area), a safety factor of 2.1, a weight of 7.18lbs, and the top of the bracket remained almost completely unaffected. Each value except for max stress was still off from the boundaries given in the original design problem; however, I was on the right track because they did improve from the last test.

![error](b_design3.png)
(Figure 4)

After the results from the second FEA, I made three major changes as seen in Figure 4. Since I knew the maximum deflection was happening at the very edge of feature A, I figured it needed a little extra support I added a mirror of feature B on the other side of the bracket. However, I knew this change would add a lot of unwanted weight to the design, so I reduced the total length of the bracket body & feature A to 2.75in, and I turned Feature A into a tube rather than a solid bar. After the design changes I began the FEA analysis with the same fixtures and the load concentrated at the same place. After a course & medium mesh were applied the design did still fail to converge. However, the convergence percentages were very close to the desired 7% and the actual values were ideal to my given limitations from the original design. Since it didn't converge I repeated the same process and used a fine mesh to determine my finalized results. The results were a max stress of about 602psi located at the intersection of feature A & B(red area), a max deflection of 0.00013in located at the middle of feature A(red area), a safety factor of 66, a weight of 4.99lbs, and the top of the bracket was still almost completely unaffected. Although the values didn't converge, the results were well below my original design limits. 

![error](b_inner_table.png)
(Figure 5)

The above tables show a summarized version of my FEA "inner loop" and which values converge or don't. 

### Link FEA / Design changes

![error](l_design1.png)
(Figure 6)

![error](l_design2.png)
(Figure 7)

![error](l_design3.png)
(Figure 8)

![error](b_inner_table.png)
(Figure 9)

## Communicate
### Final Bracket Results

![error](b_outer_table.png)

### Final Link Results

![error](l_outer_table.png)

### Reflection



### Download Final Designs
[Final Bracket Design](bracket_final.SLDPRT)

[Final Link Design](link_final.SLDPRT)
