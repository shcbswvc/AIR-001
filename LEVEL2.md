# Level 2
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

![generative design drone](https://gist.github.com/user-attachments/assets/34751975-3489-4334-acb9-067ce2a7fd13)
---

## ROS 1

### Gain a solid foundation in ROS 1 concepts and practices.

**Tasks:**
* Set up a ROS 1 environment.
* Understand core ROS concepts: nodes, topics, messages, services, parameters.
* Create basic ROS 1 nodes (publishers, subscribers).
* Explore ROS 1 tools and visualization (rqt, rviz).
* Work with ROS 1 packages and workspaces.
* Develop a small ROS 1 project (e.g., simple robot simulation).
* Rule of the Sky: Implementing Drone Regulations Using ROS

  [Resources](https://www.ros.org/)
  ![ROS](https://gist.github.com/user-attachments/assets/b6006280-af07-4af8-8b1e-1862ad0d3715)


### Apply ROS 1 to a real-world robotics challenge.

**Tasks:**
* Create a Gazebo simulation environment.
* Model drones and their dynamics in ROS 1.
* Implement drone collision avoidance logic using ROS 1.
* Simulate drone regulations and enforcement.

  [Resources](https://gazebosim.org/home)

### Integrate sensors and hardware with ROS 1.

**Tasks:**
* Set up sensors (camera, LIDAR, IR) on a companion board.
* Publish sensor data as ROS 1 topics.
* Develop ROS 1 nodes to process sensor data.

 [Resources](https://github.com/Intelligent-Quads/iq_tutorials)

### Task:Integrating LiDAR Sensor for 3D Mapping using ROS

**Objective:** To integrate a LiDAR sensor into a drone payload system using ROS and generate a 3D map of a specified area.   

*Hardware Required:*
* Assembeled drone from level-1
* compatible payload Interface
* ROS-compatible flight controller
* laptop or computer with ROS-installed

**Procedure:**
1. *ROS Setup*
   * Install ROS on your computer and make sure it's compatible with your drone's flight controller.
   * Create a ROS workspace and download necessary packages for LiDAR integration and 3D mapping. (e.i. pcl, gmapping, tf)
2. *LiDAR Sensor Integration*
   * Physically connect the LiDAR sensor to the drone's payload interface.
   * locate the designated payload interface on your drone (could be port or mounting point). Carefully allign the LiDAR sensor with the payload interface ensuring proper orientation and fit. Use screws and clamps to securely attach the LiDAR sensor to the drone. Connect the LiDAR sensor to drone's power supply and data base. use additional cables or adapters if necessary.
   * Configure the LiDAR sensor's parameters (e.i scan rate, min/max angle) using provided software or ROS drivers.
3. *ROS Node Creation*
   * Create a ROS node to receive and process data from the LiDAR sensor.
   * Use an appropriate ROS driver for your LiDAR sensor to publish point cloud data to a topic.
4. *3D Mapping Node*
   * Create a separate ROS node for 3D mapping.
   * subscribe to the point cloud topic from the LiDAR sensor.
   * Use a SLAM algorithm ( Gmapping ) to process the point cloud data and create a 3D map.
   * Publish the generated map to a topicc.
5. *Visualization.*
   * Use ROS visualization tool (e.i.RViz) to visualize the point cloud data and the generated 3D map.
6. *Testing and refinement*
   * Conduct test flights to collect LiDAR data and evaluate the accuracy of the generated 3D map.
   * Refine the mapping parameters and algorithm as needed to improve the map's quality.

**Precaution:**
ensure that the LiDAR sensor is properly caliberated to obtain accurate measurements.5

**Resources:**    
* https://www.youtube.com/watch?v=eJZXRncGaGM
* https://www.youtube.com/watch?v=Qrtz0a7HaQ4
* http://www.ijater.com/Files/5afad700-9e01-4f8c-8bfc-eb8f4892775b_IJATER_51_12.pdf


---

## ROS 2 Fundamentals

### Learn the new features and improvements in ROS 2.

**Tasks:**
* Set up a ROS 2 environment.
* Understand ROS 2 architecture (DDS-based communication).
* Create basic ROS 2 nodes (publishers, subscribers).
* Explore ROS 2 tools and visualization (rclcpp, rclpy).
* Compare and contrast ROS 1 and ROS 2.

**Resources:**
* [ROS 2 Playlist](https://www.youtube.com/playlist?list=PLLSegLrePWgJudpPUof4-nVFHGkB62Izy)
* [ROS 2 Documentation](https://docs.ros.org/en/humble/index.html)

---

## ROS-taurant Renovation: Learning How to Use ROS 2 with ROS 1

### Integrate ROS 1 and ROS 2 systems.

**Tasks:**
* Understand the need for interoperability.
* Learn about the ros1_bridge package.
* Create a bridge between ROS 1 and ROS 2 topics.
* Build a hybrid system using both ROS 1 and ROS 2 components.

**Resources:**
* [YouTube Video on ros1_bridge](https://www.youtube.com/watch?v=sJLvv1xtjSM)
* [ros1_bridge Guide](https://docs.ros.org/en/humble/How-To-Guides/Using-ros1_bridge-Jammy-upstream.html)
* [GitHub - ros2/ros1_bridge](https://github.com/ros2/ros1_bridge#example-1-run-the-bridge-and-the-example-talker-and-listener)

---

## Advanced Topics and ROS 2 Deep Dive

### ROS-a-saurus Rex: Taming the Legacy Beast (ROS 1) with a New Language (ROS 2) (continued)

**Migrate an existing ROS 1 node into a ROS 2 node (not completely migrating from ROS 1 to ROS 2).**

**Steps:**
1. **Node Selection**: Select a simple ROS 1 node from your project (e.g., sensor driver, processing node).
2. **Port Functionality**: Port the functionality of the chosen node to ROS 2 using appropriate ROS 2 libraries and message types.
3. **Integration**: Integrate the migrated ROS 2 node with the ROS 1 project using the bridge (if necessary).

**Resources:**
* [Practical Guide for Migrating from ROS1 to ROS2](https://admantium.medium.com/robot-operating-system-practical-guide-for-migrating-from-ros1-to-ros2-2fe93aca9363)
