# Task 1 : Gazebo-Making Our Own and Testing Environments

## Overview

In this module, we will use Gazebo simulator software to create a virtual drone and test it in customized environments. Our primary objective is to gather parameters specific to Bangalore UVCE and create a simulated environment based on these parameters.

## Prerequisites

- **Software:** Gazebo Simulator
- **Operating System:** Ubuntu
- **Availability:** 2 PCs with Ubuntu installed

### Resources

- [Gazebo Official Website](https://gazebosim.org/home)
- Secure SDF files needed for the Gazebo simulator to facilitate environment customization.

## Environment Setup

1. **Install Gazebo:** Ensure Gazebo is installed on Ubuntu laptops.
2. **World Installation:** Confirm that the Gazebo worlds are correctly installed and functional.
3. **Parameter Collection:** Gather parameters specific to the Bangalore UVCE environment for accurate simulation.



# Task 2: Design a Leg for a Quadcopter Frame

## Objective

Design a leg for a quadcopter frame using the dimensions of the standard T50 frame design for quadcopters. Utilize the generative design tools in Fusion 360 to complete this task with a focus on weight reduction while maintaining the structural stiffness of the leg.

## Steps

1. **Understand Generative Design Environment:**
   - Gain a thorough understanding of how to operate the generative design environment in Fusion 360.
   - Learn about the use of **Obstacle Geometry**, **Preserve Geometry**, and **Starting Shape**.

2. **Design Considerations:**
   - Weight reduction of the legs is a high priority.
   - Ensure that the structural stiffness of the legs is not compromised.

3. **Resource:**
   - Use the following playlist to understand the generative design environment: [Fusion 360 Generative Design Playlist](https://www.youtube.com/watch?v=sps-OR60fVU&list=PLEzzQIuBvBkr7tNcgERS9IIxLSPbb8A6M).

## Design Process

1. **Dimensions:**
   - Use the dimensions of the standard T50 frame design for quadcopters.

2. **Generative Design Tools:**
   - Launch Fusion 360 and navigate to the generative design workspace.
   - Define **Preserve Geometry** to specify the areas of the design that must remain unchanged.
   - Set up **Obstacle Geometry** to define the areas that the generated design should avoid.
   - Determine the **Starting Shape** to guide the initial design process.

3. **Optimization:**
   - Apply constraints and objectives focused on minimizing weight while ensuring the design meets structural requirements.

4. **Evaluation:**
   - Analyze the generated design outcomes and select the optimal design for manufacturing.

5. **Iteration:**
   - Refine the design based on the initial outcomes and repeat the process as needed to achieve the best results.

## Conclusion

By completing this task, you will gain practical experience in using generative design tools to create optimized components for quadcopters. This exercise emphasizes the importance of balancing weight reduction and structural integrity in design engineering.



# Task 3 : Using ROS and Companion Board

## Objective

In this task, we will add a camera, LIDAR, or IR sensor to the drone and attach it to the companion board. We will send the data from these sensors to implement an AI model. The task will be implemented in two parts:

### Part 1: Sensor Setup

1. **Install Sensors:** Attach a camera, LIDAR, or IR sensor to the drone.
2. **Data Publication:** Set up the sensors to provide real-time data that can be published and subscribed to based on our code.
3. **Verification:** Ensure the code is able to successfully publish and subscribe to the sensor data.

### Part 2: Computation on the Companion Board

1. **Computation Setup:** Use the companion board to process and compute the sensor data.
2. **Hardware Selection:**
   - If the computation is lightweight, use a Raspberry Pi board.
   - If the computation is complex, use the Jetson Nano board available in Marvel.

## Expected Outcomes

- **ROS Proficiency:** Learn how to use ROS to subscribe and publish data.
- **Telemetry Utilization:** Use telemetry to gather data and compute it on the companion board.
- **Companion Board Computation:** Perform computations based on the real-time data.
- **Machine Learning Basics:** Understand the basics of Machine Learning and Convolutional Neural Networks (CNNs).
- **IoT Basics:** Gain knowledge of Internet of Things (IoT) concepts.

### Resources

- [GitHub - Intelligent-Quads/iq_tutorials](https://github.com/Intelligent-Quads/iq_tutorials) - This repository contains tutorials from the basics and seems good for learning.
- [ROS Software](https://www.ros.org/)

### Software Requirements

- **ROS (Robot Operating System):** A framework for robot software development.
- **Operating System:** Ubuntu is recommended with Gazebo software.

---

## Rule of the Sky : Implementing Drone Regulations Using ROS

## Objective

Create a Gazebo simulation that simulates a head-on collision between two drones, where they detect each other and avoid collision according to regulations. The goal is to employ ROS programming to ensure drone operations conform to regulatory guidelines.

### Importance

- **Pedagogical Tool:** This approach serves as a pedagogical tool for learning ROS while reinforcing adherence to pertinent drone regulations.
- **Computational Resource Utilization:** It is significant for tasks requiring substantial computational resources and real-time data processing.
- **Regulatory Compliance:** It facilitates a comprehensive understanding and compliance with drone regulations.

### Scenario Example

In scenarios involving simultaneous trajectories of multiple drones, the ROS-coded system mandates specific actions under regulatory mandates. For instance, when two drones approach head-on:

- **Drone 1:** Ascend and veer right.
- **Drone 2:** Descend and veer left.

Such implementations impart regulatory knowledge and enhance technical proficiency in ROS programming.

### Additional Tasks

- **Path Following:** The drone can be programmed to follow a path based on visual markers like roads and traffic flow.

## Expected Outcomes

- **ROS Proficiency:** Gain proficiency in ROS programming.
- **Real-time Data Processing:** Learn to process real-time data.
- **Regulatory Understanding:** Understand drone regulations.

---

## ROS (Robot Operating System)

ROS is a framework for robot software development. It provides tools and libraries that help create robot applications from reusable software components. Here’s an overview of ROS 1 and ROS 2, the two main versions:

### ROS 1

- **Established and Widely Used:** ROS 1 has been around for longer and has a vast ecosystem of libraries, tools, and tutorials.
- **Master-Slave Architecture:** Uses a central ROS Master to manage communication between nodes (programs) in the system. This can limit scalability.
- **XML-RPC Middleware:** Communication between nodes relies on XML-RPC, which might not be ideal for real-time systems due to potential latency issues.
- **Limited Platform Support:** Primarily supported on Linux-based operating systems.

### ROS 2

- **Designed for Scalability and Performance:** Addresses ROS 1 limitations by utilizing a distributed communication architecture using Data Distribution Service (DDS). This enables better scalability, reliability, and real-time performance.
- **No Central Master:** Nodes discover and communicate directly with each other, eliminating a single point of failure.
- **Richer APIs:** Offers improved APIs with better language support (C++, Python).
- **Multi-Platform Support:** Runs on Linux, macOS, and Windows, providing more flexibility for development environments.

## ROS Environment Requirements

The specific requirements for setting up a ROS environment depend on the version you choose (ROS 1 or ROS 2) and your operating system. Here's a general guideline:

- **Operating System:**
  - **ROS 1:** Primarily Linux (Ubuntu is a popular choice).
  - **ROS 2:** Linux, macOS, or Windows.
- **Dependencies:**
  - Both ROS 1 and ROS 2 require dependencies like build tools (e.g., CMake, Python development tools), version control systems (e.g., Git), and libraries (e.g., Python libraries like NumPy).
- **ROS Installation:**
  - Follow the official installation instructions for your chosen ROS version and operating system from the [Robot Operating System website](http://wiki.ros.org/ROS/Installation).

---

## ROS-taurant Renovation: Learning How to Use ROS 2 with ROS 1

## Objective

Learn to integrate ROS 2 with ROS 1 and make the best use of both versions.

### ROS 2 Fundamentals

#### To Do:

1. **Install ROS 2:** Install the Humble Distribution on your development machine.
2. **Workspace Setup:** Follow guidelines to set up a simple ROS 2 workspace and write a basic ROS 2 publisher and subscriber node in Python.
3. **Explore ROS 2 Tools:** Familiarize yourself with tools like `ros2 launch` and `ros2 node`.
4. **Create a ROS 2 Workspace:** Implement a functional publisher-subscriber example.

#### Resources:

- [ROS 2 Playlist](https://www.youtube.com/playlist?list=PLLSegLrePWgJudpPUof4-nVFHGkB62Izy)
- [ROS 2 Documentation](https://docs.ros.org/en/humble/index.html)

### ROS 1 Refresher

#### To Do:

1. **Review Existing Project:** Review your existing ROS 1 project.
2. **Identify Components:** Identify ROS 1 nodes, topics, messages, and launch files used in the project.
3. **Documentation:** Briefly document the functionality of each ROS 1 component.

### Bridging the Gap

Learn to use the `ros1_bridge` package and establish communication between your ROS 1 project and the simple ROS 2 node created in the previous task.

#### Resources:

- [YouTube Video on ros1_bridge](https://www.youtube.com/watch?v=sJLvv1xtjSM)
- [ros1_bridge Guide](https://docs.ros.org/en/humble/How-To-Guides/Using-ros1_bridge-Jammy-upstream.html)
- [GitHub - ros2/ros1_bridge](https://github.com/ros2/ros1_bridge#example-1-run-the-bridge-and-the-example-talker-and-listener)

---

## ROS-a-saurus Rex: Taming the Legacy Beast (ROS 1) with a New Language (ROS 2)

## Task

Migrate an existing ROS 1 node into a ROS 2 node (not completely migrating from ROS 1 to ROS 2).

### Steps:

1. **Node Selection:** Select a simple ROS 1 node from your project (e.g., sensor driver, processing node).
2. **Port Functionality:** Port the functionality of the chosen node to ROS 2 using appropriate ROS 2 libraries and message types.
3. **Integration:** Integrate the migrated ROS 2 node with the ROS 1 project using the bridge (if necessary).

#### Resources:

- [Practical Guide for Migrating from ROS1 to ROS2](https://admantium.medium.com/robot-operating-system-practical-guide-for-migrating-from-ros1-to-ros2-2fe93aca9363)



