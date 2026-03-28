---
action_type: feature
class: fury
feature_type: trait
file_basename: 3rd Level Aspect Feature
file_dpath: Features/Fury/3rd-Level Features
item_id: 3rd-level-aspect-feature
item_index: '01'
item_name: 3rd-Level Aspect Feature
level: 3
scc:
- mcdm.heroes.v1:feature.trait.fury.3rd-level-feature:3rd-level-aspect-feature
scdc:
- 1.1.1:11.1.5.7:01
source: mcdm.heroes.v1
type: feature/trait/fury/3rd-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: 3rd-Level Aspect Feature
metadata:
  action_type: feature
  class: fury
  feature_type: trait
  file_basename: 3rd Level Aspect Feature
  file_dpath: Features/Fury/3rd-Level Features
  item_id: 3rd-level-aspect-feature
  item_index: "01"
  item_name: 3rd-Level Aspect Feature
  level: 3
  scc:
    - mcdm.heroes.v1:feature.trait.fury.3rd-level-feature:3rd-level-aspect-feature
  scdc:
    - 1.1.1:11.1.5.7:01
  source: mcdm.heroes.v1
  type: feature/trait/fury/3rd-level-feature
effects:
  - effect: |-
      Your [primordial aspect](REL_PATH_PREFIXRules/Features/Fury/1st-Level%20Features/Primordial%20AspectREL_PATH_SUFFIX) grants you a feature, as shown on the 3rd-Level Aspect Features table.

      ###### 3rd-Level Aspect Features Table
      | Aspect     | Feature                                                                                                                                                        |
      | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
      | Berserker  | [Immovable Object](REL_PATH_PREFIXRules/Features/Fury/3rd-Level%20Features/3rd-Level%20Aspect%20Feature/Immovable%20ObjectREL_PATH_SUFFIX)                     |
      | Reaver     | [See Through Their Tricks](REL_PATH_PREFIXRules/Features/Fury/3rd-Level%20Features/3rd-Level%20Aspect%20Feature/See%20Through%20Their%20TricksREL_PATH_SUFFIX) |
      | Stormwight | [Nature's Knight](REL_PATH_PREFIXRules/Features/Fury/3rd-Level%20Features/3rd-Level%20Aspect%20Feature/Natures%20KnightREL_PATH_SUFFIX)                        |
      ##### Immovable Object
      You add your level to your effective size for the purpose of interacting with creatures and objects, including determining whether you can lift an object, are affected by forced movement, and so forth. This has no effect on whether you can be [grabbed](REL_PATH_PREFIXRules/Conditions/GrabbedREL_PATH_SUFFIX).
      Additionally, you have a bonus to [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX) equal to your Might score.
      ##### Nature's Knight
      You can speak with animals and elementals. Additionally, you automatically sense the presence of animals and elementals within 10 squares of you, even if they are hidden.
      When you are in a negotiation with an animal or elemental, you treat your Renown as 1 higher than usual. This stacks with the increase to your effective Renown in a negotiation with an animal of your type while in animal form (see Stormwight Kits).
      ##### See Through Their Tricks
      You have a double edge on tests made to search for hidden creatures, discern hidden motives, or detect lies. You also have a double edge on tests made to gamble!
```