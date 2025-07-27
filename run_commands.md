```bash
docker build -t f1tenth_gym_ros -f Dockerfile .
```

```bash
rocker --nvidia --x11 --volume .:/ros2_ws/src/f1tenth_gym_ros -- f1tenth_gym_ros
```

```bash
source /opt/ros/humble/setup.bash
source install/local_setup.bash
ros2 launch f1tenth_gym_ros gym_bridge_launch.py
```

```bash
 docker exec -it interesting_ritchie /bin/bash
 ```

```bash
 ros2 topic pub /goal_pose geometry_msgs/PoseStamped "{header: {stamp: {sec: 0}, frame_id: 'map'}, pose: {position: {x: 18.2, y: 7.0, z: 0.0}, orientation: {w: 0.0}}}"
 ```

  ros2 topic pub /goal_pose geometry_msgs/PoseStamped "{header: {stamp: {sec: 0}, frame_id: 'map'}, pose: {position: {x: 18.2, y: 7.0, z: 0.0}, orientation: {w: 0.0}}}"