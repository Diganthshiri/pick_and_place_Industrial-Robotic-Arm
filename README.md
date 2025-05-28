<<<<<<< HEAD
# pick_and_place_Industrial-Robotic-Arm
=======
# two_scara_collaboration

This project simulates two SCARA robots collaboratively sorting red and blue cylinders from a conveyor belt in Gazebo, with collision avoidance and distributed task handling.

## How to Run

1. **Launch the simulation:**
   ```
   roslaunch two_scara_collaboration initialize.launch
   ```
   - Gazebo starts paused. Unpause to begin.

2. **Start the motion planners:**
   ```
   rosrun two_scara_collaboration scara_left_motion_planner
   rosrun two_scara_collaboration scara_right_motion_planner
   ```

## Features

- Two independent SCARA robots with self-defined PD joint controllers.
- Collision avoidance via workspace boundary negotiation.
- Automatic cylinder spawning and tracking.
- Gripper control via ROS action server.

## File Structure

- `src/`: ROS nodes for control, planning, and simulation.
- `urdf/`: Robot and object models.
- `launch/`: Launch files for simulation setup.
- `config/`: Controller configuration.
- `msg/`, `srv/`, `action/`: Custom ROS message, service, and action definitions.

## Requirements

- ROS (tested with Kinetic/Melodic/Noetic)
- Gazebo simulator

## Video Demo

https://drive.google.com/drive/folders/1tAMU318ZdGLQdAaYkucQySdV8L-aONbm
>>>>>>> 6231c5a (update)
