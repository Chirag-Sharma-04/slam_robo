# SLAM Navigation Robot

Welcome to the SLAM Navigation Robot project! This project involves the development of an autonomous robot capable of simultaneous localization and mapping (SLAM) using a Raspberry Pi 4B and ROS2 Humble. The robot uses various sensors, including a lidar, and is designed to navigate and create maps of its environment.

## Table of Contents

- [Introduction](#introduction)
- [Hardware](#hardware)
- [Software](#software)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Reference](#reference)


## Introduction

This project aims to build an autonomous SLAM navigation robot using a Raspberry Pi 4B, Arduino, and ROS2 Humble. The robot is designed to create a map of its environment and navigate autonomously within that map, making it suitable for applications in research, education, and hobbyist robotics.

## Hardware

### Components

- **Raspberry Pi 4B**: The central processing unit running ROS2 Humble.
- **Rplidar A1M8 Lidar**: Sensor for distance measurement and environment mapping.
- **Arduino**: Microcontroller for motor control and encoder data processing.
- **Encoder Motors**: Two motors for robot movement, controlled via a motor driver.
- **L298 Motor Driver**: Electronic device that drives the motors based on Arduino signals.
- **PC Command Centre**: For high-level control and monitoring.

### Hardware Diagram

![block diagram](https://github.com/user-attachments/assets/33b283b5-baea-43b9-8107-6f49b14c1c54)

## Software

### Key Technologies

- **ROS2 Humble**: The Robot Operating System running on the Raspberry Pi 4B.
- **Ubuntu 22.04 LTS**: The operating system for the Raspberry Pi.
- **SLAM Toolbox**: For SLAM operations and navigation.
- **Arduino Code**: For motor control and encoder feedback.


## Working 

https://github.com/user-attachments/assets/b889edf1-8d70-474d-8a2f-062cfd3fdc9f

https://github.com/user-attachments/assets/57495cd0-23d3-4e67-a990-98cff119ca28

### Prerequisites

- Raspberry Pi 4B with Ubuntu 22.04 LTS installed
- ROS2 Humble installed on the Raspberry Pi
- Arduino IDE for programming the Arduino


## Usage

### Running the Robot

- Run the real life robot:
  ```bash
  ros2 launch slam_robo launch_robot.launch.py
  ```

### Simulation

- Run simulations using Gazebo and RViz2:
  ```bash
  ros2 launch slam_robo launch_sim.launch.py world:=./src/slam_robo/worlds/obstacles.world
  ```
- Be inside your ros2 workspace for the world to load

https://github.com/user-attachments/assets/bb17e439-6686-43cf-a109-3dd77535f435

## Contributing

We welcome contributions to this project! If you have suggestions or improvements, please fork the repository and create a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Reference

- The Construct : https://www.youtube.com/watch?v=rZOxPGCn4QM&list=PL-6_gw-1x-od0hQmVsZQsGy5TvFgYoTPk&index=8
- Robotics Back-End : https://www.youtube.com/watch?v=idQb2pB-h2Q&list=PL-6_gw-1x-od0hQmVsZQsGy5TvFgYoTPk&index=7
- Udemy : https://www.udemy.com/course/self-driving-and-ros-2-learn-by-doing-map-localization/?couponCode=NVDIN35 (I have personally not done the course but have found the content to be helpful for new learners)
