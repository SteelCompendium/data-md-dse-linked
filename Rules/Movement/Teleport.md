---
file_basename: Teleport
file_dpath: Movement
item_id: teleport
item_index: '05'
item_name: Teleport
scc:
  - mcdm.heroes.v1:movement:teleport
scdc:
  - 1.1.1:10:05
source: mcdm.heroes.v1
type: movement
---

##### Teleport

When a creature teleports, they move from one space to another space instantaneously. The following rules apply to teleporting:

- Teleporting doesn't provoke opportunity attacks or other effects that are triggered by a creature moving.
- When a creature teleports, they bypass any obstacles between the space they leave and their destination space.
- A creature teleporting themself must have line of effect to their destination space. A creature teleporting another creature must have line of effect from the space the [teleported](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) creature leaves and to their destination space.
- A teleporting creature's destination space can't be occupied by another creature or object.
- The effect that lets a creature [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) indicates how far they can [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX). That distance can be greater than the creature's speed.
- If a creature can [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) as part of their usual movement, they can use the Advance move action to [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) a number of squares up to their usual speed, unmodified by conditions or effects.
- If a creature teleports while [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX), they can be standing when they reach their destination space provided they are able to stand. If a [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) creature is [teleported](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) by another creature, it is up to that creature whether the [teleported](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) creature remains [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) or stands if they are able.
- If you [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) while affected by the [grabbed](REL_PATH_PREFIXRules/Conditions/GrabbedREL_PATH_SUFFIX) or [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX) conditions, those conditions end for you.
- When a creature teleports, they must leave the space where they start and enter a new space. A creature can't [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) to and from the same space.
