# Part 1
## Fetch in Gazebo

This part assumes that you have gone through the ROS tutorial and have a basic knowledge of ros concepts like ros workspace, nodes, launch files etc. 

We adapted a portion of the [fetch documentation](http://docs.fetchrobotics.com/gazebo.html) into the following steps. You are encouraged to go through the page for more details.


- Create a ROS workspace
```
mkdir -p ~/fetch_ws/src
cd ~/fetch_ws/src 
catkin_init_workspace 
```

- Clone relevant ROS packages
```
git clone https://github.com/fetchrobotics/fetch_ros.git

git clone https://github.com/fetchrobotics/robot_controllers.git

git clone https://github.com/HumanoidRobotics/fetch_gazebo.git
```

- Build packages
```
cd ..
catkin_make
```

- Run set-up

Start Gazebo simulator with the playground:
```
roslaunch fetch_gazebo playground.launch
```
Wait until the simulator is fully running and then run the demo launch file:
```
roslaunch fetch_gazebo_demo demo.launch
```

- RVIZ visualization
You can visualize several details about the robot in rviz.
```
rosrun rviz rviz
```

### Demo to TAs
- Show the simulated robot in action

- List 5 properties of the robots you can access in rviz


## References
- http://docs.fetchrobotics.com/gazebo.html