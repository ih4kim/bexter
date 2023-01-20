# bexter-ros
# Bexter ROS Repo

This repo consists of the controls portion of Bexter, as well as handling the story telling portion of Bexter's pipeline

## Prerequistes

Installing Moveit!
```
sudo apt install ros-noetic-catkin python3-catkin-tools python3-osrf-pycommon
sudo apt install python3-wstool
# Move to workspace src/ directory

cd bexter_ws/src/

wstool init .
wstool merge -t . https://raw.githubusercontent.com/ros-planning/moveit/master/moveit.rosinstall
wstool remove  moveit_tutorials  # this is cloned in the next section
wstool update -t .

rosdep install -y --from-paths . --ignore-src --rosdistro noetic

cd bexter_ws


```