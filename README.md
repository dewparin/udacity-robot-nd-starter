# udacity-robot-nd-starter
Starter Project for Udacity Robotics Software Engineer Nanodegree

![Screen Shot 2022-08-12 at 17 57 00](https://user-images.githubusercontent.com/28327235/184341847-d225d292-e3d0-4be3-89d9-70859c3fe6b3.png)


## Created and tested on

[Udacity Robotics Software Engineer Nanodegree Lubuntu VM](https://www.udacity.com/course/robotics-software-engineer--nd209)

ROS: `Kinetic 1.12.7`

Gazebo: `7.8.1`

## How to launch
```
$ catkin_make
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```

## Drive the bot
```
$ source devel/setup.bash
$ rostopic pub /cmd_vel geometry_msgs/Twist  "linear:
  x: 0.1
  y: 0.0
  z: 0.0
angular:
  x: 0.0
  y: 0.0
  z: 0.1"
```

## Available Topics

Wheel joints: `cmd_vel`

Camera: `rgb/image_raw`

Lidar: `scan`
