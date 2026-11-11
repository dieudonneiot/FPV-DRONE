# Findings

## F-01 — ROS 2 Jazzy and Gazebo Harmonic compatibility

- **Finding:** ROS 2 Jazzy on Ubuntu 24.04 (Noble) and Gazebo Harmonic are a
  recommended compatible combination. Gazebo's ROS installation guide points
  users to the ROS `ros_gz` packages for the matching integration.
- **Source:** [Gazebo Harmonic ROS installation guide](https://gazebosim.org/docs/harmonic/ros_installation/)
- **Status:** Confirmed

## F-02 — ROS 2 Lyrical Ubuntu platform

- **Finding:** ROS 2 Lyrical binary packages are available for Ubuntu 26.04
  (Resolute), which is the installed operating system.
- **Source:** [ROS 2 Lyrical Ubuntu installation guide](https://docs.ros.org/en/lyrical/Get-Started/Installation/Ubuntu-Install-Debs.html)
- **Status:** Confirmed

## F-05 — Gazebo Jetty Ubuntu platform

- **Finding:** Gazebo Jetty binaries are provided for Ubuntu 26.04 (Resolute)
  and 24.04 (Noble).
- **Source:** [Gazebo Jetty Ubuntu installation guide](https://gazebosim.org/docs/jetty/install_ubuntu/)
- **Status:** Confirmed

## F-06 — Current ROS and Gazebo recommendation

- **Finding:** The Gazebo ROS integration guide recommends Ubuntu Resolute
  26.04, ROS 2 Lyrical and Gazebo Jetty for new installations. ROS 2 Jazzy and
  Gazebo Harmonic remain a compatible pairing for Ubuntu Noble 24.04.
- **Source:** [Gazebo ROS installation guide](https://gazebosim.org/docs/harmonic/ros_installation/)
- **Status:** Confirmed

## F-07 — ROS computer-vision packages

- **Finding:** ROS 2 vision packages `vision_opencv` (including `cv_bridge`),
  `image_transport` and `image_geometry` are installed and discoverable. The
  Ubuntu `python3-opencv` package and ROS `camera_info_manager` package are
  installed.
- **Source:** Local package and ROS package checks
- **Status:** Confirmed

## F-03 — Installation preparation

- **Finding:** Back up the computer before installing Ubuntu; more than 240 GB
  of storage is preferred if possible. The team guidance recommends trying
  the setup independently and asking for help when blocked.
- **Source:** Project workshop setup guidance shared by the user
- **Status:** Confirmed

## F-04 — Betaflight

- **Finding:** Betaflight may be installed on Windows or Ubuntu and is expected
  to be used later; it is not part of the immediate ROS 2/Gazebo installation
  sequence.
- **Source:** Project workshop setup guidance shared by the user
- **Status:** Confirmed
