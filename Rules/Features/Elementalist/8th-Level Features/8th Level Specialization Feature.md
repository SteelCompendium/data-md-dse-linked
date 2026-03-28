---
action_type: feature
class: elementalist
feature_type: trait
file_basename: 8th Level Specialization Feature
file_dpath: Features/Elementalist/8th-Level Features
item_id: 8th-level-specialization-feature
item_index: '02'
item_name: 8th-Level Specialization Feature
level: 8
scc:
- mcdm.heroes.v1:feature.trait.elementalist.8th-level-feature:8th-level-specialization-feature
scdc:
- 1.1.1:11.1.9.2:02
source: mcdm.heroes.v1
type: feature/trait/elementalist/8th-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: 8th-Level Specialization Feature
metadata:
  action_type: feature
  class: elementalist
  feature_type: trait
  file_basename: 8th Level Specialization Feature
  file_dpath: Features/Elementalist/8th-Level Features
  item_id: 8th-level-specialization-feature
  item_index: "02"
  item_name: 8th-Level Specialization Feature
  level: 8
  scc:
    - mcdm.heroes.v1:feature.trait.elementalist.8th-level-feature:8th-level-specialization-feature
  scdc:
    - 1.1.1:11.1.9.2:02
  source: mcdm.heroes.v1
  type: feature/trait/elementalist/8th-level-feature
effects:
  - effect: |-
      Your [elemental specialization](REL_PATH_PREFIXRules/Features/Elementalist/1st-Level%20Features/Elemental%20SpecializationREL_PATH_SUFFIX) grants you a feature, as shown on the 8th-Level [Elemental Specialization](REL_PATH_PREFIXRules/Features/Elementalist/1st-Level%20Features/Elemental%20SpecializationREL_PATH_SUFFIX) Features table.

      ###### 8th-Level Elemental Specialization Features Table
      | Specialization | Feature                                                                                                                                                                |
      | -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
      | Earth          | [Summon Source of Earth](REL_PATH_PREFIXRules/Abilities/Elementalist/8th-Level%20Features/Summon%20Source%20of%20EarthREL_PATH_SUFFIX)                                 |
      | Fire           | [The Flame Primordial](REL_PATH_PREFIXRules/Features/Elementalist/8th-Level%20Features/8th-Level%20Specialization%20Feature/The%20Flame%20PrimordialREL_PATH_SUFFIX)   |
      | Green          | [Chimeric Manifestation](REL_PATH_PREFIXRules/Features/Elementalist/8th-Level%20Features/8th-Level%20Specialization%20Feature/Chimeric%20ManifestationREL_PATH_SUFFIX) |
      | Void           | [Black Hole Star](REL_PATH_PREFIXRules/Features/Elementalist/8th-Level%20Features/8th-Level%20Specialization%20Feature/Black%20Hole%20StarREL_PATH_SUFFIX)             |
      ##### Black Hole Star
      You warp gravity around your heavenly body and can pull even the sturdiest titans toward your core. At the end of each of your turns, you target one creature or object within distance of your [Hurl Element](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Hurl%20ElementREL_PATH_SUFFIX) ability and [vertical](REL_PATH_PREFIXRules/Movement/VerticalREL_PATH_SUFFIX) pull that target up to 5 squares. If their [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX) reduces this forced movement, they are pulled a minimum of 2 squares. This forced movement ignores [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX) for your allies.
      Additionally, your [Mantle of Essence](REL_PATH_PREFIXRules/Features/Elementalist/4th-Level%20Features/Mantle%20of%20EssenceREL_PATH_SUFFIX) improves. While in the area of the aura, enemies and objects have their [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX) reduced by an amount equal to your level.
      ##### Chimeric Manifestation
      Nature isn't static and unchanging, and neither are you. You can enter or exit your animal form as a free maneuver the first time you use your [Disciple of the Green](REL_PATH_PREFIXRules/Features/Elementalist/2nd-Level%20Features/2nd-Level%20Specialization%20Feature/Disciple%20of%20the%20GreenREL_PATH_SUFFIX) feature on your turn.
      Additionally, whenever you use your [Disciple of the Green](REL_PATH_PREFIXRules/Features/Elementalist/2nd-Level%20Features/2nd-Level%20Specialization%20Feature/Disciple%20of%20the%20GreenREL_PATH_SUFFIX) feature, you can select an additional animal form and gain the positive benefits from both forms. You can choose the size of either animal, and if both animal forms grant you the same benefit, you can choose whichever you prefer. You gain the highest speed between the two animal forms and have all types of movement from both forms.
      You can only combine animal forms whose levels add up to 12 or less. For example, you can combine a shark (8th level) with a horse (4th level), but you can't combine a shark with a bear (5th level).
      ##### The Flame Primordial
      You produce a fire that entrances the fates, distracting them from aiding your foes. Whenever you deal fire damage to a creature or object, they take an extra 1d6 fire damage. If you deal fire damage to a mundane object, you can use a free triggered action to target it with your [Return to Formlessness](REL_PATH_PREFIXRules/Abilities/Elementalist/1st-Level%20Features/Return%20to%20FormlessnessREL_PATH_SUFFIX) ability instead.
      Additionally, any enemy who starts their turn adjacent to you has fire weakness equal to your Reason score until the start of their next turn. This increases to twice your Reason score if the enemy is made of or is wearing mostly metal.
      ##### Summon Source of Earth
      You have the following ability.
    features:
      - type: feature
        feature_type: ability
        name: Summon Source of Earth
        flavor: The ground rumbles as an elemental bursts forth, ready to serve.
        keywords:
          - Earth
          - Magic
          - Ranged
        usage: Main action
        distance: Ranged 10
        target: Special
        effects:
          - name: Effect
            effect: >-
              A **source of earth** emerges from an unoccupied space within
              distance. The source takes their turn immediately after you,
              moving up to their speed and either taking a main action or a
              maneuver. The source is dismissed at the start of your next turn.

              The source starts an encounter at full Stamina, but maintains
              their current Stamina throughout the encounter, even if they are
              dismissed and you use this ability again. They can't regain
              Stamina during the encounter. When the source's Stamina is reduced
              to 0, you can't use this ability again until you earn 1 or more
              Victories.
          - name: Persistent 2
            effect: >-
              The source takes another turn. They are dismissed at the start of
              your next turn.

              ###### Source of Earth Statblock
          - effect: |-
              **Source of Earth**

              |       Elemental       |                                        -                                        |       Level 8       |                                     BRUTE                                      |                                                    EV -                                                     |
              | :-------------------: | :-----------------------------------------------------------------------------: | :-----------------: | :----------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------: |
              |    **2**<br/> Size    |                                **6**<br/> Speed                                 | **45**<br/> Stamina | **5**<br/> [Stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX) | **5**<br/> [Free Strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX) |
              | **-**<br/> Immunities | **[Burrow](REL_PATH_PREFIXRules/Movement/BurrowREL_PATH_SUFFIX)**<br/> Movement |                     |                            **-**<br/> With Captain                             |                                            **-**<br/> Weaknesses                                            |
              |   **+3**<br/> Might   |                               **+1**<br/> Agility                               | **-5**<br/> Reason  |                             **-5**<br/> Intuition                              |                                            **-3**<br/> Presence                                             |
            features:
              - type: feature
                feature_type: trait
                name: Earthwalk
                effects:
                  - effect: Difficult terrain composed of earth and stone doesn't cost the source
                      extra movement.
              - type: feature
                feature_type: trait
                name: Tunneler
                effects:
                  - effect: When the source
                      [burrows](REL_PATH_PREFIXRules/Movement/BurrowREL_PATH_SUFFIX),
                      they create a size 2 tunnel.
              - type: feature
                feature_type: trait
                name: Earth Harness
                effects:
                  - effect: A creature that has the [Earth Accepts
                      Me](REL_PATH_PREFIXRules/Abilities/Elementalist/3rd-Level%20Features/Earth%20Accepts%20MeREL_PATH_SUFFIX)
                      ability can use it as a free action to meld into the
                      source.
              - type: feature
                feature_type: ability
                name: Boulder Bash
                keywords:
                  - Melee
                  - Ranged
                  - Strike
                  - Weapon
                usage: Signature
                distance: Melee 2 or ranged 10
                target: One creature or object
                effects:
                  - roll: Power Roll + 3
                    tier1: 5 damage; push 3
                    tier2: 9 damage; push 4
                    tier3: 12 damage; push 5
```