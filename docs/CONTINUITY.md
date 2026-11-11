# Continuity

## Last checkpoint

The host is Ubuntu 26.04 with ROS 2 Lyrical, Gazebo Jetty, and the ROS-Gazebo
integration installed. Verification passed: the `ros2` and `gz sim` CLIs work,
ROS-Gazebo packages are discoverable, and Gazebo completed a short headless
empty-world simulation. ROS OpenCV integration, `cv_bridge`, `image_transport`,
`image_geometry`, `camera_info_manager`, and Python OpenCV are installed and
discoverable. The ROS workspace is `/home/kossi/DEVELOPER/tools/ros2_ws/`;
apt-managed software is installed system-wide. Findings and decisions are
recorded in `FINDINGS.md` and `DECISIONS.md`. The project purpose, flight
controller and other hardware are still open.

## Next step

Source `/opt/ros/lyrical/setup.bash` in each new terminal before using ROS.
Next, create a small ROS/Gazebo example in the workspace and continue research
on the project's purpose, competition rules, flight controller, video system
and radio link. Betaflight can be explored later.
