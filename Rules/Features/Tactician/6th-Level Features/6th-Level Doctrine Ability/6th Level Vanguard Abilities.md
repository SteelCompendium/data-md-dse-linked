---
action_type: feature
class: tactician
feature_type: subtrait
file_basename: 6th Level Vanguard Abilities
file_dpath: Features/Tactician/6th-Level Features/6th-Level Doctrine Ability
item_id: 6th-level-vanguard-abilities
item_index: '01'
item_name: 6th-Level Vanguard Abilities
level: 6
scc:
- mcdm.heroes.v1:feature.subtrait.tactician.6th-level-feature:6th-level-vanguard-abilities
scdc:
- 1.1.1:11.2.4.5:01
source: mcdm.heroes.v1
type: feature/subtrait/tactician/6th-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: 6th-Level Vanguard Abilities
metadata:
  action_type: feature
  class: tactician
  feature_type: subtrait
  file_basename: 6th Level Vanguard Abilities
  file_dpath: Features/Tactician/6th-Level Features/6th-Level Doctrine Ability
  item_id: 6th-level-vanguard-abilities
  item_index: "01"
  item_name: 6th-Level Vanguard Abilities
  level: 6
  scc:
    - mcdm.heroes.v1:feature.subtrait.tactician.6th-level-feature:6th-level-vanguard-abilities
  scdc:
    - 1.1.1:11.2.4.5:01
  source: mcdm.heroes.v1
  type: feature/subtrait/tactician/6th-level-feature
effects:
  - effect: Choose one of the following abilities.
    features:
      - type: feature
        feature_type: ability
        name: Instant Retaliation
        cost: 9 Focus
        flavor: You parry with almost supernatural speed.
        keywords:
          - Melee
          - Weapon
        usage: Free triggered
        distance: Melee 1
        target: One ally
        trigger: A creature deals damage to the target.
        effects:
          - name: Effect
            effect: The target takes half the damage. You then make a power roll against the
              triggering creature.
          - roll: Power Roll + Might
            tier1: A < WEAK, [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
            tier2: A < AVERAGE,
              [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
            tier3: A < STRONG, [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
      - type: feature
        feature_type: ability
        name: To Me Squad!
        cost: 9 Focus
        flavor: You lead your allies in a charge.
        keywords:
          - "[Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Char\
            geREL_PATH_SUFFIX)"
          - Melee
          - Strike
          - Weapon
        usage: Main action
        distance: Melee 1
        target: One creature
        effects:
          - roll: Power Roll + Might
            tier1: 6 + M damage; one ally within 10 squares can use the
              [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
              main action as a free triggered action, and can use a melee strike
              signature ability instead of a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              for the
              [charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
            tier2: 9 + M damage; one ally within 10 squares can use the
              [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
              main action as a free triggered action, and can use a melee strike
              signature ability that gains an edge instead of a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              for the
              [charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
            tier3: 13 + M damage; two allies within 10 squares can use the
              [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
              main action as a free triggered action, and can each use a melee
              strike signature ability that gains an edge instead of a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              for the
              [charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX)
          - name: Effect
            effect: If the target is hit with two or more strikes as part of this ability
              and they have R < STRONG, they are
              [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends). If the target is reduced to 0 Stamina before one or
              both allies has made their strike, the ally or allies can pick a
              different target.
```