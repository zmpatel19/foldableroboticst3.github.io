---
title: Researchquestion
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

### Research Question

Legged motion is one of the most demanding and highly cycled movements in any land based vertebrate. Naturally, this makes muscle dynamics during legged motion an ideal benchmark for our experiments. Through this project, our team will try to investigate if such an artificial muscle can be tuned to match stiffness and damping properties of muscles involved in legged motion. Through this project, we aim to answer the following research questions:

Can an elemental artificial muscle be designed to reproduce the same biomechanical properties as that of muscles involved in legged motion?


