# ucf_igvc
UCF IGVC specific workspace.

Temp for testing git stuff

## Table of Contents
* [Packages](#packages)
* [Getting Started](#getting-started)

## <a name="packages"></a>Packages
Below is a brief description of and links to the various ROS packages in this workspace.
* [igvc_description](https://github.com/ucfroboticsclub/ucf_robotics/tree/master/ucf_igvc/src/igvc/igvc_description) -- Complete robot description using URDF.
* [igvc_navigation](https://github.com/ucfroboticsclub/ucf_robotics/tree/master/ucf_igvc/src/igvc_apps/igvc_navigation) -- Configuration of ROS Navigation Stack and any other custom navigation nodes.
* [igvc_gazebo](https://github.com/ucfroboticsclub/ucf_robotics/tree/master/ucf_igvc/src/igvc_simulator/igvc_gazebo) -- Configuration of IGVC Gazebo functionality.
* [igvc_rviz](https://github.com/ucfroboticsclub/ucf_robotics/tree/master/ucf_igvc/src/igvc_viz/igvc_rviz) -- Rviz launchers and configurations.

## <a name="getting-started"></a>Getting Started
If you're completely new, follow these steps to get up and running with our current builds.

1. Set up your development environment.  You need to be running Ubuntu 14.04 and have ROS installed.  Ubuntu installs end up being fairly unique, so we leave that to [google](http://google.com).  To get ROS set up propertly, see Chapter 2 of [this book available freely online](http://www.cse.sc.edu/~jokane/agitr/).  We have no official IDE supported by club members currently, but QtCreator and Eclipse both seem to work ok if you search around for configurations.  Your text editor of choice is the easiest option.

2. Become familiar with basic ROS functionality including how to build existing packages and create new ones.  The book linked above is an excellent resource for getting started and a fairly short read.

3. Fork (recommended if you're looking to get involved in development) and clone this repository.

4. Build ucf_core first.
  1. In a terminal navigate to ../ucf_core/ , enter the following:
    
    `rosdep install -i -y --from-paths src`
    
  2. Now `catkin_make` and `source devel/setup.bash` like usual.
  
5. In the same terminal window where you have sourced the ucf_core setup.bash, navigate to any other workspaces you want to build ( ie. ucf_igvc, ucf_boat, ucf_sub ).

6. Perform the same `rosdep install` as shown in step 4, build, and source to use.
