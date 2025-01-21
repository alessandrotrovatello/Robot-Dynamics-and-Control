# Robot Dynamics and Control

This repository contains some exercises completed during the _Robot Dynamics and Control_ course at the University of Genoa.

## [2R Planar Robot](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/tree/main/2R_planar_robot)

In this folder there are some exercises on a **Planar Robot** with 2 **revolute** joints.

![image](https://github.com/user-attachments/assets/afa6b5bb-ffee-4e74-93ef-3cde9877a974)

The set of parameters of the model are as follows:

- **Mass of link 1**: 10.5 Kg
- **Length of link 1**: 600 mm
- **Mass of link 2**: 2 Kg
- **Length of link 1**: 450 mm

### Ex 1: Statics
[Ex 1.1](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_planar_robot/Ex_1_1.slx
). Set joint positions at q = [-30°, 30°]. Implement gravity compensation using the manipulator statics.

[Ex 1.2](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_planar_robot/Ex_1_2.slx
). Implement gravity compensation in the same configuration using the manipulator statics considering a spherical end-effector of mass M<sub>ee</sub> = 0.1 Kg and two additional masses (modeled as a spherical objects): one of 2.6 Kg placed on link 1 at 1/3 of its total length, the other one of 7 Kg placed on link 2 at 2/3 of its total length.

### [Ex 2](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_planar_robot/Ex_2.slx): Newton-Euler Algorithm

Implement the Newton-Euler algorithm for recursive inverse dynamics. Generate a cubic polynomial trajectory with the following initial and final configurations: 𝑞<sub>i</sub> = [-50°, 20°], 𝑞<sub>f</sub> = [85°; -40°]. Consider gravity effect. Do not consider damping in the joints. 

### [Ex 3](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_planar_robot/Ex_3.slx): Control

Implement the Computed Torque control law using the Robotics System Toolbox blocks. Generate a quintic polynomial trajectory with the following initial and final configurations: 𝑞<sub>i</sub> = [-90°, 10°], 𝑞<sub>f</sub> = [−40°; 30°]. Also, the trajectory should pass by an intermediate  joint configuration 𝑞 = [0°,  55°]. Also consider gravity action. 

## [2R Spatial Robot](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/tree/main/2R_spatial_robot)

Here, the robot is considered in 3D space. With respect to the previous model, the second joint axis is orthogonal to first joint axis. The gravity act along the y-axis of the world frame, with negative direction.

![image](https://github.com/user-attachments/assets/ad013649-afa0-44a3-ae66-34c9ae8df0fe)

The set of parameters of the model are as follows:

- **Mass of link 1**: 5 Kg
- **Length of link 1**: 200 mm
- **Mass of link 2**: 4.5 Kg
- **Length of link 1**: 180 mm

### Ex 1: Statics
[Ex 1.1](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_spatial_robot/Ex_1_1.slx
). Consider the joint configuration q = [10°, 35°] . Implement gravity compensation using the manipulator statics.

[Ex 1.2](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_spatial_robot/Ex_1_2.slx
). Implement gravity compensation in the same configuration of ex. 1, using the manipulator statics considering a spherical end-effector of mass M<sub>ee</sub> = 2.5 Kg and an additional mass of 6 Kg (modeled as a spherical object) placed on link 2 at 1/3 of its total length. 

### [Ex 2](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_spatial_robot/Ex_2.slx): Newton-Euler Algorithm

Implement the Newton-Euler algorithm for recursive inverse dynamics. Generate a cubic polynomial trajectory with the following initial and final configurations: 𝑞<sub>i</sub> = [15°,−50°], 𝑞<sub>f</sub> = [75°;0°]. Consider gravity effects. Do not consider damping in the joints.

### [Ex 3](https://github.com/alessandrotrovatello/Robot-Dynamics-and-Control/blob/main/2R_spatial_robot/Ex_3.slx): Control

Implement the Computed Torque control law using the Robotics System Toolbox blocks. Generate a quintic polynomial trajectory with the following initial and final configurations: 𝑞<sub>i</sub> = [-50°, 20°], 𝑞<sub>f</sub> = [−10°; 60°]. Also, the trajectory should pass by an intermediate  joint configuration 𝑞 = [20°,  85°]. Also consider gravity action.
