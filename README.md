This package requires installing the ridgeback simulation and navigation pacakges mentioned in the ridgeback tutorials by clearpath robotics (http://www.clearpathrobotics.com/assets/guides/kinetic/ridgeback/simulation.html)

The terminal commands for installing the above mentioned packages: 
```console
sudo apt-get install ros-kinetic-ridgeback-simulator ros-kinetic-ridgeback-desktop
sudo apt-get install ros-kinetic-ridgeback-navigation
```

Clone the repository into the src folder of your workspace and run catkin_make in the toplevel directory of your workspace. You can use the following roslaunch command straight out of the box.
```console
roslaunch multi_ridgeback_simulation multi_ridgeback_world.launch
```
