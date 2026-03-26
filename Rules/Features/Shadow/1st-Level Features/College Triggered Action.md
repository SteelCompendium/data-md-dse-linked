---
action_type: feature
class: shadow
feature_type: trait
file_basename: College Triggered Action
file_dpath: Features/Shadow/1st-Level Features
item_id: college-triggered-action
item_index: '03'
item_name: College Triggered Action
level: 1
scc:
- mcdm.heroes.v1:feature.trait.shadow.1st-level-feature:college-triggered-action
scdc:
- 1.1.1:11.1.2.1:03
source: mcdm.heroes.v1
type: feature/trait/shadow/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: College Triggered Action
metadata:
  action_type: feature
  class: shadow
  feature_type: trait
  file_basename: College Triggered Action
  file_dpath: Features/Shadow/1st-Level Features
  item_id: college-triggered-action
  item_index: "03"
  item_name: College Triggered Action
  level: 1
  scc:
    - mcdm.heroes.v1:feature.trait.shadow.1st-level-feature:college-triggered-action
  scdc:
    - 1.1.1:11.1.2.1:03
  source: mcdm.heroes.v1
  type: feature/trait/shadow/1st-level-feature
effects:
  - effect: |-
      Your [shadow](REL_PATH_PREFIXRules/Classes/ShadowREL_PATH_SUFFIX) college grants you a triggered action, as shown on the College Triggered Actions table.

      ###### College Triggered Actions Table
      | College         | Triggered Action                                                                                                               |
      | --------------- | ------------------------------------------------------------------------------------------------------------------------------ |
      | Black Ash       | [In All This Confusion](REL_PATH_PREFIXRules/Abilities/Shadow/1st-Level%20Features/In%20All%20This%20ConfusionREL_PATH_SUFFIX) |
      | Caustic Alchemy | [Defensive Roll](REL_PATH_PREFIXRules/Abilities/Shadow/1st-Level%20Features/Defensive%20RollREL_PATH_SUFFIX)                   |
      | Harlequin Mask  | Clever Trick                                                                                                                   |
    features:
      - type: feature
        feature_type: ability
        name: Clever Trick
        cost: 1 Insight
        flavor: You sow a moment of confusion in combat, to your enemy's peril.
        keywords:
          - Magic
        usage: Triggered
        distance: Self
        target: Self
        trigger: An enemy targets you with a strike.
        effects:
          - name: Effect
            effect: Choose an enemy within distance of the triggering strike, including the
              enemy who targeted you. The strike targets that enemy instead.
      - type: feature
        feature_type: ability
        name: Defensive Roll
        flavor: When an enemy attacks, you roll with the impact to reduce the harm.
        keywords:
          - "-"
        usage: Triggered
        distance: Self
        target: Self
        trigger: Another creature damages you.
        effects:
          - name: Effect
            effect: You take half the triggering damage, then can shift up to 2 squares
              after the triggering effect resolves. If you end this shift with
              concealment or cover, you can use the
              [Hide](REL_PATH_PREFIXRules/Abilities/Common/Maneuvers/HideREL_PATH_SUFFIX)
              maneuver even if you are observed.
          - cost: Spend 1 Insight
            effect: The potency of any effects associated with the damage are reduced by 1
              for you.
      - type: feature
        feature_type: ability
        name: In All This Confusion
        flavor: You vanish in a plume of black smoke to avoid danger.
        keywords:
          - Magic
        usage: Triggered
        distance: Self
        target: Self
        trigger: You take damage.
        effects:
          - name: Effect
            effect: You take half the damage, then can
              [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              up to 4 squares after the triggering effect resolves.
          - cost: Spend 1+ Insight
            effect: You [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX) 1
              additional square for each insight spent.
```