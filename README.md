# r12_moveit_config
ROS package providing moveit support for the ST Robotics r12 arm, including controller configuration .

## Setup
Ensure r12_moveit_config, my_r12_description and r12_hardware_interface packages are all in the catkin workspace src folder. The r12 arm must be running a version of ROBOFORTH supporting the $JL and $RUN commands- you can test this by sending the commands ' $JL and ' $RUN, which will return OK if the respective command are present. If this is not the case please contact ST-ROBOTICS.

## Use
Run the ros nodes joint_trajectory_action_server.py and joint_state_remapper.py from the r12_hardware_interface package. Launch move_group.launch . For visualisation, moveit_rviz.launch may also be launched .
