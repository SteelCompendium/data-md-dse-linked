---
action_type: feature
class: talent
feature_type: trait
file_basename: 8th Level Tradition Features
file_dpath: Talent/8th-Level Features
item_id: 8th-level-tradition-features
item_index: '02'
item_name: 8th-Level Tradition Features
level: 8
scc:
- mcdm.heroes.v1:feature.trait.talent.8th-level-feature:8th-level-tradition-features
scdc:
- 1.1.1:11.1.1.2:02
source: mcdm.heroes.v1
type: feature/trait/talent/8th-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: 8th-Level Tradition Features
metadata:
  action_type: feature
  class: talent
  feature_type: trait
  file_basename: 8th Level Tradition Features
  file_dpath: Talent/8th-Level Features
  item_id: 8th-level-tradition-features
  item_index: "02"
  item_name: 8th-Level Tradition Features
  level: 8
  scc:
    - mcdm.heroes.v1:feature.trait.talent.8th-level-feature:8th-level-tradition-features
  scdc:
    - 1.1.1:11.1.1.2:02
  source: mcdm.heroes.v1
  type: feature/trait/talent/8th-level-feature
effects:
  - effect: |-
      Your [talent](REL_PATH_PREFIXRules/Classes/TalentREL_PATH_SUFFIX) tradition grants you two features, as shown on the 8th-Level Tradition Features table.

      ###### 8th-Level Tradition Features Table
      | Tradition   | Features                                                                                                                                                                                                                                        |
      | ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
      | Chronopathy | [Doubling the Hours](REL_PATH_PREFIXRules/Talent/8th-Level%20Features/8th-Level%20Tradition%20Features/Doubling%20the%20HoursREL_PATH_SUFFIX), [Stasis Shield](REL_PATH_PREFIXRules/Talent/8th-Level%20Features/Stasis%20ShieldREL_PATH_SUFFIX) |
      | Telekinesis | [Levitation Field](REL_PATH_PREFIXRules/Abilities/Talent/8th-Level%20Features/Levitation%20FieldREL_PATH_SUFFIX), [Low Gravity](REL_PATH_PREFIXRules/Talent/8th-Level%20Features/8th-Level%20Tradition%20Features/Low%20GravityREL_PATH_SUFFIX) |
      | Telepathy   | [Mindlink](REL_PATH_PREFIXRules/Talent/8th-Level%20Features/8th-Level%20Tradition%20Features/MindlinkREL_PATH_SUFFIX), [Universal Connection](REL_PATH_PREFIXRules/Talent/8th-Level%20Features/Universal%20ConnectionREL_PATH_SUFFIX)           |
      ##### Doubling the Hours
      While you have 5 or more Victories, you can undertake an additional respite activity during a respite.
      ##### Levitation Field
      You have the following ability.
    features:
      - type: feature
        feature_type: ability
        name: Levitation Field
        flavor: You manipulate the air around your allies so they can move as freely
          through the sky as you can.
        keywords:
          - Area
          - Psionic
        usage: Maneuver
        distance: 3 burst
        target: Each ally in the area
        effects:
          - name: Effect
            effect: Each target can [fly](REL_PATH_PREFIXRules/Movement/FlyREL_PATH_SUFFIX)
              until the start of your next turn, and can immediately shift up to
              their speed. You can also shift up to your speed. While
              [flying](REL_PATH_PREFIXRules/Movement/FlyREL_PATH_SUFFIX), a
              target's
              [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX)
              is reduced to 0 and can't be increased.
          - cost: Spend 5 Clarity
            effect: The effects last for 1 hour instead.
  - effect: |-
      ##### Low Gravity

      Your mind can carry your body through tough times. You ignore difficult terrain and don't need to spend additional movement while [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX).
      ##### Mindlink
      During a respite, you can choose a number of creatures up to your Reason score who you have communicated with using your [Telepathic Speech](REL_PATH_PREFIXRules/Talent/1st-Level%20Features/Telepathic%20SpeechREL_PATH_SUFFIX) feature, creating a telepathic link among all of you. Whenever a linked creature spends one or more Recoveries, each other linked creature can spend a Recovery.
```