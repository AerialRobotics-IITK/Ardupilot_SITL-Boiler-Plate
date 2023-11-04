## Instructions for Running Single Drone Simulation

### Requirements 
- <a href="https://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html">ArduPilot SITL</a>
- <a href="https://github.com/mavlink/mavros">MAVROS</a>

### Step 1 : Run ArduPilot SITL
``sim_vehicle.py -v ArduCopter -f gazebo-iris --console``
### Step 2 : Initiate ArduPilot Gazebo
``export GAZEBO_MODEL_PATH=<path-to-ws>/src/single_drone/models:$GAZEBO_MODEL_PATH`` 
<br>
Here, ``<path-to-ws>`` should point to absolute path to the workspace in which you have this package

``roslaunch single_drone iris_with_roscam.launch``

### Step 3 : Initiate MAVROS
``roslaunch single_drone apm.launch ``

### Step 4 : Run the Waypoint Node
``rosrun single_drone single_drone_node``
