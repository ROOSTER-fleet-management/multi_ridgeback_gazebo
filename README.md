This package requires installing the ridgeback simulation and navigation pacakges mentioned in the ridgeback tutorials by clearpath robotics (http://www.clearpathrobotics.com/assets/guides/kinetic/ridgeback/simulation.html)

The terminal commands for installing the above mentioned packages: 
```console
sudo apt-get install ros-kinetic-ridgeback-simulator ros-kinetic-ridgeback-desktop
sudo apt-get install ros-kinetic-ridgeback-navigation
```
Also for teleoperation of the robots from terminal, install the teleop_twist_keyboard package using the following command:
```console
sudo apt-get install ros-kinetic-teleop-twist-keyboard
```

Clone the repository into the src folder of your workspace and run catkin_make in the toplevel directory of your workspace. You can then use the following roslaunch command straight out of the box, to start a gazebo simulation with 2 ridgebacks and two terminals to teleoperate the ridgebacks.
```console
roslaunch multi_ridgeback_gazebo multi_ridgeback_world.launch
```
You can also launch rviz to visualize the ridgebacks, their TFs and their laser scans using the following launch command:
```console
roslaunch multi_ridgeback_gazebo multi_ridgeback_rviz.launch
```