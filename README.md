# ArduPilot SITL BoilerPlate
This repository provides a simple code to which connects to ArduPilot SITL via MAVROS, and publishes specified waypoints for the drone to move there. This is meant to provide a quick start, and to be built upon on the requirements for the given problem statement.
<br>

This repository has two packages:

1. For a single drone
2. For a swarm of drones (upto 11)


The instructions for running the above are mentioned in the respective README(s) in their subdirectory.


## References
- Much of the code is a simplified version of<a href="https://github.com/r0ch1n/ardupilot_gazebo_roscam">iq_sim</a> and <a href="https://github.com/Intelligent-Quads/iq_gnc">iq_gnc</a>. Some of the parts are directly taken.
- <a href="https://github.com/r0ch1n/ardupilot_gazebo_roscam">ArduPilot Gazebo Iris Integration (with Camera)</a>. The models have been directly used from this source.