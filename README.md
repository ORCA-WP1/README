# ORCA Work Package 1 Repository
This github organisation holds core packages for our work

# Installation of the full demo environment

## downloads

clone the following packages into your ROS workspace src/ folder:

simulation environment [AUTH NEEDED]: `git clone https://github.com/YanielCarreno/orcawp1_integration`

modified simulator: `git clone https://github.com/ORCA-WP1/uuv_simulator`

current controller: `git clone https://github.com/ORCA-WP1/current_controller`

tidal disturbances [AUTH NEEDED]: `git clone https://github.com/ORCA-WP1/environment_controller`

mounting for iiwa14 on rexrov2: `git clone https://github.com/ORCA-WP1/rexrov2_iiwa14`

Rexrov2 robot: `git clone https://github.com/ORCA-WP1/rexrov2`

iiwa manipulator: `git clone https://github.com/ORCA-WP1/iiwa_stack`


## dependencies

ensure your apt packages are up to date: `sudo apt-get update` then `sudo apt-get upgrade`

install any missing dependencies with: `rosdep install --from-paths src --ignore-src -r -y`

## build
navigate to your workspace folder one level up then: `catkin_make` to build all the packages

# Usage:

ORCAWP1 Experiment: Simulation Scenario

to run default simulation: 

`roslaunch orcawp1_integration integration_scenario.launch`

to run with rexrov2 and iiwa14 manipulator:

`roslaunch orcawp1_integration integration_scenario_rexrov2_iiwa14.launch`

[WIP] to run with blurov2 and hdt manipulator:

`roslaunch orcawp1_integration integration_scenario_bluerov2_hdt.launch`

## launch arguments
 
disturbances from file: `disturbances:=true`

random disturbances: `random_disturbances:=true`

tidal_currents: `tidal_current:=true`