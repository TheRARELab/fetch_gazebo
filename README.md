# Fetch Gazebo

This repository contains the Gazebo simulation for Fetch Robotics Fetch and
Freight Research Edition Robots.

Please note the _branch_: the default branch in GitHub is **gazebo9**.
1. **gazebo9** should be used with **ROS Melodic** and **Ubuntu 18.04**
2. **gazebo7** should be used with **ROS Kinetic** and **Ubuntu 16.04**
3. **gazebo2** should be used with **ROS Indigo** and **Ubuntu 14.04**

## Tutorial & Documentation

Please refer to our documentation page: http://docs.fetchrobotics.com/gazebo.html

## Launch it on ROSDS

The Fetch Gazebo packages can be run in the cloud, through an external service ROSDS, provided by TheConstruct.
http://docs.fetchrobotics.com/gazebo.html#launch-it-on-rosds

## ROS Buildfarm Release
 
Fetch Gazebo Package | Indigo Source | Indigo Debian | Kinetic Source | Kinetic Debian | Melodic Source | Melodic Debian
-------------------- | ------------- | ------------- | -------------- | -------------- | -------------- | --------------
fetch_gazebo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Isrc_uT__fetch_gazebo__ubuntu_trusty__source)](http://build.ros.org/job/Isrc_uT__fetch_gazebo__ubuntu_trusty__source/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ibin_uT64__fetch_gazebo__ubuntu_trusty_amd64__binary)](http://build.ros.org/view/Ibin_uT64/job/Ibin_uT64__fetch_gazebo__ubuntu_trusty_amd64__binary/) | | | | |
fetch_gazebo_demo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Isrc_uT__fetch_gazebo_demo__ubuntu_trusty__source)](http://build.ros.org/job/Isrc_uT__fetch_gazebo_demo__ubuntu_trusty__source/) | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ibin_uT64__fetch_gazebo_demo__ubuntu_trusty_amd64__binary)](http://build.ros.org/job/Ibin_uT64__fetch_gazebo_demo__ubuntu_trusty_amd64__binary/) | | | | |
fetchit_challenge | | | | | | |

## ROS Buildfarm Devel

Fetch Gazebo Package | Indigo Devel | Kinetic Devel | Melodic Devel
-------------------- | ------------ | ------------- | -------------
fetch_gazebo | [![Build Status](http://build.ros.org/buildStatus/icon?job=Idev__fetch_gazebo__ubuntu_trusty_amd64)](http://build.ros.org/view/Idev/job/Idev__fetch_gazebo__ubuntu_trusty_amd64/) | | |
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
