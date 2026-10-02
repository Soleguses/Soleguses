# Planetary Frontiers – Development Log

Planetary Frontiers has been in active development since **May 31, 2026**.

The project originally began under the working title **Planetary Expansion** and
predates its public GitHub documentation. The early development history presented
here has therefore been reconstructed from archived local builds, development
laboratories and project records.

Internal development has produced dozens of iterative builds. This public log
focuses on the most important milestone versions and major changes in the direction,
technology and gameplay of the project.

> **Versioning note:** lettered internal builds represent rapid iterative snapshots
> rather than public releases. Intermediate micro-revisions are intentionally omitted
> unless they mark an important development step.

## Milestone builds

1. **v0.1 – Project origin**  
   First self-contained HTML/Canvas prototype and the beginning of the core
   exploration, platforming and combat loop.

2. **v0.3.1 – First two-stage demo structure**  
   Established Stage 1-1 and Stage 1-2, the prologue, energy shield, shooting drones,
   two bosses, HUD, pause mode and procedural sound effects.

3. **v0.4.8 – Character and gameplay refinement**  
   Integrated the redesigned Nich Ozimov character, improved presentation and
   movement, and expanded environmental and mission logic.

4. **v0.5.5 – Directed combat and environmental interaction**  
   Added directional aiming, aim-lock, expanded character poses and more systemic
   puzzle interactions with the level environment.

5. **v0.6.5 – Narrative presentation layer**  
   Expanded the prologue into a sequence involving the shuttle cockpit, navigation
   briefing, orbital transition and the approach to NEX-17.

6. **v0.7.5f – Game framework expansion**  
   Added the main menu, tutorial, difficulty modes, settings, save system and a
   procedural music playlist.

7. **v0.8.0d – Planetary Frontiers identity and machine redesign**  
   Consolidated the rename from Planetary Expansion and integrated the redesigned
   autonomous machines of NEX-17.

8. **v0.8.1f – Major Level 1 expansion**  
   Significantly extended Stage 1-1 and Stage 1-2 while preserving the intended
   routes, boss arenas and environmental logic.

9. **v0.8.3d – NEX-17 visual redesign**  
   Introduced a more detailed multilayer parallax environment and a dedicated
   nighttime visual treatment for Stage 1-2.

10. **v0.8.6j_new – Mnemosyne laser and systemic gameplay**  
    Added a second weapon/tool mode for Mnemosyne, allowing a continuous energy laser
    to interact with enemies and selected environmental objects.

11. **v0.8.7z – Advanced Stage 1-2 systems**  
    Consolidated terminal puzzles, transforming structures, destructible objects and
    more complex Heavy Guardian boss behavior.

12. **v0.8.8f – Current development build**  
    Consolidates the latest Level 1 systems, including Drone Dock mechanics,
    NEX/FORTH-17 terminal development and additional protection for critical mission
    objects in Stage 1-1.

---

## Project origin – v0.1 to v0.3.1

Development began on May 31, 2026 with a compact browser prototype built as a
self-contained HTML/CSS/JavaScript/Canvas file.

The first iterations established the fundamental structure that still defines the
project: side-scrolling exploration, platform movement, procedural characters and
environments, technological artifacts, hazardous areas, autonomous enemies and
portal-based progression.

The early prototype rapidly developed into a two-stage Level 1 demo. Stage 1-1
introduced the ruined city during daylight and sunset, while Stage 1-2 created a
nighttime continuation with more dangerous enemies.

By v0.3.1 the prototype already contained a prologue, an energy shield, shooting
drone variants, two boss encounters, a HUD, pause mode and procedural sound effects
generated through the Web Audio API.

This period established the basic identity of the project before more complex
systems were introduced.

## Character, controls and environmental interaction – v0.4.x to v0.5.x

A major early priority was replacing the original simplified player representation
with a more readable procedural human character wearing a futuristic protective
technical suit designed to provide spacesuit-like environmental protection when
required.

A separate Character Lab was used to develop **Nich Ozimov**, his protective suit
and the **Mnemosyne** ER scanner – a multi-purpose research device that also serves
as an energy weapon and technical interaction tool. From the earliest game builds,
Mnemosyne already provided its basic pulse-fire capability, while later development
expanded both its combat and environmental functions.

Character work gradually expanded from idle and walking poses into aiming,
crouching, crouch movement and multiple directional weapon poses.

These experiments were integrated into the main game during the v0.4.x line.

Gameplay also became less dependent on simple traversal. Breakable platforms,
physical obstacles, scripted reactions and mission-specific environmental states
began to appear inside Stage 1-1.

The v0.5.x branch expanded the control system with upward and diagonal aiming,
aim-lock and dedicated interaction controls. Mnemosyne increasingly became both a
weapon and an exploration tool rather than a simple projectile emitter.

Environmental puzzles also became more systemic. Important artifacts could depend
on supports, destructible structures or specific mission sequences, and incorrect
player actions could produce explicit mission-failure states.

## Narrative and cinematic presentation – v0.6.x

The v0.6.x development cycle substantially expanded the opening presentation.

Instead of moving directly from the textual prologue into gameplay, the game gained
a sequence of intermediate scenes covering the damaged shuttle, navigation data,
the discovery of the KDR-17 system, the approach to NEX-17 and the technological
objectives required for survival.

The sequence evolved into a structured flow:

**Prologue → Cockpit briefing → Shuttle transition → Orbital arrival → Surface mission**

Procedural cockpit displays, status panels, navigation information and other
interface elements were refined across several iterations.

By v0.6.5 the opening sequence had become an important part of the game's world
building rather than a simple introduction screen.

## From prototype to game framework – v0.7.x

The v0.7.x line expanded Planetary Expansion beyond the structure of a standalone
level prototype.

A full main menu was introduced together with:

- start and continue flows;
- a playable tutorial;
- three difficulty levels;
- persistent game settings;
- separate music and sound-effect controls;
- autosaves;
- two manual save slots;
- level and stage progression data.

A larger procedural music system was also developed using the Web Audio API.

Rather than relying on prerecorded music files, the soundtrack is generated in
real time from synthesized and layered musical parts. Its direction combines
space ambient, retro-futuristic electronic textures, melodic sequences and
atmospheric transitions, while different compositions are assigned to specific
game contexts.

Separate tracks were created for the main menu, prologue and Level 1, together
with an in-game playlist interface. By v0.7.5f the audio system had been refined
to support clean track starts, contextual playback and correct UI sound behavior.

This was an important architectural step: the project was no longer only a playable
Level 1 experiment, but the foundation of a larger game.

## Planetary Frontiers and the internal development toolchain – v0.8.0 to v0.8.2

With the beginning of the v0.8 line, the project was renamed from
**Planetary Expansion** to **Planetary Frontiers**.

The new title was more distinctive and better reflected the expanding direction
of the game: exploration was intended to move beyond a relatively linear planetary
sequence toward a broader network of worlds, locations and portals.

At the same time, development increasingly moved into dedicated experimental
laboratories.

The Enemy Visual Lab redesigned the autonomous machines of NEX-17:

- **Guardian** – flying patrol drone;
- **Collector** – ground-based maintenance machine;
- **Heavy Collector** – large spider-like combat machine;
- **Heavy Guardian** – heavy flying combat drone.

Their sensor colors, patrol modes, combat states, silhouettes and animation logic
were developed separately before being integrated into the main build.

The v0.8.1 line then significantly expanded the physical size of Stage 1-1 and
Stage 1-2. Several early expansion attempts were discarded after testing revealed
route and arena problems. The stable v0.8.1f layout instead preserved the established
boss areas while extending exploration and adding new hazards, machines and
industrial sections.

Development tools also became more specialized.

The **Debug Overlay Matrix** exposed coordinates and object information directly
inside the running game, while the separate **Level Layout Lab** provided a compressed
map of Stage 1-1 and Stage 1-2 with selectable layers, labels and object inspection.

These tools marked the beginning of a more structured internal level-design workflow.

## NEX-17 visual and systemic refinement – v0.8.3 to v0.8.6

The next group of versions focused on both visual depth and environmental systems.

The original procedural city backgrounds were progressively replaced with more
detailed multilayer parallax environments. The redesigned Abandoned City uses
several independently moving architectural and atmospheric layers to create a
stronger sense of depth, while the buildings themselves were given more volumetric
forms and structural detail.

Stage 1-2 received a dedicated night treatment with a star field, two moons of
NEX-17, cold atmospheric haze and darkened city layers rather than artificially
illuminated abandoned buildings.

The v0.8.4 and v0.8.5 branches concentrated heavily on level geometry and interaction
precision. Platforms, artifacts, industrial objects and traversal routes were
adjusted repeatedly using the newly created debugging tools.

Stage 1-2 also gained more complex technological infrastructure, including electrical
systems and interactive nodes that temporarily change the state of hazardous areas.

The most important mechanical change of the period arrived in v0.8.6.

Mnemosyne received a second functional mode: a continuous **energy laser** selected
independently from the normal pulse weapon. The laser consumes energy while active
and can be used both in combat and for selected environmental interactions.

This transformed Mnemosyne more clearly into a hybrid research instrument, weapon
and technical tool.

## Advanced Stage 1-2 gameplay – v0.8.7

The v0.8.7 line concentrated on interconnected gameplay systems rather than isolated
objects.

Stage 1-2 gained terminal-driven puzzles, scripted transformations of structures,
destructible environmental elements and more tightly controlled progression through
the industrial part of the ruined city.

The Heavy Guardian boss was also expanded beyond a simple flying target.

Its behavior was refined to track the player both horizontally and vertically,
maintain a usable combat distance and interact with destructible parts of the arena.

By v0.8.7z these systems had been stabilized into a more coherent boss and puzzle
sequence.

## Drone Dock, NEX/FORTH-17 and v0.8.8

The v0.8.8 development cycle expanded the technological identity of NEX-17.

A **Drone Dock** sequence introduced multiple functional drones with different
sensor colors and movement patterns. Their activation became part of the progression
logic of Stage 1-2 rather than a purely decorative event.

Another major experiment was the **NEX/FORTH-17 Service OS**.

Originally developed as a separate laboratory, it simulates an alien service
computer through a translated interface inspired by CP/M, Forth, early
microcomputer monitors and CRT-era systems.

The experimental system includes:

- a virtual filesystem;
- command-line navigation;
- readable archive files;
- image reconstruction modes;
- diagnostic commands;
- a small Forth-like stack environment;
- information about the history, technology and biosphere of NEX-17;
- references to the surviving planetary AI;
- service commands connected to the future transition toward Stage 1-3.

The terminal system was designed as both a gameplay mechanic and a form of
environmental storytelling.

The same development period also addressed sequence-breaking possibilities in
Stage 1-1. A critical navigation artifact received an energy-field protection
system, stronger physical knockback and revised mission-failure logic to prevent
premature collection through destruction of its support.

The current working build is **v0.8.8f**.

## Current direction

Level 1 – **Abandoned City Gate** is planned as a four-stage opening world.

Stage 1-1 and Stage 1-2 are the most developed and largely playable parts of the
current build.

**Stage 1-3** is being designed as an industrial complex beneath the ruined city.
A separate background and level-design prototype already explores a large
multi-layer industrial environment with machinery, pipelines, conveyors, reservoirs
and surviving automation. Its planned boss is a large machine assembled from
smaller drones.

**Stage 1-4** is intended to move further into the surviving infrastructure and
history of NEX-17, including a major encounter connected to the planetary AI.

Design prototypes are also being developed for later worlds.

Current experiments include:

- a desert planet with ruins, dunes, sandstorms and a monumental pyramid complex;
- a low-gravity asteroid mining environment with an increased emphasis on
  platforming and meteor hazards;
- a biomechanical horror environment with a distinct visual and gameplay identity.

The long-term structure is intended to evolve from the relatively linear first
world toward wider planetary exploration, including a future star-map system and
greater freedom in the order in which some worlds can be visited.

---

**Development started:** May 31, 2026  
**Original working title:** Planetary Expansion  
**Current title:** Planetary Frontiers  
**Current build:** v0.8.8f  
**Status:** Active development
