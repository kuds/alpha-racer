# Picar-V-ROS-2
Using the Picar-V and ROS 2 platforms to build an autonomous system that navigates a predefined track as quickly as possible

## Prerequisits
### Hardware
 - [Raspbery PI 4B](https://www.amazon.com/dp/B09LYP7QH3?ref_=cm_sw_r_apin_dp_VMXPRDF13GEB3HZ2BBBR)
 - [Picar-V](https://www.amazon.com/dp/B06XWSVLL8?ref_=cm_sw_r_apin_dp_KSH0WGD7QD2PA3DQH86D)
 - [Lipo Batteries](https://www.amazon.com/dp/B06XWSVLL8?ref_=cm_sw_r_apin_dp_KSH0WGD7QD2PA3DQH86D)
 - [Raspberry Pi Camera Module 3](https://www.seeedstudio.com/Raspberry-Pi-Camera-3-p-5574.html?queryID=976e3c95a6cc2c6cca4fe95f3674438b&objectID=5574&indexName=bazaar_retailer_products)
 - [Coral USB Accelerator](https://www.seeedstudio.com/Coral-USB-Accelerator-p-2899.html?queryID=e2a50252acb7b76b6a30810d2c9f5476&objectID=2899&indexName=bazaar_retailer_products)

### Software
 - [Raspberry PI Imager](https://www.raspberrypi.com/software/)
 - [Visual Studio Code](https://code.visualstudio.com/)

### Helpful Links
 - [Picar-V Instruction Manual](https://docs.sunfounder.com/projects/picar-v/en/latest/)
 - [korzen - PiCar_ROS Repo](https://github.com/korzen/PiCar_ROS)
 - [Roslibpy](https://roslibpy.readthedocs.io/en/latest/)
 - [Raspberry Pi ROS Python Publisher GPIO State (ROS 1)](https://roboticsbackend.com/raspberry-pi-ros-python-publisher-publish-a-gpio-state/)
 - [ROS Client Library for the Python](https://github.com/ros2/rclpy)
 - [ROS 2 Rclpy Parameter Callback](https://roboticsbackend.com/ros2-rclpy-parameter-callback/)
 - [Rosdep](https://docs.ros.org/en/independent/api/rosdep/html/)
 - [DeepPicar](https://github.com/dctian/DeepPiCar)
 - [Nav2](https://navigation.ros.org/)

## Software Setup
 - [Ubuntu Server (22.04.2 LTS)](https://ubuntu.com/download/server)
 - [ROS2 Humble](https://docs.ros.org/en/humble/index.html)

### Chapter 1 - Setting up Raspberry PI

#### Chapter 1.1 - PWM
It's possible that you meant PWM, which stands for Pulse Width Modulation. PWM is a technique used in electronic circuits to control the amount of power delivered to a load, such as a motor, LED or speaker.

In PWM, the signal switches between a high and low state at a fixed frequency, and the duration of the high state (known as the duty cycle) is varied to control the amount of power delivered to the load. By rapidly turning the signal on and off, the load sees an average voltage or current that can be precisely controlled by adjusting the duty cycle.

PWM is widely used in a variety of applications, including motor speed control, LED brightness control, and audio amplifiers.

#### Chapter 1.2 - GPIO
GPIO stands for General Purpose Input/Output, which is a common interface found on microcontrollers, single-board computers, and other electronic devices. GPIO allows the device to interact with the outside world by providing a way to send and receive digital signals.

GPIO pins are typically configured as either inputs or outputs. Input pins allow the device to read the state of a connected sensor or other external device, while output pins allow the device to send a signal to control an external device, such as turning on an LED or activating a motor.

GPIO pins are typically controlled using software, either through low-level programming or through higher-level libraries and APIs. The specific functions and capabilities of GPIO pins can vary depending on the device and the software environment.

GPIO is a versatile and powerful interface that is used in a wide range of applications, from simple hobby projects to complex industrial control systems.

### Chapter 2 - Navigating and Rout Planning

#### Chapter 2.1 - Navigation
There are several navigation techniques that are commonly used in robotics. Here are some of the most common ones:

Odometry: This technique involves using sensors to measure the distance traveled by a robot's wheels. By keeping track of the number of rotations and the wheel size, the robot can estimate its position and orientation relative to its starting point.

Inertial Navigation: This technique involves using sensors that measure the robot's acceleration and rotation to estimate its position and orientation. This technique is commonly used in autonomous vehicles and drones.

GPS Navigation: This technique involves using GPS satellites to determine the robot's position on the earth's surface. GPS navigation is commonly used in outdoor environments.

Laser-based Navigation: This technique involves using a laser scanner to measure the distance between the robot and its surroundings. By creating a 2D or 3D map of the environment, the robot can navigate autonomously.

Vision-based Navigation: This technique involves using cameras to capture images of the robot's surroundings. By processing these images, the robot can determine its position and orientation and navigate autonomously.

SLAM: Simultaneous Localization and Mapping (SLAM) is a technique used to build a map of an unknown environment while at the same time navigating through it. This technique involves combining data from sensors such as odometry, laser scanners, and cameras to create a map of the environment and estimate the robot's position and orientation within it.

Path Planning: Path planning involves generating a trajectory or a set of actions for the robot to follow in order to reach a specific goal. This technique takes into account the robot's current position, the environment, and any obstacles in the way. It can be used in combination with any of the above navigation techniques.

#### Chapter 2.2 - SLAM
Simultaneous Localization and Mapping, or SLAM, is a technique used in robotics and computer vision to simultaneously construct a map of an unknown environment and estimate the robot's location within that environment.

The SLAM problem arises when a robot needs to navigate in a new or previously unknown environment without a pre-built map of the surroundings. In order to solve this problem, the robot must use its sensors to gather information about the environment and use that information to construct a map of the surroundings. At the same time, the robot must estimate its own location within the map in order to be able to navigate effectively.

SLAM algorithms typically use a combination of sensor data such as LIDAR, cameras, and inertial measurement units (IMUs) to build a map of the environment and estimate the robot's location within that map. These algorithms use probabilistic methods to fuse sensor measurements over time, and can deal with uncertainty and errors in the sensor data.

SLAM is a critical technology for autonomous robots and self-driving vehicles, as it allows them to operate in new and changing environments without relying on pre-built maps.
