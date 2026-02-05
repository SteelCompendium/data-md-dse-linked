---
action_type: Main action
class: fury
cost: 5 Ferocity
cost_amount: 5
cost_resource: Ferocity
distance: Melee 1
feature_type: ability
file_basename: Death Death
file_dpath: Abilities/Fury/2nd-Level Features
flavor: Your unbridled rage strikes terror in their hearts.
item_id: death-death-5-ferocity
item_index: '01'
item_name: Death... Death! (5 Ferocity)
keywords:
- Melee
- Strike
- Weapon
level: 2
scc:
- mcdm.heroes.v1:feature.ability.fury.2nd-level-feature:death-death-5-ferocity
scdc:
- 1.1.1:11.2.5.5:01
source: mcdm.heroes.v1
target: One creature
type: feature/ability/fury/2nd-level-feature
---

```ds-feature
type: feature
feature_type: ability
name: Death... Death!
cost: 5 Ferocity
flavor: Your unbridled rage strikes terror in their hearts.
keywords:
  - Melee
  - Strike
  - Weapon
usage: Main action
distance: Melee 1
target: One creature
metadata:
  action_type: Main action
  class: fury
  cost: 5 Ferocity
  cost_amount: 5
  cost_resource: Ferocity
  distance: Melee 1
  feature_type: ability
  file_basename: Death Death
  file_dpath: Abilities/Fury/2nd-Level Features
  flavor: Your unbridled rage strikes terror in their hearts.
  item_id: death-death-5-ferocity
  item_index: "01"
  item_name: Death... Death! (5 Ferocity)
  keywords:
    - Melee
    - Strike
    - Weapon
  level: 2
  scc:
    - mcdm.heroes.v1:feature.ability.fury.2nd-level-feature:death-death-5-ferocity
  scdc:
    - 1.1.1:11.2.5.5:01
  source: mcdm.heroes.v1
  target: One creature
  type: feature/ability/fury/2nd-level-feature
effects:
  - roll: Power Roll + Might
    tier1: 3 + M damage; P < WEAK,
      [dazed](%7BREL_PATH_PREFIX%7DRules/Conditions/Dazed%7BREL_PATH_SUFFIX%7D)
      and
      [frightened](%7BREL_PATH_PREFIX%7DRules/Conditions/Frightened%7BREL_PATH_SUFFIX%7D)
      (save ends)
    tier2: 5 + M damage; P < AVERAGE,
      [dazed](%7BREL_PATH_PREFIX%7DRules/Conditions/Dazed%7BREL_PATH_SUFFIX%7D)
      and
      [frightened](%7BREL_PATH_PREFIX%7DRules/Conditions/Frightened%7BREL_PATH_SUFFIX%7D)
      (save ends)
    tier3: 8 + M damage; P < STRONG,
      [dazed](%7BREL_PATH_PREFIX%7DRules/Conditions/Dazed%7BREL_PATH_SUFFIX%7D)
      and
      [frightened](%7BREL_PATH_PREFIX%7DRules/Conditions/Frightened%7BREL_PATH_SUFFIX%7D)
      (save ends)
```