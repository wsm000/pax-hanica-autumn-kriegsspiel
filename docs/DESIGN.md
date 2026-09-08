# Design Brief

## Premise

*Pax Hanica: Autumn Kriegsspiel* is an independent digital wargame about command decisions in a fictional war. The player is the highest commander in a theater of war, not a direct controller of individual soldiers.

The game should make the player ask:

- What do I believe about the enemy?
- Which objective matters enough to spend lives and time on?
- Where should I concentrate force?
- When should I commit a reserve?
- What can I afford to leave undefended?

## Scale

- A field unit represents roughly one hundred people.
- The player controls groups of units through orders and priorities.
- Individual soldiers, bullets, and room-by-room movement are abstracted.
- A unit's meaningful state includes strength, morale, fatigue, ammunition, supply, cohesion, position, orders, and confidence in its information.

The exact in-world name for a one-hundred-person unit is still open. The design should use a neutral term such as `unit` until the fictional organization is defined.

## Time Model

The current working assumption is:

- standard operational turn: six hours;
- four standard turns per day: dawn, day, dusk, and night;
- local combat phase: two-hour resolution when a contact requires closer decisions;
- long periods without meaningful decisions should advance to the next relevant event.

The player should not need to rewrite every unit's orders every two hours. Orders should remain active until completed, interrupted, expired, or invalidated by a trigger.

## Core Loop

1. Review reports, known enemy positions, supply, morale, and unfinished orders.
2. Set objectives, priorities, stances, reserves, and support allocation.
3. Advance time and let units execute with friction and local initiative.
4. Receive reports that distinguish observation, inference, and uncertainty.
5. Respond to meaningful changes and reassess the operational plan.
6. Review the outcome and understand which assumptions led to success or failure.

## Interface Direction

The interface should be map-first and information-dense, taking inspiration from serious operations software and command simulators such as CMO without reproducing a specific game's visual design.

The first interface pass should prioritize:

- a central operational map with strong unit, terrain, objective, and information-state readability;
- a compact command panel for selected units and groups;
- a report and event feed that separates confirmed observations from estimates;
- time controls that make pause, planning, execution, and local combat phases obvious;
- a consistent way to batch orders without hiding the consequences of those orders; and
- a post-turn or post-scenario review that reconstructs decisions and outcomes.

The interface should expose complexity progressively. A player can inspect details when needed, but the main map should answer the most important questions at a glance: where are my forces, what do they know, what are they doing, and what needs my attention now?

## Design Pillars

### Decisions over actions

The main interaction should be choosing between competing plans. More clicks should not automatically mean more depth.

### Incomplete but trustworthy information

The player should not see everything. Reports can be late or uncertain, but after a battle the game should provide enough evidence to explain what happened.

### Persistent intent

A commander gives an order with an objective, posture, duration, and stop conditions. The order is not a single tile-by-tile command.

### Friction creates character

Communication delay, fatigue, morale, terrain, supply, weather, and unit initiative should make plans imperfect without making outcomes arbitrary.

### Fiction serves play

The setting should create meaningful asymmetry between factions and make objectives matter. Lore should arrive through the player's decisions, reports, and consequences rather than blocking access to the game.

## First Vertical Slice

A first playable scenario should include:

- one compact map;
- two factions;
- five to eight units per side;
- one contested objective such as a bridge, town, or supply route;
- limited reconnaissance and one or two support assets;
- at least one reserve decision;
- a two-day operational window; and
- a result that can be reviewed after the scenario.

## Deliberate Non-Goals for the First Slice

- individual soldier simulation;
- a complete campaign system;
- multiplayer;
- a general-purpose map editor;
- every faction and weapon in the setting;
- a fully autonomous strategic AI;
- perfect historical or technical simulation.

## Open Questions

- What is the player's exact in-world rank and command structure?
- What is the fictional name and organization of a one-hundred-person unit?
- How much control can subordinate commanders exercise without player intervention?
- Which three resources create the most meaningful trade-offs: time, information, supply, morale, or something else?
- What kind of scenario best introduces the setting and the core decision loop?
