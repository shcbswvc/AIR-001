## Design a Leg for a Quadcopter Frame

### Objective

Design a leg for a quadcopter frame using the dimensions of the standard T50 frame design for quadcopters. Utilize the generative design tools in Fusion 360 to complete this task with a focus on weight reduction while maintaining the structural stiffness of the leg.

#### Steps

1. **Understand Generative Design Environment:**
   - Gain a thorough understanding of how to operate the generative design environment in Fusion 360.
   - Learn about the use of **Obstacle Geometry**, **Preserve Geometry**, and **Starting Shape**.

2. **Design Considerations:**
   - Weight reduction of the legs is a high priority.
   - Ensure that the structural stiffness of the legs is not compromised.

3. **Resource:**
   - Use the following playlist to understand the generative design environment: [Fusion 360 Generative Design Playlist](https://www.youtube.com/watch?v=sps-OR60fVU&list=PLEzzQIuBvBkr7tNcgERS9IIxLSPbb8A6M).

#### Design Process

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

#### Conclusion

By completing this task, you will gain practical experience in using generative design tools to create optimized components for quadcopters. This exercise emphasizes the importance of balancing weight reduction and structural integrity in design engineering.

## ROS 1:
### Gain a solid foundation in ROS 1 concepts and practices.
Tasks:
* Set up a ROS 1 environment.
* Understand core ROS concepts: nodes, topics, messages, services, parameters.
* Create basic ROS 1 nodes (publishers, subscribers).
* Explore ROS 1 tools and visualization (rqt, rviz).
* Work with ROS 1 packages and workspaces.
* Develop a small ROS 1 project (e.g., simple robot simulation).
* Rule of the Sky: Implementing Drone Regulations Using ROS
  [Resources](https://www.ros.org/)

### Apply ROS 1 to a real-world robotics challenge.
Tasks:
* Create a Gazebo simulation environment.
* Model drones and their dynamics in ROS 1.
* Implement drone collision avoidance logic using ROS 1.
* Simulate drone regulations and enforcement.
  [Resources](https://gazebosim.org/home)


### Integrate sensors and hardware with ROS 1.
Tasks:
* Set up sensors (camera, LIDAR, IR) on a companion board.
* Publish sensor data as ROS 1 topics.
* Develop ROS 1 nodes to process sensor data.
 [Resources](https://github.com/Intelligent-Quads/iq_tutorials)

## ROS 2 Fundamentals

### Learn the new features and improvements in ROS 2.
Tasks:
* Set up a ROS 2 environment.
* Understand ROS 2 architecture (DDS-based communication).
* Create basic ROS 2 nodes (publishers, subscribers).
* Explore ROS 2 tools and visualization (rclcpp, rclpy).
* Compare and contrast ROS 1 and ROS 2.
Resources:
* [ROS 2 Playlist](https://www.youtube.com/playlist?list=PLLSegLrePWgJudpPUof4-nVFHGkB62Izy)
* [ROS 2 Documentation](https://docs.ros.org/en/humble/index.html)

## ROS-taurant Renovation: Learning How to Use ROS 2 with ROS 1
#### Integrate ROS 1 and ROS 2 systems.
Tasks:
* Understand the need for interoperability.
* Learn about the ros1_bridge package.
* Create a bridge between ROS 1 and ROS 2 topics.
* Build a hybrid system using both ROS 1 and ROS 2 components.
Resources:
* [YouTube Video on ros1_bridge](https://www.youtube.com/watch?v=sJLvv1xtjSM)
* [ros1_bridge Guide](https://docs.ros.org/en/humble/How-To-Guides/Using-ros1_bridge-Jammy-upstream.html)
* [GitHub - ros2/ros1_bridge](https://github.com/ros2/ros1_bridge#example-1-run-the-bridge-and-the-example-talker-and-listener)

## Advanced Topics and ROS 2 Deep Dive
### ROS-a-saurus Rex: Taming the Legacy Beast (ROS 1) with a New Language (ROS 2) (continued)
Migrate an existing ROS 1 node into a ROS 2 node (not completely migrating from ROS 1 to ROS 2).
Steps:
1. Node Selection: Select a simple ROS 1 node from your project (e.g., sensor driver, processing node).
2. Port Functionality: Port the functionality of the chosen node to ROS 2 using appropriate ROS 2 libraries and message types.
3. Integration: Integrate the migrated ROS 2 node with the ROS 1 project using the bridge (if necessary).

Resources: 
* [Practical Guide for Migrating from ROS1 to ROS2](https://admantium.medium.com/robot-operating-system-practical-guide-for-migrating-from-ros1-to-ros2-2fe93aca9363)
