---
action_type: Maneuver
class: elementalist
distance: Self; see below
feature_type: ability
file_basename: Practical Magic
file_dpath: Abilities/Elementalist/1st-Level Features
flavor: Your mastery of elemental power lets you customize your conjurations.
item_id: practical-magic
item_index: '10'
item_name: Practical Magic
keywords:
- Magic
level: 1
scc:
- mcdm.heroes.v1:feature.ability.elementalist.1st-level-feature:practical-magic
scdc:
- 1.1.1:11.3.9.1:10
source: mcdm.heroes.v1
target: Self
type: feature/ability/elementalist/1st-level-feature
---

```ds-feature
type: feature
feature_type: ability
name: Practical Magic
flavor: Your mastery of elemental power lets you customize your conjurations.
keywords:
  - Magic
usage: Maneuver
distance: Self; see below
target: Self
metadata:
  action_type: Maneuver
  class: elementalist
  distance: Self; see below
  feature_type: ability
  file_basename: Practical Magic
  file_dpath: Abilities/Elementalist/1st-Level Features
  flavor: Your mastery of elemental power lets you customize your conjurations.
  item_id: practical-magic
  item_index: "10"
  item_name: Practical Magic
  keywords:
    - Magic
  level: 1
  scc:
    - mcdm.heroes.v1:feature.ability.elementalist.1st-level-feature:practical-magic
  scdc:
    - 1.1.1:11.3.9.1:10
  source: mcdm.heroes.v1
  target: Self
  type: feature/ability/elementalist/1st-level-feature
effects:
  - name: Effect
    effect: |-
      Choose one of the following effects:
      - You use the [Knockback](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/KnockbackREL_PATH_SUFFIX) maneuver (see Chapter 10: Combat), but its distance becomes the range of your [Hurl Element](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Hurl%20ElementREL_PATH_SUFFIX) ability, and you use Reason instead of Might for the power roll.
      - You choose a creature within the distance of your [Hurl Element](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Hurl%20ElementREL_PATH_SUFFIX) ability and one of the following damage types: acid, cold, corruption, fire, lightning, poison, or sonic. That creature takes damage of the chosen type equal to your Reason score.
      - You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) up to a number of squares equal to your Reason score. If you choose this option, you can spend essence to [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) 1 additional square for each essence spent.
```