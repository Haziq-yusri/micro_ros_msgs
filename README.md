# Micro-ROS platform ROS2 messages

Abbreviated telemetry messages for robotic training using ESP32 microcontroller.


## TODO
- enable discarding broken scans, when micro-ROS packets get dropped
  - add bool scan_start_hint; needs support from LDS libraries

## Change Log

### v0.2.0
- added WifiState message for ROS2
- added Telemetry2 message
  - added JointPosVel message
  - adds wifi_rssi_dbm, battery_mv, distance_mm[], bumper[], cliff[], touch[]
  - limits array lengths
  - change joint_pos[], joint_vel[] to JointPosVel[]
- added WifiState message

### v0.1.0
- initial release
  - odometry position, yaw, velocity
  - joint positions, velocity
  - raw LiDAR/LDS laser distance scan data stream
