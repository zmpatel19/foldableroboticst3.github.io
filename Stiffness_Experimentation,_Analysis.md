---
title: Data Collection, Experimentation and Analysis
---

# Data Collection, Experimentation and Analysis

## Procedure Writeup

Recap of stiffness requirements: The human Achilles Tendon (AT) shows a stiffness of around 328 - 500 N/mm. This is the stiffness range required from the elemental muscle under development.

Rationale for picking stiffness as our primary parameter to be optimized: Our prototype has been developed within tolerances and limitations posed by manufacturing processes taught and materials available. In order to determine the hinge material that would provide the required torsional stiffness at joints q5 and q2 (Fig. 1), we would need to match **endplate stiffness** characteristics of our prototype model to that of the simulation model and run the scipy.optimize function to zero in on the required joint stiffness parameter k. 

K obtained from this process would effectively be the material properties of the hinges/links used to manufacture our prototype and would prove that our optimization operations are working as desired. From here, we can then run the optimization for the required stiffness of our elemental muscle (500 N/mm) to obtain the optimal k value and would determine the material (and thickness) to be selected as a compliant hinge

**Endplate stiffness - defined as the force - displacement relationship perceived at the end effector (link E, fig. 1) when a force is applied normally to the link.**

Step 1 (prototype manufacturing) - Our Sarrus mechanism prototype has undergone a couple of iterations since our first attempt:
Iteration 1: Consists of a circular (3 link circular arrangement). Challenges discussed in later sections.
Iteration 2: Element with 4 links arranged on either side of a square end effector surface
Iteration 3: Fiberglass stiffeners added to the actuating arms.

Step 2 - Actuator placement and initial characterization 
Step 3 (Stiffness measurements) - The mechanism was first set to a particular pose (determined by servo hold angle). At steady state, weights of known mass (50g and 100g) are placed to alter the end effector position. The force - deflection ratio (endplate stiffness) is thus calculated after multiple such loading cycles are performed to obtain an average stiffness at the end effector at a given pose.

Above process is repeated for different poses.

## Discussion of each steps

Step 1: After initial characterization, it was observed that the model exhibited little to no stiffness - a far from ideal property as we require the structural component of our muscle element to exhibit passive stiffness. This prompted our move from a circular (3 link arrangement) to a square structure with 4 links arranged orthogonally. The actuating arms were split into two arms on either side of the compliant arm to offer better stability.

Step 2: Servo motors were chosen for actuation. It was observed that actuating a single arm was not ideal as other arms would comply under higher loading and buckling. To offer more actuating stability, two servos were placed opposite each other. Further, we observed compliance in the actuating arms themselves despite symmetrical servo placement. To counteract this, we added stiffening elements (fiberglass cuts) to the actuating arms

Step 3: A ruler placed beside the end plate was used to measure the deflection induced due to loading. As expected, we were able to observe varying stiffness. Lower servo angles (mechanism simulating isotonic muscle contraction) result in lower stiffness values and can be ideal for larger displacements translating from actuator to system/joint acted upon. Conversely, higher servo angels (mechanism simulating isometric muscle contraction) can be ideal for translating a larger percentage of actuator forces into the system acted upon.

## Data

![Stiffness Tabular Column](https://github.com/schen304joseph/team3.github.io/blob/main/Images/Capture1.PNG)

## Plots & Figures

![Stiffness Graph](https://github.com/schen304joseph/team3.github.io/blob/main/Images/Capture.PNG)
