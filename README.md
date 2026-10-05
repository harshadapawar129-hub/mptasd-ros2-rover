# MPT-ASD ROS 2 Rover

ROS 2 simulation and development of a six-wheel rocker-bogie rover based on the MPT-ASD project.

## Project Overview

This project focuses on developing a mobile robotic platform using ROS 2. The rover uses a six-wheel rocker-bogie suspension system designed for improved mobility over uneven terrain.

The ROS 2 version of the project is being developed as a simulation and robotics portfolio project.

## Current Progress

- [x] ROS 2 workspace setup
- [x] ROS 2 package creation
- [x] URDF/Xacro rover model
- [x] Six-wheel rocker-bogie structure
- [x] Robot State Publisher
- [x] TF2 visualization
- [x] RViz visualization
- [ ] Gazebo physics simulation
- [ ] Collision and inertial properties
- [ ] ros2_control
- [ ] Wheel control
- [ ] LiDAR
- [ ] IMU
- [ ] Camera
- [ ] SLAM
- [ ] Nav2 autonomous navigation
- [ ] 4-DOF robotic arm
- [ ] MoveIt 2
- [ ] Color detection
- [ ] Pick-and-place

## Software

- Ubuntu 22.04
- ROS 2 Jazzy
- Gazebo Harmonic
- RViz2
- URDF
- Xacro
- TF2
- ros2_control
- SLAM Toolbox
- Nav2
- MoveIt 2
- OpenCV

## Robot

### Configuration

- Six-wheel rocker-bogie suspension
- Differential drive concept
- Six DC gear motors
- 10 cm wheel diameter
- Custom rover chassis

## Current Stage

The current model has been successfully visualized in RViz using URDF/Xacro, Robot State Publisher and TF2.

The next stage is to add physics simulation in Gazebo Harmonic.

## Future Work

The final objective is to develop a complete autonomous mobile manipulation platform capable of:

1. Traversing uneven terrain
2. Mapping its environment
3. Autonomous navigation
4. Object detection and color classification
5. Robotic arm manipulation
6. Pick-and-place operations

