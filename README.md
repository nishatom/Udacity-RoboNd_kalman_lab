# Udacity-RoboNd_kalman_lab

The main.launch file located inside a main package. 
This launch file is a combination of all the 5 nodes we interfaced so far.
Now you have to go into catkin_ws directory and launch the following command:

$ catkin_make

$ source devel/setup.bash

$ roslaunch main main.launch


NOte : All the packages are cloned into src  directory
If  the clone directory does not work for u then  install each package and install there respective dependencies
Also main.launch is provided so that u dont have to launch each node in different cmd.

System:Winodws/Ubuntu 16.04 
Ros   :   Kinetic


TurtleBot Gazebo Package

$ git clone https://github.com/turtlebot/turtlebot

$ rosdep -i install turtlebot_gazebo

$ roslaunch turtlebot_gazebo turtlebot_world.launch

Robot Pose EKF Package

$ git clone https://github.com/udacity/robot_pose_ekf 

$ roslaunch robot_pose_ekf robot_pose_ekf.launch

Visualize the topics:
$ rosrun rqt_graph rqt_graph

Odometry to Trajectory Package

$ git clone https://github.com/udacity/odom_to_trajectory

$ roslaunch odom_to_trajectory create_trajectory.launch 

TurtleBot Teleop Package


Install the Dependencies:

$ rosdep -i install turtlebot_teleop

Rviz Package
$ roslaunch RvizLaunch.launch

Instructions for Installing and Running the rqt_multiplot ROS plugin:
Open a new terminal and install the rqt_multiplot:

$ sudo  apt-get install ros-kinetic-rqt -y

$ sudo  apt-get install ros-kinetic-rqt-multiplot -y

$ sudo apt-get install libqwt-dev -y

$ rm -rf ~/.config/ros.org/rqt_gui.ini

$ rosrun rqt_multiplot rqt_multiplot

Note : if you are unable to install any package try to find the .deb file for the package install via 

$ sudo apt install  {path}/name.deb

http://packages.ros.org/ros/ubuntu/pool/main/r/ros-kinetic-rqt-multiplot/

http://packages.ros.org/ros/ubuntu/pool/main/r/ros-kinetic-variant-msgs/

http://packages.ros.org/ros/ubuntu/pool/main/r/ros-kinetic-variant-topic-tools/

If u have any issue,feel free to ask .

