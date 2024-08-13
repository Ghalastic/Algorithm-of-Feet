# Algorithm of Robot Feet
####
## Task Description:-
#### 
Write the algorithm of the design of the feet and the mechanism of the movement with support of possible images and designs.
#### 
## Introduction:
#### 
The design of humanoid robots has evolved from the serial design of the first humanoids to more refined architectures. And it’s safe to say that Humanoid robotics has fascinated and challenged scientists for decades. Despite the feet playing a key role in human motion, the mobility of most of these robots is still limited to the legs, arms, hands, and head only, with very few examples including the feet. The human foot architecture is characterized by three main segments, the heel, mid‐foot, and toes, that fulfill distinct roles during bipedal locomotion. Several research groups have tried to improve the foot performance by compensating for a limited mechanical design with an enhanced sensing/control capability, which can be obtained by adding force/pressure sensors to the foot plant. Foot designs with three segments have been proposed to better mimic human‐like motion but are usually characterized by active mechanisms that require complex control and motion coordination with the rest of the body.
#### 
### In this task, an innovative mechanism for robotic feet is presented that can adapt to the environment without the need for external actuation, all thanks to joint elasticity.
#### 
### 1- Requirements for Humanoid Foot Mechanisms:
#### 
To obtain the mobility requirements for humanoid foot mechanisms, the human gait was analyzed in terms of absolute and angular motion, The motion was acquired through a VICON Motion Capture system, with the following retroreflective marker set configuration and alignment: 
#### 
-	RA, right ankle marker: Placed at the level of the lateral malleolus.  
-	RT, right toe marker: Placed on the lateral aspect of the foot at the second metatarsal head.  
-	RQ, right heel marker: Positioned so that the heel-toe marker vector is parallel to (but offset from) the sole of the foot and is aligned with the foot progression line (i.e., the line from the ankle center to the space between the second and third metatarsal heads).  
-	LA, left ankle marker: Placed at the level of the lateral malleolus.   
-	LT, left toe marker: Placed on the lateral aspect of the foot at the second metatarsal head.   
-	LQ, left heel marker: Positioned so that the heel-toe marker vector is parallel to (but offset from) the sole of the foot, and is aligned with the foot progression line.
####
![leftfot](https://github.com/user-attachments/assets/09368972-34d3-4486-94b6-ebdc7e49aa45)
#### 
### Example of the marker placements on the left foot, with the left ankle (LA), left toe (LT) and left heel (LQ) markers.
#### 
![rightfot](https://github.com/user-attachments/assets/5bd567d6-aef2-47ea-8c0c-c2321ea7d0d9)
#### 
### Example of the marker placements on the right foot of a patient, with the right ankle (RA), right toe (RT) and right heel (RQ) markers.
#### 
### 2- An Underactuated Humanoid Foot Mechanism:
#### 
The proposed foot mechanism aims to enhance robot mobility and efficiency by enabling body support in all the stances. To do so, a three-segment design was considered. During the gait, the foot motion is ruled by four main centers of rotation, which correspond to the ankle joint, the heel bone (or calcaneus), the navicular tuberosity, and the metatarsophalangeal (MTP) joint, as shown in the next illustration.
####
![fig4](https://github.com/user-attachments/assets/e355b266-6b72-44b8-96bb-17036acff241)
####
-	The first segment of the foot can be associated with the calcaneus‐talus complex, which includes the heel and ankle and can be approximated to a rigid body.  

-	The motion of the central segment of the foot is enabled by the active stiffening behavior of the intrinsic foot muscles in the plantar arches, which connect the calcaneus to the MTP joint.  

-	The plantar fascia and several ligaments support the plantar arches, which store mechanical energy during weight bearing by deforming.   

-	The motion of the last segment of the foot can be approximated to a flexion/extension movement of the toes, which rotate around the MTP joint and the interphalangeal joints. The MTP joint is usually described as a condyloid joint, while the interphalangeal joints resemble revolute joints.  
#### 
To replicate the behavior of the human foot, a new compliant foot mechanism based on the kinematic scheme in the next figure is here presented. The proposed mechanism is based on a compliant mechanism in the plant, which can be approximated with a revolute‐revolute‐prismatic‐revolute architecture, with revolute joints in points B, C, and D, and a link of varying length between B and D.
#### 
![fig6](https://github.com/user-attachments/assets/964573fc-6532-420d-a9bf-f8841f37e685)
#### 
The mechanism works mainly on the sagittal plane, even if the compliant part can be designed to balance 3D loads as well. When analyzing the planar behavior of the proposed foot design, its degrees of freedom can be evaluated from its rigid mechanism which is equivalent to two. controlled respectively by the plantar-compliant element and by the torsional spring of the MTP joint. A design example of the proposed foot mechanism is shown in the next figure.
#### 
![fig7](https://github.com/user-attachments/assets/41ef99aa-5796-4edc-aeff-3306d0396529)
####
### 3- Simulation and Results:
#### 
The results can be observed in the step‐by‐step effect of the load on the different bodies of the humanoid foot:
####
![fig 10](https://github.com/user-attachments/assets/2c7f0d04-8f13-4e9f-852a-31990e7b41bc)
#### 
-	Starting from the rigid body of the hindfoot, the angular displacement is applied to the ankle joint. The hindfoot is connected to the flexible body of the midfoot, which starts to deform.   
-	When the angular displacement causes the foot to hit the ground, the midfoot is characterized by a stress concentration in the upper part.   
-	The arc bottom part of the foot is loaded with a maximum tension of 1.57 × 106 N/m2, behaving as the human foot muscle when stepping.   
-	The spring connecting the two bodies of the forefoot is stretched. This helps the foot to adapt to the ground, and the potential energy of the spring restores the neutral ‘flat’ position when the contact is released.  
#### 
These results validate the behavior of the proposed humanoid foot, showing that it acts similarly to the human foot in terms of stress while walking. Furthermore, the results prove that the proposed design can safely withstand the loads associated with an average human gait, including the impact of the foot on the ground.
#### 
## References:- 
#### 
[A Bioinspired Humanoid Foot Mechanism](https://www.mdpi.com/2076-3417/11/4/1686)
#### 
