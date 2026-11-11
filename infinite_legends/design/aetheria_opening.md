# Aetheria opening — implementation brief

## Location
**Lumenport Town**, Aetheria.

A coastal settlement built around an old lighthouse. The lighthouse's lower
chamber has recently begun emitting an unusual energy signal. Most residents
believe it is a harmless equipment fault.

## Opening sequence
1. The player arrives in Lumenport Town.
2. A local assistant directs the player to the research building.
3. Professor [name to be decided] explains that unusual Pokémon energy readings
   have appeared near the old lighthouse.
4. The player chooses one starter from the approved starter-selection roster.
5. The player leaves town for the first route.
6. A rival encounter introduces the first battle.
7. The route's closing event hints that Project Eclipse has already investigated
   the lighthouse.

## Starter selection
The final selection interface should let the player choose from the original
starter Pokémon regions, as requested. This is a large roster and needs a
purpose-built selection flow; do not silently limit the final game to only three
Hoenn starters. For the first test build, implement a small temporary test roster
only if the full selection UI is not ready, and label it clearly as temporary.

## Battle and progression
- Use the expansion engine's existing battle system.
- The first rival battle should be tuned after the starter roster and rival team
  are finalized.
- Save/load must be tested after the player receives a starter and after the rival
  battle.

## Technical notes
The current repository contains the upstream Hoenn map set and expansion engine.
Littleroot Town, Professor Birch's Lab, and Route 101 were inspected as examples
of map JSON, scripts, connections, and starter flow. They are references only:
do not edit those upstream maps to pretend they are Lumenport.
Aetheria needs its own map IDs, map layouts, event scripts, region/map metadata,
and original art before it can be compiled as a new playable area.
