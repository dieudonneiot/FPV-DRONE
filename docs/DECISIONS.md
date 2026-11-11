# Decisions

## D-01 — Simulation development environment

- **Decision:** Keep the existing Ubuntu 26.04 installation and use ROS 2
  Lyrical with Gazebo Jetty.
- **Installation order:** Ubuntu 26.04 → ROS 2 Lyrical → Gazebo Jetty (with its ROS
  integration).
- **Reason:** The initially requested Jazzy/Harmonic stack targets Ubuntu 24.04.
  The project will keep the installed OS and use the current officially
  supported ROS/Gazebo combination for Ubuntu 26.04 instead.
- **Source:** [F-02](FINDINGS.md#f-02--ros-2-lyrical-ubuntu-platform),
  [F-05](FINDINGS.md#f-05--gazebo-jetty-ubuntu-platform),
  [F-06](FINDINGS.md#f-06--current-ros-and-gazebo-recommendation)
- **Status:** Confirmed

## D-02 — Delay Betaflight setup

- **Decision:** Keep Betaflight as a later tool to try; prioritize the Ubuntu,
  ROS 2 and Gazebo setup first.
- **Reason:** The workshop guidance gives that order. The flight-controller
  hardware and the project's flight requirements have not been selected yet.
- **Source:** [F-04](FINDINGS.md#f-04--betaflight)
- **Status:** Confirmed
