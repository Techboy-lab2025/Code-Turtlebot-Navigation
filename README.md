# Ros Turtlebot Navigation

# Robot Simulation Node

This project demonstrates a simple ROS2 node that simulates the movement of a robot using the `geometry_msgs/Twist` message to send velocity commands. The node periodically publishes velocity commands to the `cmd_vel` topic to simulate forward motion.

## Features

- **ROS2 Node**: The node continuously publishes velocity commands for robot movement.
- **Velocity Command**: Publishes a linear velocity of 0.5 m/s in the forward direction.
- **Logging**: The node logs the published velocity command every time it is published.
  
## Prerequisites

To run this node, you'll need to have ROS2 (e.g., Foxy) installed and set up on your system.

1. Install ROS2 by following the official [installation guide](https://docs.ros.org/en/foxy/Installation.html).
2. Ensure that you have the `geometry_msgs` package installed as it is required to use the `Twist` message type.

## Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Techboy-lab2025/robot_simulation_node.git
    cd robot_simulation_node
    ```

2. **Create a ROS2 workspace** (if not already created):
    ```bash
    mkdir -p ~/ros2_ws/src
    cd ~/ros2_ws/src
    git clone https://github.com/Techboy-lab2025/robot_simulation_node.git
    cd ~/ros2_ws
    colcon build
    ```

3. **Source the ROS2 workspace**:
    ```bash
    source install/setup.bash
    ```

## Running the Node

To run the node, use the following command:
```bash
ros2 run robot_simulation robot_simulation_node
