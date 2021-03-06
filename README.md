This package is part of Robot Optimization, Scheduling, Task Execution and Routing (Ro.O.S.T.E.R.)
is a ROS (Robot Operating System) based open source project to develop a heterogeneous fleet management solution
with task allocation, scheduling and autonomous navigation capabilities. Detailed documentation including architectural overview, installation instructions, license information and source code API documentation can be found [here](https://rooster-fleet-management.github.io/rooster_fleet_manager/).
 
This software has been developed as part of the work at
the ['Center of Design for Advanced Manufacturing'](https://www.tudelft.nl/en/ide/research/research-labs/center-of-design-for-advanced-manufacturing/) lab of [TU Delft](https://www.tudelft.nl/en/)
on the ['Collaborating and coupled AGV swarms with extended environment recognition'](https://eitmanufacturing.eu/collaborating-and-coupled-agv-swarms-with-extended-environment-recognition/)  project
funded by [EIT Manufacturing](<https://eitmanufacturing.eu/>).
 


## Installation and Use
This package requires installing the ridgeback simulation and navigation pacakges mentioned in the ridgeback tutorials by clearpath robotics (http://www.clearpathrobotics.com/assets/guides/kinetic/ridgeback/simulation.html)

The terminal commands for installing the above mentioned packages: 
```console
sudo apt-get install ros-melodic-ridgeback-simulator ros-melodic-ridgeback-desktop
sudo apt-get install ros-melodic-ridgeback-navigation
```
Also for teleoperation of the robots from terminal, install the teleop_twist_keyboard package using the following command:
```console
sudo apt-get install ros-melodic-teleop-twist-keyboard
```

Clone the repository into the src folder of your workspace and run catkin_make in the toplevel directory of your workspace. You can then use the following roslaunch command straight out of the box, to start a gazebo simulation with 2 ridgebacks and two terminals to teleoperate the ridgebacks. This launch file also launches rviz to visualize the two robots, their laser scans and the TF tree.
```console
roslaunch multi_ridgeback_gazebo multi_ridgeback_world.launch
```


 

