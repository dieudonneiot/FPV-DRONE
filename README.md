# FPV Drone

Software for an FPV drone project, built the same way as our TEKNOFEST rocket
work: deep research first, then a documented plan, then tested code with CI.

## Status

Repository set up. Nothing is decided yet: the goal, rules and hardware come
out of phase 1.

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

- **Purpose:** racing, freestyle, a competition (which one and which category),
  or a mission such as inspection or search?
- **Rules and regulations:** the rules that apply, and the legal radio bands for
  video and control in the country where we fly.
- **Hardware:** frame size, flight controller, video system (analogue or digital)
  and radio link.
- **Firmware:** an existing flight stack (Betaflight, INAV, ArduPilot or PX4)
  configured and extended, or our own code. Some competitions require original
  software.
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
