# onenight_ros

This repo contains a set of packages for the simulation of the onenight robot which participate the Eurobot 2020 competition.
It also include a Gazebo simulation environment for the Eurobot 2020 including the table and the tumblers (tags). Feel free to use it to train your robot ! ;)


## Simulation environment setup

The Eurobot simulation contains a set of models which you have to import as a gazebo library.
Thus, you will want to add to your **GAZEBO_MODEL_PATH** environment variable the path to the onenight_gazebo/worlds/models directory.
To do so, I would advise to add in your ~.bashrc the following line: 
```
export GAZEBO_MODEL_PATH=<your_catkin_ws_paths>/src/onenight_ros/onenight_gazebo/worlds/models:$GAZEBO_MODEL_PATH
```
You should now be able to see this model repository in your *insert*  tab of gazebo.

To run only the Eurobot environment, launch from the *onenight_gazebo/world repository* the folowing command :
```
gazebo eurobot_2020.world
```

## Launch Onenight

To launch onenight on the table, please use :
```
roslaunch onenight_bringup simu.launch
```

![Simu photo](https://github.com/Luczia/onenight_ros/blob/master/data/pictures/Simu.png)
