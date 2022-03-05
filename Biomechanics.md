---
title: Biomechanics
---

# Biomechanics Background and 

###  Bioinspiration & assumption

Since our project would be dealing with the designing of a novel artificial muscle concept, we decided to start by finding a muscle group that we could use as a benchmark for designing and comparing our artificial muscle to. Doing so would give us an idea of the stiffness and forces to be replicated in our own Series Elastic Element (SEE) actuator and eventually, a novel artificial muscle concept. Thus, we needed tensions and stiffness data that directly correlated to Isometric and Isotonic muscle activation.

For this, we referred to various articles that dealt with muscle groups in Humans that were crucial to the gait modality of running. We chose running as it is one of the most highly cyclic and energetic movements of the human body. Furthermore, since most human gait related biomechanics studies were performed in controlled laboratory environments, we needed to be sure we had minimal - if not negligible differences between treadmill and open ground running when selecting the most performing muscle group. 

### Selection of muscle group to study:

For this, we used the data produced by Riley et al. [6]. Here, we found that the ankle joint produced the most moments. The table below shows some of the normalized moment data collected over 20 healthy Human subjects during running over treadmill:


| Joint         | Moment (N-m/kg) |
| ------------- |:-------------:| 
| Hip extension | 1.3                
Hip abduction | 0.32
Knee flexion | 1.7
Knee varus | 1.5
Ankle plantarflexion | 4.01

Table 1: muscle group selection

From the anatomy of the human ankle (Fig. 1), we see that the group of muscles known as Triceps Surae, consisting of the Gastrocnemius and Soleus muscles act on the ankle. These muscles are attached to the Calcaneus bone (which serves as a lever arm for the foot) through the Achilles tendon. On further investigation, we found that there was no shortage of literature on biomechanical properties of these muscle groups. Thus, we determined that the Gastrocnemius muscle was to be used as a benchmark to study muscle dynamics.

### Ankle impedance studies:

Human gait can be simplified to model a second degree inverse pendulum system. This system is governed by the equation:

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/Eqn.JPG)

Studies by Shorter et al. [9] aimed to quantify these properties about the ankle (results provided in table of specifications). However, it should be noted that these properties are a result of tissue dynamics of a muscle-tendon compound. I.e. these do not explicitly deal with muscle fascicle properties. Nevertheless, this does cover important dynamics of joint properties that would eventually be important when it comes to muscle-tendon-joint interactions.

From this, we understand that stiffness and damping properties are a result of muscle-tendon compounds and do not arise purely from either of those. We must understand the kinetics of these individual components: the Gastrocnemius muscle and the Achilles tendon that attaches the Gastrocnemius muscle group to the Ankle Calcaneus:

### Gastrocnemius muscle fascicle studies:

This muscle group has been extensively studied under Human walking and running conditions. This muscle actuates the ankle dorsiflexion movement. Muscle forces generated under contraction are translated to the ankle through the Achilles Tendon. The anatomy of the muscle reveals that it is a pennate type of muscle (fascicles attach at a slanting angle, Fig. 2). Details on the muscle contraction kinematics are explained in the Engineering Representation section.
We extracted the muscle forces and displacement ranges [10,11] and are detailed in the Table of Specifications section.

### Achilles tendon studies:

The Achilles tendon provides the major component of ankle stiffness. Studies have shown that during running, the displacement of the Calcaneus bone is not entirely translated to muscle contraction. This difference between calcaneus and muscle displacements have been found to be converted to strain energy stored by the Achilles tendon.
Energy is stored in the Achilles Tendon during Isometric contraction of the Triceps Surae muscles group. Achilles Tendon stiffness and kinematics has been measured in previous studies [12,13] and have been reported in the Table of Specifications section.

### Citations used:

1. A kinematics and kinetic comparison of overground and treadmill running. [6]
2. Ankle mechanical impedance during the stance phase of running. [9]
3. Muscle fascicle and series elastic element length changes along the length of the human gastrocnemius during walking and running [10]
4. Experimental determination of force-length relations of intact human gastrocnemius muscles [11]
5. Achilles tendon strain energy in distance running: consider the muscle energy cost [12]
6. Changes in Achilles tendon stiffness and energy cost following a prolonged run in trained distance runners [13]

| Parameter | Unit | Range of Values | Reference
| -------- | ------- | --------- | --------- 
| Ankle Stiffness Constant (Impedance studies) | Nm/rad/kg | 2 - 13 | [9]
| Ankle Damping Constant (Impedance studies) | Nms/rad/kg | 0.01 - 0.07 | [9]
| Ankle Angular Displacement | degrees | -25 - 10 | [9]
Ankle Net Torque|Nm/kg|0 - 2|[9]
AT Max Stiffness|N/mm|328 - 500|[6]
GM Max Isometric Force|N|2500 - 3000|[11,12]
Average Subject Mass|kg|47.8 - 76|[9, 6, 11, 12]

### Existing bio-inspired research

### List of 5 bio-inspired human robot
1. Robotic Leg via pneumatic muscle actuators* [1]
2. Anthropomorphic Walking Robot LOLA* [2]
3. Supercoiled Polymer Artificial Muscle [3]
4. Series Elastic Actuators for legged robots [4]
5. Hydraulic artificial muscles* [5]

### 3 most useful citation for initial specifications

*1. In this article a human inspired robotic leg is presented with pneumatic muscle actuation (PMA’s). The objective of the paper is to develop a pneumatic form of actuation possessing the parameters to mimic the motion characteristics of a human ankle. It provides a good basis to study postural control and prosthetic limbs. Pneumatic Muscle Actuator, is characterized by reducing the length when pressurized and providing properties of those of the organic muscles. The proposed design in this article consists of 4 PMA’s for producing 2 degrees of freedom movement similar to the human ankle which are plantar flexion and inversion. To generate this kind of motion a muscle tendon based approach is used. The four PMA’s act and provide direction by reducing the length of selective ones based on the  pneumatic input.

*2. The second article that our group thinks is closely related to our research topic is about a full size human robot LOLA. The objective of the robot is to achieve fast and human like locomotion and increase autonomous guided walking capabilities. LOLA shows active toe joints that allow the control of the center of the pressure that is exerted during heel rise. The area of contact helps to stabilize the robot and provide forward motion. At the same time heel rise in human gait contributes significantly to reducing the center of mass during displacement of the robot. During motion feet is the only part that is being reacted upon with ground forces. They are the last link in motion to provide acceleration. The main requirements in order to develop a functional foot include high grip on different surface, good damping and shock attenuation mechanism, rigid mechanical structure and minimal weight. These are some of  the important parameters that we can extract from this paper to design our muscle that can counteract those forces and provide desired motion.   

*3 Despite the fact that the actuation mechanism is identical to that of pneumatic artificial muscles, hydraulic artificial muscles have received little attention. When compared to typical fluidic cylinder actuators, hydraulic artificial muscles have all of the same benefits of pneumatic artificial muscles, such as compliance, light weight, minimal maintenance, and cheap cost. The characterisation of muscles under isometric and isobaric situations is explored, and pneumatic artificial muscles are contrasted. A quasi-static model is described that incorporates the effects of mesh angle, friction, and muscle volume change during actuation. The paper is valuable to the project as it discusses how to implement hydraulic muscles to the muscle structure mentioned in the engineering representation section below.

### Figures from literature

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/1.JPG)

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/2.JPG)

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/3.JPG)

### Engineering representation

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/4.JPG)

![alt text](https://github.com/schen304joseph/team3.github.io/blob/Zaki-Patel/Images/5.JPG)

The mechanical drawing of the muscle system contains 3 links. Number 1 in Figure 5 can be considered as a rigid part in the system. Link number 2 and 3 can be considered as massless as they are the moving part of the system. The link of number 3 in Figure 5 represents the ligament which acts as a spring to provide stiffness to the system. Number 2 in Figure 5 represents the natural muscle which acts as an actuator of the system.

### Discussion

Based on the research our team has done there are many existing solutions regarding artificial inspired muscle. We planned to replicate the muscle on a human's leg with a foldable robotics mechanism. In terms of the size of the muscle, we plan to construct a muscle with a smaller scale and focus on the foldable mechanism design. The muscle then can be scaled up to its desired application. Since we are replicating a general muscle actuator, there are not many constraints in terms of the material selection. Testing different materials and choosing the material with best performance under a budget can be an objective of the project.

Research suggests that natural muscle has 0.4-40 J/kg energy density. [7] Also, some human muscles can output over 2000 watts of power. [8]. It’s hard to choose a motor to compare with a natural muscle that produces non-linear power output. Moreover, there are many factors that result in different power output. For example, each person has a different muscle to fat ratio which results in muscle densities difference. To attain the power output of natural human muscle our team found a brushless DC motor which can output 2000 watts of power. However, the actuator weighs 12 kg excluding the power supply. Power supply which is capable of outputting 2000 W can weigh 45kg which is over the average weight of a human. As a result we conclude that natural muscle has more power density compared to electrical power.

### Bibliography
1. Andrikopoulos, George, and George Nikolakopoulos. “Humanoid Robotic Leg via Pneumatic Muscle Actuators: Implementation and Control.” Meccanica, vol. 53, no. 1-2, 2017, pp. 465–480., https://doi.org/10.1007/s11012-017-0738-6. 

2. S. Lohmeier, T. Buschmann, and H. Ulbrich, “System design and control of anthropomorphic walking robot Lola,” IEEE/ASME Transactions on Mechatronics, vol. 14, no. 6, pp. 658–666, 2009. 

3. J. Zhang, “Modeling of a bending supercoiled polymer (SCP) artificial muscle,” IEEE Robotics and Automation Letters, vol. 5, no. 3, pp. 3822–3829, 2020. 

4. J. E. Pratt and B. T. Krupp, “,” SPIE Proceedings, 2004. 

5. “Hydraulic artificial muscles.” [Online]. Available: https://people.csail.mit.edu/cmm386/publications/hams_journal_paper.pdf. [Accessed: 14-Feb-2022]. 

6. Riley, P. O., Dicharry, J., Franz, J., Croce, U. della, Wilder, R. P., & Kerrigan, D. C. (2008). A kinematics and kinetic comparison of overground and treadmill running. Medicine and Science in Sports and Exercise, 40(6), 1093–1100. https://doi.org/10.1249/MSS.0b013e3181677530

7. “Dielectric elastomer actuator,” Biomimetic Robotic Artificial Muscles, pp. 179–200, 2013. 

8. O. C. Ozcanli, "Turning Body Heat Into Electricity," Forbes, 8 Jun 10.

9. Shorter, A. L., & Rouse, E. J. (2020). Ankle mechanical impedance during the stance phase of running. IEEE Transactions on Biomedical Engineering, 67(6), 1595–1603. https://doi.org/10.1109/TBME.2019.2940927

10. Lichtwark, G. A., Bougoulias, K., & Wilson, A. M. (2007). Muscle fascicle and series elastic element length changes along the length of the human gastrocnemius during walking and running. Journal of Biomechanics, 40(1), 157–164. https://doi.org/10.1016/j.jbiomech.2005.10.035

11. Herzog Phd’, W., Read Msc’ H E D J Ter, L. J., & Phd, K. (1991). Experimental determination of force-length relations of intact human gastrocnemius muscles. In Clinical Biomechanics (Vol. 6).

12. Fletcher, J. R., Macintosh, B. R., & Fletcher, J. R. (2015). Achilles tendon strain energy in distance running: consider the muscle energy cost. J Appl Physiol, 118, 193–199. https://doi.org/10.1152/japplphysiol.00732.2014.-The

13. Fletcher, J. R., & MacIntosh, B. R. (2018). Changes in Achilles tendon stiffness and energy cost following a prolonged run in trained distance runners. PLoS ONE, 13(8). https://doi.org/10.1371/journal.pone.0202026
