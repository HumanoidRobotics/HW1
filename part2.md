# Part 2
## Building a map using slam

This part assumes that you have done [Part 1](./part_1.md) and makes use of some of the packages downloaded and built for [Part 1](./part_1.md).

You are encouraged to go through this [fetch documentation page](http://docs.fetchrobotics.com/navigation.html#building-a-map) for more details.


- Run set-up
Start Gazebo simulator with the playground:
```
roslaunch fetch_gazebo playground.launch
```

Wait until the simulator is fully running and then run the fetch navigation launch file:
```
roslaunch fetch_navigation fetch_nav.launch map_file:=NONE
```

Run the build map launch file:
```
roslaunch fetch_navigation build_map.launch
```

- RVIZ visualization
```
rosrun rviz rviz
```

### Demo to TAs
- Show the simulated robot in action

- What is the least number of navigation goals required to have 90% of the environment built?


## References
- http://docs.fetchrobotics.com/navigation.html#building-a-map
