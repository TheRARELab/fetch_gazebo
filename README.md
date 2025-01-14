# Fetch Gazebo

This repository contains the Gazebo simulation for Fetch Robotics Fetch and
Freight Research Edition Robots.

Please note the _branch_: the default branch in GitHub is **gazebo9**.
1. **gazebo11** should be used with **ROS Noetic** and **Ubuntu 20.04** (untested as of 1-2021)
2. **gazebo9** should be used with **ROS Melodic** and **Ubuntu 18.04**
3. **gazebo7** should be used with **ROS Kinetic** and **Ubuntu 16.04** (not supported on hardware)
4. **gazebo2** should be used with **ROS Indigo** and **Ubuntu 14.04** (EOL)

## Tutorial & Documentation

Please refer to our documentation page: http://docs.fetchrobotics.com/gazebo.html

## Launch it on ROSDS

The Fetch Gazebo packages can be run in the cloud, through an external service ROSDS, provided by TheConstruct.
http://docs.fetchrobotics.com/gazebo.html#launch-it-on-rosds

## ROS Buildfarm Release
 
Fetch Gazebo Package | Kinetic Source | Kinetic Debian | Melodic Source | Melodic Debian
-------------------- | -------------- | -------------- | -------------- | --------------
fetch_gazebo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ksrc_uX__fetch_gazebo__ubuntu_xenial__source)](http://build.ros.org/job/Ksrc_uX__fetch_gazebo__ubuntu_xenial__source/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Kbin_uX64__fetch_gazebo__ubuntu_xenial_amd64__binary)](http://build.ros.org/view/Kbin_uX64/job/Kbin_uX64__fetch_gazebo__ubuntu_xenial_amd64__binary/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Msrc_uB__fetch_gazebo__ubuntu_bionic__source)](http://build.ros.org/view/Mbin_uB64/job/Msrc_uB__fetch_gazebo__ubuntu_bionic__source/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Mbin_uB64__fetch_gazebo__ubuntu_bionic_amd64__binary)](http://build.ros.org/view/Mbin_uB64/job/Mbin_uB64__fetch_gazebo__ubuntu_bionic_amd64__binary/) |
fetch_gazebo_demo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ksrc_uX__fetch_gazebo_demo__ubuntu_xenial__source)](http://build.ros.org/job/Ksrc_uX__fetch_gazebo_demo__ubuntu_xenial__source/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Kbin_uX64__fetch_gazebo_demo__ubuntu_xenial_amd64__binary)](http://build.ros.org/job/Kbin_uX64__fetch_gazebo_demo__ubuntu_xenial_amd64__binary/) | | | | |
fetchit_challenge | | | | | | |

## ROS Buildfarm Devel

Fetch Gazebo Package | Melodic Devel
-------------------- | -------------
fetch_gazebo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Mdev__fetch_gazebo__ubuntu_bionic_amd64)](http://build.ros.org/view/Mdev/job/Mdev__fetch_gazebo__ubuntu_bionic_amd64/)
fetch_gazebo_demo | | | |
fetchit_challenge | | | |

## Changes
1. Removed the dropoff box from all worlds.
2. Removed the gearbox container from all worlds.
3. Added more gears and gearbox parts to ``` fetchit_challenge_arena_montreal2019_highlights.world``` and ```fetchit_challenge_arena_montreal2019.world```
4. Updated the screw bin in all worlds
5. Added screws to ``` fetchit_challenge_arena_montreal2019_highlights.world``` and ```fetchit_challenge_arena_montreal2019.world```
6. Added simple worlds based on ``` fetchit_challenge_arena_montreal2019_highlights.world``` for each task.  
      To run use:

      Caddy table: `roslaunch fetchit_challenge main_arena_montreal2019_simple_caddy.launch`

      Schunk table: `roslaunch fetchit_challenge main_arena_montreal2019_simple_schunk_machine.launch`

      Screw table: `roslaunch fetchit_challenge main_arena_montreal2019_simple_screw.launch`

      Gearbox table:`roslaunch fetchit_challenge main_arena_montreal2019_simple_gearbox.launch`


Before:
![b4](https://user-images.githubusercontent.com/15792263/60300328-c1ac8400-98fc-11e9-857b-f016a7c77213.png)

After:
![after](https://user-images.githubusercontent.com/15792263/62237631-53495e80-b39f-11e9-9197-5f766de23f11.png)

7. Added NEC 0115A arena with long tables and foam board walls
```
roslaunch fetchit_challenge nec0115a_arena.launch
roslaunch fetchit_challenge nec0115a_arena_highlights.launch
```
![image](https://github.com/user-attachments/assets/6daf7f16-39ca-4f53-996d-37b9c5cfe4ce)
