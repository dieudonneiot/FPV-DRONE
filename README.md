# FPV Drone

Software for an FPV drone project, built the same way as our TEKNOFEST rocket
work: deep research first, then a documented plan, then tested code with CI.

## Status

The host environment is Ubuntu 26.04 with ROS 2 Lyrical and Gazebo Jetty
installed and smoke-tested. The drone's purpose, competition rules and
hardware still need to be established.

See [the findings log](docs/FINDINGS.md) and [decisions](docs/DECISIONS.md).

## How we work

1. **Research.** Collect the requirements (competition rules or mission goals),
   regulations (radio bands and power, flight rules), hardware options and
   open-source prior art. Write every finding into a findings log with an ID
   (F-xx), a source and a status (Confirmed, Provisional or Open).
2. **Plan.** Propose the software stack and list the decisions the team must make
   (D-xx), with the trade-offs.
3. **Build.** Small pull requests, each with tests and green CI. Code cites the
   finding IDs it implements, so every behaviour traces back to its reason.
4. **Continuity.** `docs/CONTINUITY.md` always says what is done and what comes
   next, so anyone can pick the work up on any machine.

## Questions to answer first

- **Development environment:** Ubuntu 26.04, then ROS 2 Lyrical, then Gazebo
  Jetty. ROS workspaces and project tools go under `DEVELOPER/tools/`; system
  packages are installed through Ubuntu's package manager.
- **Purpose:** racing, freestyle, a competition (which one and which category),
  or a mission such as inspection or search?
- **Rules and regulations:** the rules that apply, and the legal radio bands for
  video and control in the country where we fly.
- **Hardware:** frame size, flight controller, video system (analogue or digital)
  and radio link.
- **Firmware:** Betaflight can be installed and tried separately; confirm the
  flight controller and project requirements before choosing firmware for the
  ROS/Gazebo work. Some competitions require original software.
- **Team:** skills and the available time.

## Planned layout

```
docs/       findings log, decisions, CONTINUITY.md
firmware/   flight-controller code or configuration
tools/      ground and test tools
sim/        simulation (for example SITL)
```

## Working rules

- Commits are authored by `dieudonneiot`.
- Read `docs/CONTINUITY.md` before starting work.
