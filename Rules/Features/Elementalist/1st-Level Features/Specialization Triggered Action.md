---
action_type: feature
class: elementalist
feature_type: trait
file_basename: Specialization Triggered Action
file_dpath: Features/Elementalist/1st-Level Features
item_id: specialization-triggered-action
item_index: '07'
item_name: Specialization Triggered Action
level: 1
scc:
- mcdm.heroes.v1:feature.trait.elementalist.1st-level-feature:specialization-triggered-action
scdc:
- 1.1.1:11.1.9.1:07
source: mcdm.heroes.v1
type: feature/trait/elementalist/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Specialization Triggered Action
metadata:
  action_type: feature
  class: elementalist
  feature_type: trait
  file_basename: Specialization Triggered Action
  file_dpath: Features/Elementalist/1st-Level Features
  item_id: specialization-triggered-action
  item_index: "07"
  item_name: Specialization Triggered Action
  level: 1
  scc:
    - mcdm.heroes.v1:feature.trait.elementalist.1st-level-feature:specialization-triggered-action
  scdc:
    - 1.1.1:11.1.9.1:07
  source: mcdm.heroes.v1
  type: feature/trait/elementalist/1st-level-feature
effects:
  - effect: |-
      Your [elemental specialization](REL_PATH_PREFIXRules/Features/Elementalist/1st-Level%20Features/Elemental%20SpecializationREL_PATH_SUFFIX) grants you a triggered action, as shown on the [Specialization Triggered Actions](REL_PATH_PREFIXRules/Features/Elementalist/1st-Level%20Features/Specialization%20Triggered%20ActionREL_PATH_SUFFIX) table.

      ###### Elemental Specialization Triggered Actions Table
      | Specialization | Triggered Action                                                                                                                             |
      | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
      | Earth          | [Skin Like Castle Walls](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Skin%20Like%20Castle%20WallsREL_PATH_SUFFIX)       |
      | Fire           | [Explosive Assistance](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Explosive%20AssistanceREL_PATH_SUFFIX)               |
      | Green          | [Breath of Dawn Remembered](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Breath%20of%20Dawn%20RememberedREL_PATH_SUFFIX) |
      | Void           | [Subtle Relocation](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Subtle%20RelocationREL_PATH_SUFFIX)                     |
    features:
      - type: feature
        feature_type: ability
        name: Breath of Dawn Remembered
        flavor: The power you channel grants the ability to get back in the fight.
        keywords:
          - Green
          - Magic
          - Ranged
        usage: Triggered
        distance: Ranged 10
        target: Self or one ally
        trigger: The target starts their turn or takes damage.
        effects:
          - name: Effect
            effect: The target can spend a Recovery.
          - cost: Spend 1+ Essence
            effect: The target can spend an additional Recovery for each essence spent.
      - type: feature
        feature_type: ability
        name: Explosive Assistance
        flavor: You add a little magic to an ally's aggression at just the right time.
        keywords:
          - Fire
          - Magic
          - Ranged
        usage: Triggered
        distance: Ranged 10
        target: Self or one ally
        trigger: The target force moves a creature or object.
        effects:
          - name: Effect
            effect: The forced movement distance gains a bonus equal to your Reason score.
          - cost: Spend 1 Essence
            effect: The forced movement distance gains a bonus equal to twice your Reason
              score instead.
      - type: feature
        feature_type: ability
        name: Skin Like Castle Walls
        flavor: You cover yourself or an ally in protective stone.
        keywords:
          - Earth
          - Magic
          - Ranged
        usage: Triggered
        distance: Ranged 10
        target: Self or one ally
        trigger: The target takes damage.
        effects:
          - name: Effect
            effect: The target takes half the damage.
          - cost: Spend 1 Essence
            effect: If the damage has any potency effects associated with it, the potency is
              reduced by 1 for the target.
      - type: feature
        feature_type: ability
        name: Subtle Relocation
        flavor: You call on the void to swallow and spit out an ally.
        keywords:
          - Magic
          - Ranged
          - Void
        usage: Triggered
        distance: Ranged 10
        target: Self or one ally
        trigger: The target starts their turn, moves, or is force moved.
        effects:
          - name: Effect
            effect: You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              the target up to a number of squares equal to your Reason score.
              If the target moves to trigger this ability, you can
              [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              them at any point during the move.
          - cost: Spend 1 Essence
            effect: You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              the target up to a number of squares equal to twice your Reason
              score instead.
```