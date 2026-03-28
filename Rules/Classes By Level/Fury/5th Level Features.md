---
file_basename: 5th Level Features
file_dpath: Classes By Level/Fury
item_id: 5th-level-features
item_index: '12'
item_name: 5th-Level Features
scc:
  - mcdm.heroes.v1:class.fury.level:5th-level-features
scdc:
  - 1.1.1:2.5.1:12
source: mcdm.heroes.v1
type: class/fury/level
---

### 5th-Level Features

As a 5th-level [fury](REL_PATH_PREFIXRules/Classes/FuryREL_PATH_SUFFIX), you gain the following features.

#### 5th-Level Aspect Feature

Your [primordial aspect](REL_PATH_PREFIXRules/Features/Fury/1st-Level%20Features/Primordial%20AspectREL_PATH_SUFFIX) grants you a feature, as shown on the 5th-Level Aspect Features table.

###### 5th-Level Aspect Features Table

| Aspect     | Feature                                                                                                                      |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Berserker  | [Bounder](REL_PATH_PREFIXRules/Features/Fury/5th-Level%20Features/5th-Level%20Aspect%20Feature/BounderREL_PATH_SUFFIX)       |
| Reaver     | [Unfettered](REL_PATH_PREFIXRules/Features/Fury/5th-Level%20Features/5th-Level%20Aspect%20Feature/UnfetteredREL_PATH_SUFFIX) |
| Stormwight | [Stormborn](REL_PATH_PREFIXRules/Features/Fury/5th-Level%20Features/5th-Level%20Aspect%20Feature/StormbornREL_PATH_SUFFIX)   |

##### Bounder

Your [jump](REL_PATH_PREFIXRules/Movement/JumpREL_PATH_SUFFIX) distance and height double (see Movement Types in Chapter 10: Combat). Additionally, when you fall, you reduce the effective height of your fall by a number of squares equal to your [jump](REL_PATH_PREFIXRules/Movement/JumpREL_PATH_SUFFIX) distance for the purpose of determining damage and whether you land [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) (see Falling in Chapter 10). You are not [prone](REL_PATH_PREFIXRules/Conditions/ProneREL_PATH_SUFFIX) after falling and landing on another creature.

##### Stormborn

You and each ally within 5 squares of you ignore negative effects from inclement weather, such as banes or environmental damage. Additionally, you can use the [Blessing of Fortunate Weather](REL_PATH_PREFIXRules/Features/Censor/1st-Level%20Features/1st-Level%20Domain%20Feature/Blessing%20of%20Fortunate%20WeatherREL_PATH_SUFFIX) feature as if you were a 1st-level [conduit](REL_PATH_PREFIXRules/Classes/ConduitREL_PATH_SUFFIX) (see 1st-Level Domain Feature in the [Conduit](REL_PATH_PREFIXRules/Classes/ConduitREL_PATH_SUFFIX) section).

##### Unfettered

At the start of your turn, you can end any [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX) condition on you. Additionally, you have a double edge on tests made to escape being confined or imprisoned.

#### 9-Ferocity Ability

Choose one heroic ability from the following options, each of which costs 9 ferocity to use.

<!-- -->
> ###### Debilitating Strike (9 Ferocity)
>
> *You need just one blow to sabotage your target.*
>
> | **Melee, Strike, Weapon** |     **Main action** |
> | ------------------------- | ------------------: |
> | **📏 Melee 1**            | **🎯 One creature** |
>
> **Power Roll + Might:**
>
> - **≤11:** 10 + M damage; M < WEAK, [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) (save ends)
> - **12-16:** 14 + M damage; M < AVERAGE, [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) (save ends)
> - **17+:** 20 + M damage; M < STRONG, [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) (save ends)
>
> **Effect:** While [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) this way, the target takes 1 damage for every square they move, including from forced movement.

<!-- -->
> ###### My Turn! (9 Ferocity)
>
> *You quickly strike back at a foe.*
>
> | **Melee, Strike, Weapon** |             **Free triggered** |
> | ------------------------- | -----------------------------: |
> | **📏 Melee 1**            | **🎯 The triggering creature** |
>
> **Trigger:** A creature causes you to be winded or dying, or damages you while you are winded or dying.
>
> **Power Roll + Might:**
>
> - **≤11:** 6 + M damage
> - **12-16:** 9 + M damage
> - **17+:** 13 + M damage
>
> **Effect:** You can spend a Recovery.

<!-- -->
> ###### Rebounding Storm (9 Ferocity)
>
> *You knock around enemies like playthings.*
>
> | **Melee, Strike, Weapon** |                 **Main action** |
> | ------------------------- | ------------------------------: |
> | **📏 Melee 1**            | **🎯 Two creatures or objects** |
>
> **Power Roll + Might:**
>
> - **≤11:** 9 damage; push 3
> - **12-16:** 14 damage; push 5
> - **17+:** 19 damage; push 7
>
> **Effect:** When a target would end this forced movement by colliding with a creature or object, they take damage as usual, then are pushed the remaining distance away from the creature or object in the direction they came from. As long as forced movement remains, this effect continues if the target collides with another creature or object.

<!-- -->
> ###### To Stone! (9 Ferocity)
>
> *You channel the Primordial Chaos into blows that petrify your foe... literally.*
>
> | **Magic, Melee, Strike, Weapon** |     **Main action** |
> | -------------------------------- | ------------------: |
> | **📏 Melee 1**                   | **🎯 One creature** |
>
> **Power Roll + Might:**
>
> - **≤11:** 9 + M damage; M < WEAK, [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) (save ends)
> - **12-16:** 13 + M damage; M < AVERAGE, [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) (save ends)
> - **17+:** 18 + M damage; M < STRONG, [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX) (save ends)
>
> **Effect:** While the target is [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) this way, any other effect that would make the target [slowed](REL_PATH_PREFIXRules/Conditions/SlowedREL_PATH_SUFFIX) instead makes them [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX) by this ability. Additionally, a creature who fails the saving throw while [restrained](REL_PATH_PREFIXRules/Conditions/RestrainedREL_PATH_SUFFIX) this way is petrified until they are given a supernatural cure or you choose to reverse the effect (no action required).
