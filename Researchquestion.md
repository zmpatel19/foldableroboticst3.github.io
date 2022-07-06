---
title: Defining Research Question
---


# Research Question


### Introduction:

Most modern day actuators feature high precision, but are often constrained to either dynamic or kinematic control. In other words, they can, to a high degree of precision, work with complex control systems to control either torque outputs or speed/acceleration. 

Take for example Spot, a commercially available 4 legged robot developed by Boston Dynamics. Spot is built with some of the most precise servo motors that are embedded within the robot’s leg assembly to mimic complex biomechanical properties of legged motion. Hopping, one of the modalities of legged motion requires motors to emulate the characteristics of springs (exhibiting stiffness). This is achieved by means of a complex control system that positionally controls torque outputs of the motors/servos under actuation in a closed loop over the entire duration.

When it comes to terrain based control, the engineers behind Spot have managed to build a recognition engine that classifies most types of real world terrain. This information is ultimately used to change parameters of the control system that would result in altered legged movement dynamics (stiffness and damping properties) and would thus suit the characteristics of the terrain. Here, one would recognise a number of limitations with such a ridgid/complex system (the most crucial ones are highlighted by asking the following questions):

1. What if the robot is challenged with a completely new (untrained) terrain, whose properties are not characterised/highly irregular (e.g. a sandy substrate featuring large pubbles on its surface)?

2. What if the robot is subjected to unexpected perturbations?

3. What is the maximum frequency with which the robot can respond to these perturbations? I.e. is there a servo bandwidth limitation?


Series Elastic Actuators (SEAs) have been used to solve one of these problems. Essentially, SEAs are traditional actuators coupled with stiffness/elastic elements to provide ridgid-compliant actuation. Stiffness of at joint may be controlled by introducing a displacement of the fixed end of the stiffness/elastic element using the traditional actuator. SEAs allow joint stiffness to be applied as a result of mechanical elastic deformation - allowing these joints to operate efficiently under high frequency work loops when required.

Artificial Muscles are a new class of SEA actuators that has been gaining interest and research thrusts over the last few decades. This new class of actuators promises to bring high power density actuators with better responsiveness. These actuators closely replicate vertibrate muscle tissue flexion and extension, and have been predicted to replace traditional actuators especially in the fields of robotics, biomedical engineering, exoskeletons and prosthetic devices. Below are a few attempts at artificial muscles:

1. Twisted fiber consisting of fabric and Shape Memory Alloys (SMA) 

2. Pneumatic actuators (University of Tokyo)

3. Piezoelectric Elastomers (Harvard)

4. Origami Inspired artificial muscle to replicate human bicep flexion

### Research Question:

Legged motion is one of the most demanding and highly cycled movements in any land based vertebrate. Naturally, this makes muscle dynamics during legged motion an ideal benchmark for our experiments. Through this project, our team will try to investigate if such an artificial muscle can be tuned to match stiffness and damping properties of muscles involved in legged motion. Through this project, we aim to answer the following research questions:

Can an elemental artificial muscle be designed to reproduce the same biomechanical properties as that of muscles involved in legged motion?

### Tractability:
Our approach would be to first compile data that spans force and torque requirements of muscles that are crucial for legged motion. Doing so would allow us to build a model that best replicates these stiffness and damping characteristics.

1. Our choice of materials would be prioritized according to:

2. Stiffness requirements

3. Cost of the material

The origami structure itself on which we have currently based our idea on is the extensively used Kresling mechanism[2]. 

As for the animal whose biomechanics we will be trying to replicate, we have decided to initiate our studies by sampling human bipedal movement as there is no lack of data when it comes to human gait studies.

### Novelty:
We have found that there have been a lot of applications of the “generalized artificial muscle” towards legged motion. However, since this class of actuators are still under development, we have not been able to find an application that results in promising legged motion. This provides us with a possible novelty factor.


Some references that we came across:

1. The journal “Re-foldable origami-inspired bidirectional twisting of artificial muscles reproduces biological motion”[1] has provided examples of origami-inspired muscle driven by pneumatic.

2. “Untethered control of functional origami microrobots with distributed actuation”[2] describes one of the mechanisms that we propose using towards developing the artificial muscle element

3. One of the papers that were referenced during the process is by Stuart Burgees from Bristol University who published about the topic of bioinspiration and biomimetics. This paper provides a review of biological mechanical linkage mechanisms found in animals that can be used for various real-world applications. This paper is used as a reference to understand and identify the range of kinematic functions that animals are able to perform and provide an opportunity to implement the bioinspired design. With the help of this paper, our team can understand and identify linkage mechanisms found in animal joints such as hinge, spherical, gliding joints, etc. Further, with the help of the Kresling model, we can design a linkage mechanism for our legged robot to enable rotating, oscillating or reciprocating motion. Origami structure will help us use foldable techniques. Something that sets out the research is understanding kresling mechanism and developing origamis structure to achieve motion similar to bio inspiration. Allowing high levels of integration with shared links and parallel operations focusing on motion.

4. Origami inspired structures have new design opportunities offering new possibilities to build deployable foldable mechanism to achieve shape transformation. There has been growing interest in finding new mechanisms to achieve more desirable motion. In this paper we will be looking at the kinematics of  Kresling structures and the dynamics of origami inspired structure for desirable motion. With the help of this paper we will be looking at implementing such structure for motion in legged robots. We will be looking at the aspects of bioinspired kinematics studies and dynamic motion studies.

### Open-Ended:

Our research question is structured to be open-ended that will permit a further and deeper investigation. As we are focusing on the pattern of the foldable mechanism and the control of the motion, the material of the structure can be further investigated. The research of material used for the origami-inspired actuator will maximize the performance of the actuator and possibly reduced the manufacturing cost.  Moreover, the application of the actuator can be further researched.

### Modular

Actuators are widely used in various robotics applications. As a result, the research of origami-inspired muscle can be implemented in a wide range of applications. A characteristic of the origami-inspired muscle is that it provides a damping effect which is similar to the pneumatic drive system. In this manner, the research of developing an origami-inspired actuator module is modular and can be implemented in other existing robotics systems.


### Team Fit

The team is interested in exploring new technologies that have not been utilized in diverse scenarios. By leveraging each member’s individual experience with software, hardware, and electronics, the bounds of bio-inspired design can be pushed. Throughout the semester the team hopes to learn new concepts through the course and apply them directly to the project. One of the most effective methods for understanding new technologies is applying them to proven mechanisms. Our team itends to learn ways of replicating bioinspired kinematics and dynamics, folding and joining techniques and their application. 

### Topic Fit

While typical robotic solutions struggle to mimic muscle motion and structure, the use of foldable robotics can make this easier. Foldable robotics utilizes linkages and joints to create unique motion that other mechanisms cannot. For example, a two dimensional motion such as a servo spinning can be transferred into a 3 dimensional actuation. Additionally, cyclic motion similar to walking is inherently easier with this type of mechanism. Applying a variable reduction is also a key aspect that can be leveraged to improve motion.


### References

[1] Z. Jiao, C. Zhang, J. Ruan, W. Tang, Y. Lin, P. Zhu, J. Wang, W. Wang, H. Yang, and J. Zou, “Re-foldable origami-inspired bidirectional twisting of artificial muscles reproduces biological motion,” Cell Reports Physical Science, vol. 2, no. 5, p. 100407, 2021. 

[2] Larissa S. Novelinoa, Qiji Zeb, Shuai Wub, Glaucio H. Paulinoa, and Ruike Zhaob, “Untethered control of functional origami microrobots with distributed actuation”

[3] S. Burgess, “A review of linkage mechanisms in animal joints and related bioinspired designs,” Bioinspiration & Biomimetics, 10-Jun-2021. [Online]. Available: https://iopscience.iop.org/article/10.1088/1748-3190/abf744. [Accessed: 07-Feb-2022]. 

[4] N. Kidambi and K. W. Wang , “On the Dynamics of Kresling Origami Deployment,” Available: https://arxiv.org/ftp/arxiv/papers/2003/2003.10411.pdf. 


