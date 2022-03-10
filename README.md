# ros-bridge

* first shell`docker-compose up`
* second shell `. ~/ros2_foxy/install/local_setup.bash` to setup the environment, `export ROS_MASTER_URI=http://172.19.0.3:11311` to setup the ros master, `ros2 topic pub /cmd_vel geometry_msgs/msg/Twist "{linear: {x: 0.1, y: 0.0, z: 0.0}, angular: {x: 0.0, y: 0.0, z: 1.0}}"
` to send a velocity message.


## Useful commands

`ros2 topic list`
 
