---
action_type: feature
class: elementalist
feature_type: trait
file_basename: Practical Magic
file_dpath: Elementalist/1st-Level Features
item_id: practical-magic
item_index: 09
item_name: Practical Magic
level: 1
scc:
- mcdm.heroes.v1:feature.trait.elementalist.1st-level-feature:practical-magic
scdc:
- 1.1.1:11.1.9.1:09
source: mcdm.heroes.v1
type: feature/trait/elementalist/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Practical Magic
metadata:
  action_type: feature
  class: elementalist
  feature_type: trait
  file_basename: Practical Magic
  file_dpath: Elementalist/1st-Level Features
  item_id: practical-magic
  item_index: 9
  item_name: Practical Magic
  level: 1
  scc:
    - mcdm.heroes.v1:feature.trait.elementalist.1st-level-feature:practical-magic
  scdc:
    - 1.1.1:11.1.9.1:09
  source: mcdm.heroes.v1
  type: feature/trait/elementalist/1st-level-feature
effects:
  - effect: You have the following ability.
    features:
      - type: feature
        feature_type: ability
        name: Practical Magic
        flavor: Your mastery of elemental power lets you customize your conjurations.
        keywords:
          - Magic
        usage: Maneuver
        distance: Self; see below
        target: Self
        effects:
          - name: Effect
            effect: |-
              Choose one of the following effects:
              - You use the [Knockback](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/KnockbackREL_PATH_SUFFIX) maneuver (see Chapter 10: Combat), but its distance becomes the range of your [Hurl Element](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Hurl%20ElementREL_PATH_SUFFIX) ability, and you use Reason instead of Might for the power roll.
              - You choose a creature within the distance of your [Hurl Element](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Hurl%20ElementREL_PATH_SUFFIX) ability and one of the following damage types: acid, cold, corruption, fire, lightning, poison, or sonic. That creature takes damage of the chosen type equal to your Reason score.
              - You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) up to a number of squares equal to your Reason score. If you choose this option, you can spend essence to [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) 1 additional square for each essence spent.
```