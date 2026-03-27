---
class: combat
file_basename: Charge
file_dpath: Abilities/Common/Main Actions
item_id: charge
item_index: '03'
item_name: Charge
scc:
- mcdm.heroes.v1:common-ability.main-action:charge
scdc:
- 1.1.1:15.1:03
source: mcdm.heroes.v1
type: common-ability/main-action
---

```ds-feature
type: feature
feature_type: trait
name: Charge
metadata:
  class: combat
  file_basename: Charge
  file_dpath: Abilities/Common/Main Actions
  item_id: charge
  item_index: "03"
  item_name: Charge
  scc:
    - mcdm.heroes.v1:common-ability.main-action:charge
  scdc:
    - 1.1.1:15.1:03
  source: mcdm.heroes.v1
  type: common-ability/main-action
effects:
  - effect: |-
      When a creature takes the [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX) main action, they move up to their speed in a straight line, then make a melee [free strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX) (see [Free Strikes](#page-289-1) below) against a target when they end their move. If the creature has an ability with the [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX) keyword, they can use that ability against the target instead of a [free strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX).

      A creature can't move through difficult terrain or shift when they [charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX). They can [fly](REL_PATH_PREFIXRules/Movement/FlyREL_PATH_SUFFIX) or [burrow](REL_PATH_PREFIXRules/Movement/BurrowREL_PATH_SUFFIX) as part of the [Charge](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/ChargeREL_PATH_SUFFIX) main action if they have that movement available to them, but they can't [climb](REL_PATH_PREFIXRules/Movement/Climb%20or%20SwimREL_PATH_SUFFIX) or [swim](REL_PATH_PREFIXRules/Movement/Climb%20or%20SwimREL_PATH_SUFFIX) while charging unless they can automatically use that movement at full speed.
```