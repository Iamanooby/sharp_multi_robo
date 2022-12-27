# Temporal Memory-based RRT Exploration (Simulation)
This mini project is built open the repository here: https://github.com/hikashi/TM-RRT_exploration_Simulation

## Requirements
The following code is exectuted in ROS Melodic in Ubuntu 18.04 LTS, Python 2.7

The following libraries are required to install before proceeding to run the code

    $ sudo apt-get install ros-melodic-gmapping
    $ sudo apt-get install ros-melodic-navigation
    $ sudo apt-get install python-opencv
    $ sudo apt-get install python-numpy
    $ sudo apt-get install python-scikits-learn
    $ sudo apt-get install ros-melodic-teb-local-planner

## Install turtlebot3_msgs
inside a new workspace folder
    git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs
remember to catkin_make and source the bashrc file
    
## Installation Process
create a new folder called "catkin_explore/src" by executing the following comment:

    $ sudo mkdir -p ~/workspace/catkin_explore/src
    $ cd ~/workspace/catkin_explore/src/
    $ git clone https://github.com/Iamanooby/sharp_multi_robo.git
    $ cd ~/workspace/catkin_explore
    $ catkin_make
    $ echo "source /home/<insert user here>/workspace/catkin_explore/devel/setup.bash" >> ~/.bashrc

Remember to restart terminal before continuing    

## Instruction for Running Simulation
In console one (for running small map):
    
     $ roslaunch ros_3d_multitb3 multiple_tb3_house4.launch
In console one (for running big map):
    
     $ roslaunch ros_3d_multitb3 multiple_tb3_house5.launch

In console two (for tmrrt method):
 
     $ roslaunch tmrrt_exploration trio_exploration.launch
     
 In console two (for opencv method):
 
     $ roslaunch tmrrt_exploration trio_exploration_cv.launch    
     
 
## Setting up Simulation for testing
An example of the simulation can be shown in the following video: 

[![TM-RRT Exploration for Ubuntu 18.04 ROS Melodic](https://img.youtube.com/vi/F40GGvnIfsc/0.jpg)](https://www.youtube.com/watch?v=F40GGvnIfsc "TM-RRT Exploration for Ubuntu 18.04 ROS Melodic")
