# ROS-bridge implementation with Leo Rover Gazebo

## Docker setup
Create a docker network for the two containers\
`docker network create leo_network --subnet 192.168.10.0/24 --gateway 192.168.10.1`
 
## Run simulation
Open a shell inside `bridge/` folder and run: `docker-compose up`

## Interact with simulation
 * In a fresh shell run: `. ~/ros2_foxy/install/local_setup.bash` to setup the environment
 * Control the rover with: `ros2 topic pub /cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.1, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.0}}"` to send a velocity message.


## Useful commands

`ros2 topic list`
 
