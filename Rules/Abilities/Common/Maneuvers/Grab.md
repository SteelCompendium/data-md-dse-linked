---
class: combat
file_basename: Grab
file_dpath: Abilities/Common/Maneuvers
item_id: grab
item_index: '10'
item_name: Grab
scc:
- mcdm.heroes.v1:common-ability.maneuver:grab
scdc:
- 1.1.1:16.3:10
source: mcdm.heroes.v1
type: common-ability/maneuver
---

```ds-feature
type: feature
feature_type: trait
name: Grab
metadata:
  class: combat
  file_basename: Grab
  file_dpath: Abilities/Common/Maneuvers
  item_id: grab
  item_index: "10"
  item_name: Grab
  scc:
    - mcdm.heroes.v1:common-ability.maneuver:grab
  scdc:
    - 1.1.1:16.3:10
  source: mcdm.heroes.v1
  type: common-ability/maneuver
effects:
  - effect: A creature seeking to keep a foe close and locked down can attempt to
      [grab](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/GrabREL_PATH_SUFFIX)
      a creature using the following ability.
    features:
      - type: feature
        feature_type: ability
        name: Grab
        keywords:
          - Melee
          - Weapon
        usage: Maneuver
        distance: Melee 1
        target: One creature
        effects:
          - roll: Power Roll + Might
            tier1: No effect.
            tier2: You can
              [grab](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/GrabREL_PATH_SUFFIX)
              the target, but if you do, the target can make a melee [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              against you before they are
              [grabbed](REL_PATH_PREFIXRules/Conditions/GrabbedREL_PATH_SUFFIX).
            tier3: The target is
              [grabbed](REL_PATH_PREFIXRules/Conditions/GrabbedREL_PATH_SUFFIX)
              by you.
          - name: Effect
            effect: You can usually target only creatures of your size or smaller. If your
              Might score is 2 or higher, you can target any creature with a
              size equal to or less than your Might score.
  - effect: |-
      Unless otherwise indicated, a creature can [grab](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/GrabREL_PATH_SUFFIX) only one creature at a time.

      See [Conditions](#page-91-2) in [Chapter 5: Classes](#page-83-2) for information on the [grabbed](REL_PATH_PREFIXRules/Conditions/GrabbedREL_PATH_SUFFIX) condition.
```