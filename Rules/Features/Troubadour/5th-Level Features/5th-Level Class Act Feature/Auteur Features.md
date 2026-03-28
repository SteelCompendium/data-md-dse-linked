---
action_type: feature
class: troubadour
feature_type: subtrait
file_basename: Auteur Features
file_dpath: Features/Troubadour/5th-Level Features/5th-Level Class Act Feature
item_id: auteur-features
item_index: '01'
item_name: Auteur Features
level: 5
scc:
- mcdm.heroes.v1:feature.subtrait.troubadour.5th-level-feature:auteur-features
scdc:
- 1.1.1:11.2.3.5:01
source: mcdm.heroes.v1
type: feature/subtrait/troubadour/5th-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Auteur Features
metadata:
  action_type: feature
  class: troubadour
  feature_type: subtrait
  file_basename: Auteur Features
  file_dpath: Features/Troubadour/5th-Level Features/5th-Level Class Act Feature
  item_id: auteur-features
  item_index: "01"
  item_name: Auteur Features
  level: 5
  scc:
    - mcdm.heroes.v1:feature.subtrait.troubadour.5th-level-feature:auteur-features
  scdc:
    - 1.1.1:11.2.3.5:01
  source: mcdm.heroes.v1
  type: feature/subtrait/troubadour/5th-level-feature
effects:
  - effect: |-
      Choose one of the following features.

      ###### Fix It in Post
      Once on each of your turns, you can use a free maneuver to change one condition affecting a creature within distance of your [Dramatic Monologue](REL_PATH_PREFIXRules/Abilities/Troubadour/1st-Level%20Features/Dramatic%20MonologueREL_PATH_SUFFIX) ability. Choose one of the following conditions on the target: [bleeding](REL_PATH_PREFIXRules/Conditions/BleedingREL_PATH_SUFFIX), [frightened](REL_PATH_PREFIXRules/Conditions/FrightenedREL_PATH_SUFFIX), [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX), [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX), or [taunted](REL_PATH_PREFIXRules/Conditions/TauntedREL_PATH_SUFFIX). You change that condition to another of those conditions, maintaining the duration and origin of the original condition. A target who is no longer [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) can stand up.
      ###### Take Two!
      You have the following performance ability, which is usable with your [Routines](REL_PATH_PREFIXRules/Features/Troubadour/1st-Level%20Features/RoutinesREL_PATH_SUFFIX) feature.
    features:
      - type: feature
        feature_type: ability
        name: Take Two!
        flavor: One more, and this time make it interesting.
        keywords:
          - Area
          - Magic
          - Performance
        usage: No action
        distance: 5 aura
        target: Self and each ally in the area
        effects:
          - name: Effect
            effect: While this performance is active, each target who starts their turn in
              the area can reroll the first power roll that turn that obtains a
              tier 2 outcome. They must use the new roll.
```