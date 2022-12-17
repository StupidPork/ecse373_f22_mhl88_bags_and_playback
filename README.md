# ecse373_f22_mhl88_bags_and_playback

# Laboratory 3

ROS package containing a robot model to view the map of Glennan's 5th floor

## 1. Dependencies
1. ROS Neotic
2. ROS joint-state-publisher-gui
3. gazebo-plugins
4. ROS velodyne-description
5. ROS map

## 2. Viewing the model

Use the following command:

`roslaunch bags_and_playback bags_and_playback.launch`

## 3. Viewing the model in Lab 2:

1. Using joint_state_publisher GUI:

`roslaunch navvis_description navvis_description.launch`

2. Not using joint_state_publisher GUI:

`roslaunch navvis_description navvis_description.launch use_gui:=false` 

`use_xacro` can be modified to determine if the model is viewed using the URDF or XACRO file.

3. Viewing the model using XACRO file with joint_state_publisher GUI:

`roslaunch navvis_description navvis_description.launch use_xacro:=true`

`use_robot_state_publisher` can be modified to determine whether to start robot_state publisher.

4. Viewing the model using robot_state_publisher:

`roslaunch navvis_description navvis_description.launch use_robot_state_publisher:=true`
