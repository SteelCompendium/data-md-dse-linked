---
action_type: feature
class: talent
feature_type: subtrait
file_basename: Heroic Abilities
file_dpath: Features/Talent/1st-Level Features/Talent Abilities
item_id: heroic-abilities
item_index: '02'
item_name: Heroic Abilities
level: 1
scc:
- mcdm.heroes.v1:feature.subtrait.talent.1st-level-feature:heroic-abilities
scdc:
- 1.1.1:11.2.1.6:02
source: mcdm.heroes.v1
type: feature/subtrait/talent/1st-level-feature
---

```ds-feature
type: feature
feature_type: trait
name: Heroic Abilities
metadata:
  action_type: feature
  class: talent
  feature_type: subtrait
  file_basename: Heroic Abilities
  file_dpath: Features/Talent/1st-Level Features/Talent Abilities
  item_id: heroic-abilities
  item_index: "02"
  item_name: Heroic Abilities
  level: 1
  scc:
    - mcdm.heroes.v1:feature.subtrait.talent.1st-level-feature:heroic-abilities
  scdc:
    - 1.1.1:11.2.1.6:02
  source: mcdm.heroes.v1
  type: feature/subtrait/talent/1st-level-feature
effects:
  - effect: |-
      You know a range of heroic abilities, all of which cost clarity to fuel them.

      ###### 3-Clarity Ability
      Choose one heroic ability from the following options, each of which costs 3 clarity to use. (*Quick Build:* [Choke](REL_PATH_PREFIXRules/Abilities/Talent/1st-Level%20Features/ChokeREL_PATH_SUFFIX).)
    features:
      - type: feature
        feature_type: ability
        name: Awe
        cost: 3 Clarity
        flavor: You project psionic energy out to a creature and take on a new visage in
          their mind.
        keywords:
          - Psionic
          - Ranged
          - Strike
          - Telepathy
        usage: Main action
        distance: Ranged 10
        target: One creature
        effects:
          - name: Effect
            effect: If you target an ally, they gain temporary Stamina equal to three times
              your Presence score, and they can end one effect on them that is
              ended by a saving throw or that ends at the end of their turn. If
              you target an enemy, you make a power roll.
          - roll: Power Roll + Presence
            tier1: 3 + P psychic damage; I < WEAK,
              [frightened](REL_PATH_PREFIXRules/Conditions/FrightenedREL_PATH_SUFFIX)
              (save ends)
            tier2: 6 + P psychic damage; I < AVERAGE,
              [frightened](REL_PATH_PREFIXRules/Conditions/FrightenedREL_PATH_SUFFIX)
              (save ends)
            tier3: 9 + P psychic damage; I < STRONG,
              [frightened](REL_PATH_PREFIXRules/Conditions/FrightenedREL_PATH_SUFFIX)
              (save ends)
      - type: feature
        feature_type: ability
        name: Choke
        cost: 3 Clarity
        flavor: You crush a foe in a telekinetic grip.
        keywords:
          - Psionic
          - Ranged
          - Strike
          - Telekinesis
        usage: Main action
        distance: Ranged 10
        target: One creature
        effects:
          - roll: Power Roll + Reason
            tier1: 3 + R damage; M < WEAK,
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX)
              (save ends)
            tier2: 5 + R damage; M < AVERAGE,
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX)
              (save ends)
            tier3: 8 + R damage; M < STRONG,
              [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX)
              (save ends)
          - name: Effect
            effect: You can
              [vertical](REL_PATH_PREFIXRules/Movement/VerticalREL_PATH_SUFFIX)
              pull the target up to 2 squares. If the target is made
              [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX)
              by this ability, this forced movement ignores their
              [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX).
      - type: feature
        feature_type: ability
        name: Precognition
        cost: 3 Clarity
        flavor: You give a target a glimpse into the future so that they're ready for
          what comes next.
        keywords:
          - Chronopathy
          - Melee
          - Psionic
        usage: Main action
        distance: Melee 2
        target: Self or one ally
        effects:
          - name: Effect
            effect: Ability rolls made against the target take a bane until the start of
              your next turn. Whenever the target takes damage while under this
              effect, they can use a triggered action to make a [free
              strike](REL_PATH_PREFIXRules/Abilities/Common/Main%20Actions/Free%20StrikeREL_PATH_SUFFIX)
              against the source of the damage.
      - type: feature
        feature_type: ability
        name: Smolder
        cost: 3 Clarity
        flavor: Smoke flows from your enemy like tears as their skin begins to blacken
          and flake.
        keywords:
          - Psionic
          - Pyrokinesis
          - Ranged
          - Strike
        usage: Main action
        distance: Ranged 10
        target: One creature
        effects:
          - name: Effect
            effect: "Choose the damage type and the weakness for this ability from one of
              the following: acid, corruption, or fire. The target takes damage
              before this ability imposes any weakness."
          - roll: Power Roll + Reason
            tier1: 3 + R damage; R < WEAK, the target has weakness 5 (save ends)
            tier2: 6 + R damage; R < AVERAGE, the target has weakness 5 (save ends)
            tier3: 9 + R damage; R < STRONG, the target has weakness equal to 5 + your
              Reason score (save ends)
  - effect: |-
      ###### 5-Clarity Ability

      Choose one heroic ability from the following options, each of which costs 5 clarity to use. (*Quick Build:* [Inertia Soak](REL_PATH_PREFIXRules/Abilities/Talent/1st-Level%20Features/Inertia%20SoakREL_PATH_SUFFIX).)
    features:
      - type: feature
        feature_type: ability
        name: Flashback
        cost: 5 Clarity
        flavor: The target is thrown several seconds back through time and gets to do it
          all again.
        keywords:
          - Chronopathy
          - Psionic
          - Ranged
        usage: Maneuver
        distance: Ranged 10
        target: Self or one ally
        effects:
          - name: Effect
            effect: The target uses an ability with a base Heroic Resource cost of 7 or
              lower that they've previously used this round, without needing to
              spend the base cost. Augmentations to the ability can be paid for
              as usual.
          - name: Strained
            effect: You take 1d6 damage and are
              [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX)
              (save ends).
      - type: feature
        feature_type: ability
        name: Inertia Soak
        cost: 5 Clarity
        flavor: Your psionic energy surrounds the target and pushes everything else away
          from them.
        keywords:
          - Psionic
          - Ranged
          - Telekinesis
        usage: Maneuver
        distance: Ranged 10
        target: Self or one ally
        effects:
          - name: Effect
            effect: The target ignores difficult terrain and takes no damage from forced
              movement until the start of your next turn. Whenever the target
              enters a square while under this effect, they can push one
              adjacent creature up to a number of squares equal to your Reason
              score. When pushing an ally, the target can ignore that ally's
              [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX).
              A creature can only be force moved this way once a turn.
          - name: Strained
            effect: You are
              [weakened](REL_PATH_PREFIXRules/Conditions/WeakenedREL_PATH_SUFFIX)
              (save ends). While you are
              [weakened](REL_PATH_PREFIXRules/Conditions/WeakenedREL_PATH_SUFFIX)
              this way, whenever you are force moved, the forced movement
              distance gains a +5 bonus.
      - type: feature
        feature_type: ability
        name: Iron
        cost: 5 Clarity
        flavor: The target's skin turns to hard, dark metal, impenetrable and dense.
        keywords:
          - Metamorphosis
          - Psionic
          - Ranged
        usage: Maneuver
        distance: Ranged 10
        target: Self or one ally
        effects:
          - name: Effect
            effect: The target's
              [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX)
              increases by an amount equal to your Reason score, and they gain
              10 temporary Stamina and 2 surges. This
              [stability](REL_PATH_PREFIXRules/Movement/StabilityREL_PATH_SUFFIX)
              increase lasts until the target no longer has temporary Stamina
              from this ability.
          - name: Strained
            effect: You can't use maneuvers (save ends).
      - type: feature
        feature_type: ability
        name: Perfect Clarity
        cost: 5 Clarity
        flavor: You clear the mind of nothing but the goal.
        keywords:
          - Psionic
          - Ranged
          - Telepathy
        usage: Maneuver
        distance: Ranged 10
        target: Self or one ally
        effects:
          - name: Effect
            effect: Until the start of your next turn, the target gains a +3 bonus to speed,
              and they have a double edge on the next power roll they make. If
              the target obtains a tier 3 outcome on that roll, you gain 1
              clarity.
          - name: Strained
            effect: You take 1d6 damage, and you can't use triggered actions (save ends).
```