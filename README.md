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
