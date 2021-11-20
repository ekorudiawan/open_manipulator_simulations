# OpenManipulator (ROS Gazebo Simulation Only)
**This forked version only tested on Ubuntu 20.04 and ROS Noetic Ninjemys**
<img src="https://github.com/ROBOTIS-GIT/emanual/blob/master/assets/images/platform/openmanipulator_x/OpenManipulator.png">
<img src="https://github.com/ROBOTIS-GIT/emanual/blob/master/assets/images/platform/openmanipulator_x/OpenManipulator_Chain_Capture.png" width="500">

# Install Additional ROS Package

```bash
sudo apt install ros-noetic-control
sudo apt install ros-noetic-ros-control
sudo apt install ros-noetic-ros-controllers
```

# Run The Simulation Model
**Compile Simulation Model**
```bash
cd ~ 
mkdir -p omx_ws/src
cd omx_ws/src
git clone https://github.com/ekorudiawan/open_manipulator_simulations.git
cd ..
catkin_make
source devel/setup.bash
```
**Run Gazebo Simulation**
```bash
roslaunch open_manipulator_gazebo open_manipulator_gazebo.launch
```
**Run RVIZ**
```bash
roslaunch open_manipulator_description open_manipulator_rviz.launch
```
