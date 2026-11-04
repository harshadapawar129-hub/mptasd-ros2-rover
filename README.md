# MPT-ASD ROS 2 Rover

A ROS 2-based simulation and navigation project for a six-wheel mobile robot.

The project focuses on developing a mobile robotic platform capable of traversing uneven terrain, mapping its environment, and performing autonomous navigation. It is part of the broader **MPT-ASD (Mobile Platform for Traversal, Articulation, and Spectral Differentiation)** project.

## Project Overview

MPT-ASD is a six-wheel  rover designed for mobile robotics applications.

This repository contains the ROS 2 implementation, including the robot model, Gazebo simulation, wheel control, LiDAR integration, environment mapping, and ongoing Nav2 integration.

## Current Progress

| Component                        | Status      |
| -------------------------------- | ----------- |
| ROS 2 workspace and package      | Completed   |
| URDF/Xacro robot model           | Completed   |
| Six-wheel rocker-bogie structure | Completed   |
| RViz visualization and TF2       | Completed   |
| Gazebo simulation                | Completed   |
| ros2_control integration         | Completed   |
| Differential-drive wheel control | Completed   |
| LiDAR integration                | Completed   |
| SLAM-based environment mapping   | Completed   |
| Map saving                       | Completed   |
| Nav2 integration                 | In progress |
| Autonomous navigation tuning     | In progress |


## Technology Stack

- Ubuntu 24.04 LTS
- ROS 2 Jazzy
- Gazebo Harmonic
- RViz2
- URDF and Xacro
- TF2
- ros2_control
- Gazebo Sim ROS 2 Control
- LiDAR
- SLAM Toolbox
- Nav2
- Python

## Robot Configuration

- Six-wheel rocker-bogie suspension
- Differential-drive control
- Six-wheel configuration
- Custom rover chassis
- Simulated LiDAR sensor

### Simulation Parameters

| Parameter         | Value     |
| ----------------- | --------- |
| Wheel radius      | 0.05 m    |
| Wheel separation  | 0.47 m    |
| LiDAR samples     | 720       |
| LiDAR update rate | 10 Hz     |
| LiDAR range       | 0.12–12 m |

These values describe the current simulation and controller configuration.

## SLAM and Mapping

The rover has been integrated with LiDAR-based environment mapping using SLAM Toolbox.

A map generated during simulation has been saved in the repository:

- `rover_map.pgm`
- `rover_map.yaml`

The mapping stage provides the environment map for the ongoing navigation integration.

## Repository Structure

```text
mptasd-ros2-rover/
├── README.md
├── .gitignore
├── rover_map.pgm
├── rover_map.yaml
├── docs/
│   ├── tf_tree.pdf
│   └── tf_tree.gv
└── src/
    └── mptasd_description/
        ├── config/
        ├── launch/
        ├── urdf/
        ├── worlds/
        ├── CMakeLists.txt
        └── package.xml
```

## Installation and Setup

### Prerequisites

- Ubuntu 24.04
- ROS 2 Jazzy
- Gazebo Harmonic
- Required ROS 2 packages and simulation dependencies

### Clone the Repository

```bash
git clone https://github.com/harshadapawar129-hub/mptasd-ros2-rover.git
cd mptasd-ros2-rover
```

### Build the Workspace

```bash
source /opt/ros/jazzy/setup.bash
colcon build --symlink-install
source install/setup.bash
```

### Launch RViz Visualization

```bash
ros2 launch mptasd_description display.launch.py
```

### Launch Gazebo Simulation

```bash
ros2 launch mptasd_description gazebo.launch.py
```

## Future Development

- Complete Nav2 autonomous navigation and goal execution.
- Improve localization and navigation performance.
- Tune obstacle avoidance and costmaps.
- Integrate additional sensors such as an IMU.

Project Goal

The long-term objective is to develop a mobile manipulation platform that combines mobility, environment perception, autonomous navigation, and robotic arm operations into a single system.

