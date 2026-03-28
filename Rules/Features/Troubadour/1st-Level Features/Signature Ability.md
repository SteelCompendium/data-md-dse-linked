---
action_type: feature
class: troubadour
feature_type: trait
file_basename: Signature Ability
file_dpath: Features/Troubadour/1st-Level Features
item_id: signature-ability
item_index: '06'
item_name: Signature Ability
level: 1
scc:
- mcdm.heroes.v1:feature.trait.troubadour.1st-level-feature:signature-ability
scdc:
- 1.1.1:11.1.3.1:06
source: mcdm.heroes.v1
type: feature/trait/troubadour/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Signature Ability
metadata:
  action_type: feature
  class: troubadour
  feature_type: trait
  file_basename: Signature Ability
  file_dpath: Features/Troubadour/1st-Level Features
  item_id: signature-ability
  item_index: "06"
  item_name: Signature Ability
  level: 1
  scc:
    - mcdm.heroes.v1:feature.trait.troubadour.1st-level-feature:signature-ability
  scdc:
    - 1.1.1:11.1.3.1:06
  source: mcdm.heroes.v1
  type: feature/trait/troubadour/1st-level-feature
effects:
  - effect: Choose one signature ability from the following options. Signature
      abilities can be used at will. (*Quick Build:* [Witty
      Banter](REL_PATH_PREFIXRules/Abilities/Troubadour/1st-Level%20Features/Witty%20BanterREL_PATH_SUFFIX).)
    features:
      - type: feature
        feature_type: ability
        name: Artful Flourish
        flavor: And they said practicing fencing was a waste!
        keywords:
          - Melee
          - Strike
          - Weapon
        usage: Main action
        distance: Melee 1
        target: Two creatures or objects
        effects:
          - roll: Power Roll + Agility
            tier1: 2 damage
            tier2: 5 damage
            tier3: 7 damage
          - name: Effect
            effect: You can shift up to 3 squares.
          - cost: Spend 2+ Drama
            effect: You can target one additional creature or object for every 2 drama
              spent.
      - type: feature
        feature_type: ability
        name: Cutting Sarcasm
        flavor: There you are, radiating your usual charisma.
        keywords:
          - Magic
          - Ranged
          - Strike
          - Weapon
        usage: Main action
        distance: Ranged 10
        target: One creature
        effects:
          - roll: Power Roll + Presence
            tier1: 2 + P psychic damage; P < WEAK,
              [bleeding](REL_PATH_PREFIXRules/Conditions/BleedingREL_PATH_SUFFIX)
              (save ends)
            tier2: 5 + P psychic damage; P < AVERAGE,
              [bleeding](REL_PATH_PREFIXRules/Conditions/BleedingREL_PATH_SUFFIX)
              (save ends)
            tier3: 7 + P psychic damage; P < STRONG,
              [bleeding](REL_PATH_PREFIXRules/Conditions/BleedingREL_PATH_SUFFIX)
              (save ends)
      - type: feature
        feature_type: ability
        name: Instigator
        flavor: I didn't do it! What?
        keywords:
          - Melee
          - Strike
          - Weapon
        usage: Main action
        distance: Melee 1
        target: One creature
        effects:
          - roll: Power Roll + Presence
            tier1: 3 + P damage
            tier2: 6 + P damage
            tier3: 9 + P damage
          - name: Effect
            effect: The target is
              [taunted](REL_PATH_PREFIXRules/Conditions/TauntedREL_PATH_SUFFIX)
              by you or a willing ally adjacent to you until the end of the
              target's next turn.
      - type: feature
        feature_type: ability
        name: Witty Banter
        flavor: A lyrical (and physical) jab insults an enemy and inspires an ally.
        keywords:
          - Magic
          - Melee
          - Ranged
          - Strike
        usage: Main action
        distance: Melee 1 or ranged 5
        target: One creature
        effects:
          - roll: Power Roll + Presence
            tier1: 4 + P psychic damage
            tier2: 5 + P psychic damage
            tier3: 7 + P psychic damage
          - name: Effect
            effect: One ally within 10 squares of you can end one effect on them that is
              ended by a saving throw or that ends at the end of their turn.
          - cost: Spend 1 Drama
            effect: The chosen ally can spend a Recovery.
  - effect: >-
      ##### Heroic Abilities


      You master a range of heroic abilities, all of which cost drama to empower
      them.

      ###### 3-Drama Ability

      Choose one heroic ability from the following options, each of which costs
      3 drama to use. (*Quick Build:* Harsh Critic.)
    features:
      - type: feature
        feature_type: ability
        name: Harsh Critic
        cost: 3 Drama
        flavor: Just one bad review will ruin their day.
        keywords:
          - Magic
          - Melee
          - Ranged
          - Strike
        usage: Main action
        distance: Melee 1 or ranged 10
        target: One creature or object
        effects:
          - roll: Power Roll + Presence
            tier1: 7 + P sonic damage
            tier2: 10 + P sonic damage
            tier3: 13 + P sonic damage
          - name: Effect
            effect: The first time the target uses an ability before the start of your next
              turn, any effects from the ability's tier outcomes other than
              damage are negated for all targets. Ability effects that always
              happen regardless of the power roll work as usual.
      - type: feature
        feature_type: ability
        name: Hypnotic Overtones
        cost: 3 Drama
        flavor: You produce an entrancing note that twists the senses in a spectacular
          fashion.
        keywords:
          - Area
          - Magic
        usage: Main action
        distance: 2 burst
        target: Each enemy in the area
        effects:
          - roll: Power Roll + Presence
            tier1: Slide 1; I < WEAK,
              [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
            tier2: Slide 1; I < AVERAGE,
              [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
            tier3: Slide 2; I < STRONG,
              [dazed](REL_PATH_PREFIXRules/Conditions/DazedREL_PATH_SUFFIX)
              (save ends)
          - cost: Spend 2+ Drama
            effect: The size of the burst increases by 1 for every 2 drama spent.
      - type: feature
        feature_type: ability
        name: Quick Rewrite
        cost: 3 Drama
        flavor: You write something unexpected into the scene that hinders your enemy.
        keywords:
          - Area
          - Magic
          - Ranged
        usage: Main action
        distance: 3 cube within 10
        target: Each enemy in the area
        effects:
          - roll: Power Roll + Presence
            tier1: 4 damage; P < WEAK,
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX)
              (save ends)
            tier2: 5 damage; P < AVERAGE,
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX)
              (save ends)
            tier3: 6 damage; P < STRONG,
              [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX)
              (save ends)
          - name: Effect
            effect: The area is difficult terrain for enemies.
      - type: feature
        feature_type: ability
        name: Upstage
        cost: 3 Drama
        flavor: As you bob and weave through the crowd, you can't help but leave the
          audience wanting more.
        keywords:
          - Melee
          - Strike
          - Weapon
        usage: Maneuver
        distance: Self; see below
        target: Self
        effects:
          - name: Effect
            effect: You shift up to your speed. You make one power roll that targets each
              enemy you move adjacent to during this shift.
          - roll: Power Roll + Agility or Presence
            tier1: "[Taunted](REL_PATH_PREFIXRules/Conditions/TauntedREL_PATH_SUFFIX) (EoT);
              A < WEAK,
              [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX)"
            tier2: "[Taunted](REL_PATH_PREFIXRules/Conditions/TauntedREL_PATH_SUFFIX) (EoT);
              A < AVERAGE,
              [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX)"
            tier3: "[Taunted](REL_PATH_PREFIXRules/Conditions/TauntedREL_PATH_SUFFIX) (EoT);
              A < STRONG,
              [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) and
              can't stand (EoT)"
  - effect: >-
      ###### 5-Drama Ability


      Choose one heroic ability from the following options, each of which costs
      5 drama to use. (*Quick Build:* Dramatic Reversal.)
    features:
      - type: feature
        feature_type: ability
        name: Dramatic Reversal
        cost: 5 Drama
        flavor: Give the audience a surprise.
        keywords:
          - Area
          - Magic
        usage: Main action
        distance: 3 burst
        target: Self and each ally in the area
        effects:
          - roll: Power Roll + Presence
            tier1: The target can shift 1 square and make a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX).
            tier2: The target can shift up to 2 squares and make a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              that gains an edge.
            tier3: The target can shift up to 3 squares and make a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              that gains an edge, then can spend a Recovery.
      - type: feature
        feature_type: ability
        name: Fake Your Death
        cost: 5 Drama
        flavor: O happy dagger, this is thy sheath!
        keywords:
          - Magic
        usage: Maneuver
        distance: Self
        target: Self
        effects:
          - name: Effect
            effect: You turn invisible and create a magical illusion of your corpse falling
              in your space. While you are invisible, you gain a +3 bonus to
              speed and you ignore difficult terrain. The illusion and your
              invisibility last until the end of your next turn, or until the
              illusion is interacted with, you take damage, or you use a main
              action or a maneuver.
      - type: feature
        feature_type: ability
        name: Flip the Script
        cost: 5 Drama
        flavor: You try a different take on events, justifying the new locations
          everyone ended up in.
        keywords:
          - Area
          - Magic
        usage: Main action
        distance: 3 burst
        target: Self and each ally in the area
        effects:
          - name: Effect
            effect: Each target can
              [teleport](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              up to 5 squares. Any
              [teleported](REL_PATH_PREFIXRules/Movement/TeleportREL_PATH_SUFFIX)
              target who was
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) is
              no longer
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX).
      - type: feature
        feature_type: ability
        name: Method Acting
        cost: 5 Drama
        flavor: They're so hurt by your performance, you start to believe it yourself.
        keywords:
          - Melee
          - Strike
          - Weapon
        usage: Main action
        distance: Melee 1
        target: One creature
        effects:
          - roll: Power Roll + Agility
            tier1: 6 + A damage; P < WEAK,
              [weakened](REL_PATH_PREFIXRules/Conditions/WeakenedREL_PATH_SUFFIX)
              (save ends)
            tier2: 10 + A damage; P < AVERAGE,
              [weakened](REL_PATH_PREFIXRules/Conditions/WeakenedREL_PATH_SUFFIX)
              (save ends)
            tier3: 14 + A damage; P < STRONG,
              [weakened](REL_PATH_PREFIXRules/Conditions/WeakenedREL_PATH_SUFFIX)
              (save ends)
          - name: Effect
            effect: You can become
              [bleeding](REL_PATH_PREFIXRules/Conditions/BleedingREL_PATH_SUFFIX)
              (save ends) to deal an extra 5 corruption damage to the target.
```