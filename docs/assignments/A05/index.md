# A5 – Bracket Design

## Objective
![Error](Intro.png)
(Figure 1)

The objective for this assignment was to design the dimensions for a bracket using two analysis types. These were an analysis for stress throughout the bracket and an analysis for the the stiffness of the bracket. The bracket is meant to slide smoothly over a T bar and needs to hold a strap that applies two pulling forces downward on the bracket.
## Analyze
![Error](Overview.png)
(Figure 2)

Before I started any math, I first drew out what I needed to make and what variables I needed to account for. I knew I was finding the dimensions for segments A-E. 

**For my knowns:**
- The force needs to be between 500-800 lbf
- The safety factor is 4
- Max deflection is 0.005 in
- I need to choose 1 of three materials, aluminum 6061 T6, Steel (ASTM A36), or Titanium (Ti-6Al-V4)
- And I knew the fit discriptions for all givin dimensions:
  - “a” intention for use where accuracy is not essential
  - “b” is about the closest fits that can be expected to run freely
  - “c” is where accurate location and minimum play is desired

## Decide
I chose to use Aluminum 6160 T6 as my material, and I used _MatWeb_ to find the average values for aluminum's modulus of elasticity and yield strength value. I chose to use 600 lbf simply because it was nice rounded force somewhat in the middle of the range. Lastly, I used assignment resources to segment the bracket into easy to understand segments for later use as seen in the concept design in figure 2. 

## Communicate

### Design for stress
After I determined what my known variables were, and determined what order I needed to solve the segments I began an analysis using the yield strength of my material. The last variable I chose to keep consistent, was that the length of the bracket what 4 in. 

For figure 3, Pink highlights values found by using the machinery handbooks guide on different fits starting on page 641, blue highlights symbolic solutions for values, and green highlights final values to be used.

![Error](Stress.png)
(Figure 3)

The main factor that allowed me to solve the various dimensions for the bracket was the assumptions that I made. The first assumption was that the bracket would not fail due to shear stress. At feature A I assumed that it functioned like a cantilever beam with a distributed load over the top of it, which is the same assumption I made for feature E as well. That paved way for me to solve the radius of feature A. After finding the radius of A I made the assumption that B's width was equal to the diameter of A, that the height of B was 3 in, and that B extended from the top half of A's circular face to the base of the bracket. I treated B as a bar floating in space with an axial load, which is the same assumption I made for feature D. For feature C I assumed it was a simply supported beam. For segments C-E I made the assumption that the affected area was limited to the thickness of B. 

The other main problem was a selection for proper clearances at each length a, b, and c. To do this I examined my fit descriptions and decided that feature C needed the classification RC 8, feature D needed LC 6, and feature E needed RC 4. Given my starting lengths at a, b , and c, I found a min and max range of clearance that could be used and chose values that landed generally in the middle of the range. This was so that my T-bar would fit even if the size was a little off from the values I was given for the problem. 

### Design for Stiffness
After Completing my analysis for strain I moved on to solve for the same values but using a given max deflection and modulus of elasticity. I made the same assumptions I did for stress analysis, and used the same pre-calculation values like length of segment A or B. Nothing changed with my width values that I found using the book and the various fit descriptions, so I used the same values in my stiffness analysis. 

For figure 4, blue highlights symbolic solutions for values, and green highlights final values to be used.

![Error](Stiffness.png)

### Multiview drawings for both Stress and Stiffness Analysis
These sketches were done on engineering paper where one grid square was seen as 1/2 in.

![Error]()

![Error]()

### Lessons learned

### Link design
After designing my bracket 



