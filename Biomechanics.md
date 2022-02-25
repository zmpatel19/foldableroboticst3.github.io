---
title: Biomechanics
---

# Biomechanics Background and Initial Specifications

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



Studies by Shorter et al. [9] aimed to quantify these properties about the ankle (results provided in table of specifications). However, it should be noted that these properties are a result of tissue dynamics of a muscle-tendon compound. I.e. these do not explicitly deal with muscle fascicle properties. Nevertheless, this does cover important dynamics of joint properties that would eventually be important when it comes to muscle-tendon-joint interactions.

From this, we understand that stiffness and damping properties are a result of muscle-tendon compounds and do not arise purely from either of those. We must understand the kinetics of these individual components: the Gastrocnemius muscle and the Achilles tendon that attaches the Gastrocnemius muscle group to the Ankle Calcaneus:









![image caption](Biomechanics.JPG)
