# Pax Hanica: Autumn Kriegsspiel

An independent digital wargame set in a fictional world.

The player is the highest commander in a theater of war. Each field unit represents roughly one hundred people. The game is about making consequential decisions with incomplete information: where to commit forces, when to wait, what to trust, and what losses are acceptable.

> Status: early design / work in progress

## Design Direction

- Focus on command decisions rather than individual soldier micromanagement.
- Use the fictional setting to create distinct doctrines, motives, and dilemmas.
- Keep the simulation readable: results should be uncertain, but explainable in hindsight.
- Let orders persist and interact with communication delay, morale, supply, terrain, and local initiative.
- Use a six-hour standard turn as the current design assumption, with two-hour local combat phases when a battle requires finer decisions.
- Use a map-first command interface with dense but structured information, inspired by the clarity of serious operations software rather than by any specific game's visual identity.

## Current State

This repository is currently in pre-production. It contains the project brief, design notes, roadmap, and playtest templates. There is no runnable build yet.

The first playable milestone is a single scenario that can be completed in roughly 20–40 minutes with:

- one compact map;
- two factions;
- five to eight hundred-person units per side;
- one clear objective;
- limited reconnaissance, support, and reserves; and
- a two-day operational window.

## Repository Layout

- `docs/DESIGN.md` — current design brief and assumptions
- `docs/ROADMAP.md` — staged development plan
- `docs/PLAYTEST.md` — playtest notes template
- `LICENSE` — MIT license for code, unless a file states otherwise
- `CONTENT-LICENSE.md` — license boundary for setting and creative content

## Development Principles

1. Build one complete, playable scenario before expanding the setting.
2. Prefer decisions with visible trade-offs over more systems.
3. Keep simulation rules separate from scenario and unit data.
4. Make important outcomes reproducible and reviewable.
5. Treat historical or fictional detail as a tool for better decisions, not as a reason to add complexity by itself.

## Contributing

The project is not ready for code contributions yet. Design feedback, playtest observations, and focused issue reports are welcome. Please read the design brief before proposing new systems.

## Licensing

The code is released under the MIT License. The fictional setting, narrative text, characters, names, scenarios, and project artwork or audio are not automatically covered by that license; see `CONTENT-LICENSE.md` for the current boundary.
