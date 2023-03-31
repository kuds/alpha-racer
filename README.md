# Picar-V-ROS-2
Using the Picar-V and ROS 2 platforms to build an autonomous system that navigates a predefined track as quickly as possible

## Prerequisits
### Hardware
 - [Raspbery PI 4B](https://www.amazon.com/dp/B09LYP7QH3?ref_=cm_sw_r_apin_dp_VMXPRDF13GEB3HZ2BBBR)
 - [Picar-V](https://www.amazon.com/dp/B06XWSVLL8?ref_=cm_sw_r_apin_dp_KSH0WGD7QD2PA3DQH86D)
 - [Lipo Batteries](https://www.amazon.com/dp/B06XWSVLL8?ref_=cm_sw_r_apin_dp_KSH0WGD7QD2PA3DQH86D)

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

#### Chapter 2.2 - SLAM
Simultaneous Localization and Mapping, or SLAM, is a technique used in robotics and computer vision to simultaneously construct a map of an unknown environment and estimate the robot's location within that environment.

The SLAM problem arises when a robot needs to navigate in a new or previously unknown environment without a pre-built map of the surroundings. In order to solve this problem, the robot must use its sensors to gather information about the environment and use that information to construct a map of the surroundings. At the same time, the robot must estimate its own location within the map in order to be able to navigate effectively.

SLAM algorithms typically use a combination of sensor data such as LIDAR, cameras, and inertial measurement units (IMUs) to build a map of the environment and estimate the robot's location within that map. These algorithms use probabilistic methods to fuse sensor measurements over time, and can deal with uncertainty and errors in the sensor data.

SLAM is a critical technology for autonomous robots and self-driving vehicles, as it allows them to operate in new and changing environments without relying on pre-built maps.


