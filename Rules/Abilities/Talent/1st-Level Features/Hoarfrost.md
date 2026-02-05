---
ability_type: Signature
action_type: Main action
class: talent
distance: Ranged 10
feature_type: ability
file_basename: Hoarfrost
file_dpath: Abilities/Talent/1st-Level Features
flavor: You blast a foe with a pulse of cold energy.
item_id: hoarfrost
item_index: '06'
item_name: Hoarfrost
keywords:
- Cryokinesis
- Psionic
- Ranged
- Strike
level: 1
scc:
- mcdm.heroes.v1:feature.ability.talent.1st-level-feature:hoarfrost
scdc:
- 1.1.1:11.2.1.1:06
source: mcdm.heroes.v1
target: One creature
type: feature/ability/talent/1st-level-feature
---

```ds-feature
type: feature
feature_type: ability
name: Hoarfrost
flavor: You blast a foe with a pulse of cold energy.
keywords:
  - Cryokinesis
  - Psionic
  - Ranged
  - Strike
usage: Main action
distance: Ranged 10
target: One creature
metadata:
  ability_type: Signature
  action_type: Main action
  class: talent
  distance: Ranged 10
  feature_type: ability
  file_basename: Hoarfrost
  file_dpath: Abilities/Talent/1st-Level Features
  flavor: You blast a foe with a pulse of cold energy.
  item_id: hoarfrost
  item_index: "06"
  item_name: Hoarfrost
  keywords:
    - Cryokinesis
    - Psionic
    - Ranged
    - Strike
  level: 1
  scc:
    - mcdm.heroes.v1:feature.ability.talent.1st-level-feature:hoarfrost
  scdc:
    - 1.1.1:11.2.1.1:06
  source: mcdm.heroes.v1
  target: One creature
  type: feature/ability/talent/1st-level-feature
effects:
  - roll: Power Roll + Reason
    tier1: 2 + R cold damage; M < WEAK,
      [slowed](%7BREL_PATH_PREFIX%7DRules/Conditions/Slowed%7BREL_PATH_SUFFIX%7D)
      (EoT)
    tier2: 4 + R cold damage; M < AVERAGE,
      [slowed](%7BREL_PATH_PREFIX%7DRules/Conditions/Slowed%7BREL_PATH_SUFFIX%7D)
      (EoT)
    tier3: 6 + R cold damage; M < STRONG,
      [slowed](%7BREL_PATH_PREFIX%7DRules/Conditions/Slowed%7BREL_PATH_SUFFIX%7D)
      (EoT)
  - name: Strained
    effect: You are
      [slowed](%7BREL_PATH_PREFIX%7DRules/Conditions/Slowed%7BREL_PATH_SUFFIX%7D)
      until the end of your next turn. Additionally, a target
      [slowed](%7BREL_PATH_PREFIX%7DRules/Conditions/Slowed%7BREL_PATH_SUFFIX%7D)
      by this ability is
      [restrained](%7BREL_PATH_PREFIX%7DRules/Conditions/Restrained%7BREL_PATH_SUFFIX%7D)
      instead.
```