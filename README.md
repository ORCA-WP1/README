# ORCA Work Package 1 Repository
This github organisation holds core packages for our work

# Installation of the full demo environment

## downloads

clone the following packages into your ROS workspace src/ folder:

simulation environment [AUTH NEEDED]: `git clone https://github.com/YanielCarreno/orcawp1_integration`

modified simulator: `git clone https://github.com/ORCA-WP1/uuv_simulator`

current controller: `git clone https://github.com/ORCA-WP1/current_controller`

mounting for iiwa14 on rexrov2: `git clone https://github.com/ORCA-WP1/rexrov2_iiwa14`

Rexrov2 robot: `git clone https://github.com/ORCA-WP1/rexrov2`

iiwa manipulator: `git clone https://github.com/ORCA-WP1/iiwa_stack`


## dependencies

install any missing dependencies with: `rosdep install --from-paths src --ignore-src -r -y`

## build
navigate to your workspace folder one level up then: `catkin_make` to build all the packages