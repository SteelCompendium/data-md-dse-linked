---
action_type: feature
class: shadow
feature_type: trait
file_basename: Black Ash Teleport
file_dpath: Shadow/1st-Level Features
item_id: black-ash-teleport
item_index: '11'
item_name: Black Ash Teleport
level: 1
scc:
- mcdm.heroes.v1:feature.trait.shadow.1st-level-feature:black-ash-teleport
scdc:
- 1.1.1:11.1.2.1:11
source: mcdm.heroes.v1
type: feature/trait/shadow/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Black Ash Teleport
metadata:
  action_type: feature
  class: shadow
  feature_type: trait
  file_basename: Black Ash Teleport
  file_dpath: Shadow/1st-Level Features
  item_id: black-ash-teleport
  item_index: "11"
  item_name: Black Ash Teleport
  level: 1
  scc:
    - mcdm.heroes.v1:feature.trait.shadow.1st-level-feature:black-ash-teleport
  scdc:
    - 1.1.1:11.1.2.1:11
  source: mcdm.heroes.v1
  type: feature/trait/shadow/1st-level-feature
effects:
  - effect: You have the following ability.
    features:
      - type: feature
        feature_type: ability
        name: Black Ash Teleport
        flavor: In a swirl of black ash, you step from one place to another.
        keywords:
          - Magic
        usage: Maneuver
        distance: Self
        target: Self
        effects:
          - name: Effect
            effect: You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) up
              to 5 squares. If you have concealment or cover at your
              destination, you can use the
              [Hide](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/HideREL_PATH_SUFFIX)
              maneuver even if you are observed. If you successfully
              [hide](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/HideREL_PATH_SUFFIX)
              using this maneuver, you gain 1 surge.
          - cost: Spend 1+ Insight
            effect: You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) 1
              additional square for each insight spent.
```