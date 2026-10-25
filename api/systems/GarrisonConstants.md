# GarrisonConstants

source `interface/addons/blizzard_apidocumentationgenerated/garrisonconstantsdocumentation.lua` (FileDataID 4637106)

## Types

### ContributionAppearanceFlags

*Enumeration* · 1 values, 0..0

Access values as `Enum.ContributionAppearanceFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TooltipUseTimeRemaining` | `ContributionAppearanceFlags` | = 0 |

### ContributionState

*Enumeration* · 5 values, 0..4

Access values as `Enum.ContributionState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ContributionState` | = 0 |
| `Building` | `ContributionState` | = 1 |
| `Active` | `ContributionState` | = 2 |
| `UnderAttack` | `ContributionState` | = 3 |
| `Destroyed` | `ContributionState` | = 4 |

### CovenantSkill

*Enumeration* · 4 values, 2730..2733

Access values as `Enum.CovenantSkill.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Kyrian` | `CovenantSkill` | = 2730 |
| `Venthyr` | `CovenantSkill` | = 2731 |
| `NightFae` | `CovenantSkill` | = 2732 |
| `Necrolord` | `CovenantSkill` | = 2733 |

### CovenantType

*Enumeration* · 5 values, 0..4

Access values as `Enum.CovenantType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CovenantType` | = 0 |
| `Kyrian` | `CovenantType` | = 1 |
| `Venthyr` | `CovenantType` | = 2 |
| `NightFae` | `CovenantType` | = 3 |
| `Necrolord` | `CovenantType` | = 4 |

### FollowerAbilityCastResult

*Enumeration* · 15 values, 0..14

Access values as `Enum.FollowerAbilityCastResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `FollowerAbilityCastResult` | = 0 |
| `Failure` | `FollowerAbilityCastResult` | = 1 |
| `NoPendingCast` | `FollowerAbilityCastResult` | = 2 |
| `InvalidTarget` | `FollowerAbilityCastResult` | = 3 |
| `InvalidFollowerSpell` | `FollowerAbilityCastResult` | = 4 |
| `RerollNotAllowed` | `FollowerAbilityCastResult` | = 5 |
| `SingleMissionDuration` | `FollowerAbilityCastResult` | = 6 |
| `MustTargetFollower` | `FollowerAbilityCastResult` | = 7 |
| `MustTargetTrait` | `FollowerAbilityCastResult` | = 8 |
| `InvalidFollowerType` | `FollowerAbilityCastResult` | = 9 |
| `MustBeUnique` | `FollowerAbilityCastResult` | = 10 |
| `CannotTargetLimitedUseFollower` | `FollowerAbilityCastResult` | = 11 |
| `MustTargetLimitedUseFollower` | `FollowerAbilityCastResult` | = 12 |
| `AlreadyAtMaxDurability` | `FollowerAbilityCastResult` | = 13 |
| `CannotTargetNonAutoMissionFollower` | `FollowerAbilityCastResult` | = 14 |

### GarrAutoBoardIndex

*Enumeration* · 14 values, -1..12

Access values as `Enum.GarrAutoBoardIndex.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrAutoBoardIndex` | = -1 |
| `AllyLeftBack` | `GarrAutoBoardIndex` | = 0 |
| `AllyRightBack` | `GarrAutoBoardIndex` | = 1 |
| `AllyLeftFront` | `GarrAutoBoardIndex` | = 2 |
| `AllyCenterFront` | `GarrAutoBoardIndex` | = 3 |
| `AllyRightFront` | `GarrAutoBoardIndex` | = 4 |
| `EnemyLeftFront` | `GarrAutoBoardIndex` | = 5 |
| `EnemyCenterLeftFront` | `GarrAutoBoardIndex` | = 6 |
| `EnemyCenterRightFront` | `GarrAutoBoardIndex` | = 7 |
| `EnemyRightFront` | `GarrAutoBoardIndex` | = 8 |
| `EnemyLeftBack` | `GarrAutoBoardIndex` | = 9 |
| `EnemyCenterLeftBack` | `GarrAutoBoardIndex` | = 10 |
| `EnemyCenterRightBack` | `GarrAutoBoardIndex` | = 11 |
| `EnemyRightBack` | `GarrAutoBoardIndex` | = 12 |

### GarrAutoCombatSpellTutorialFlag

*Enumeration* · 5 values, 0..4

Access values as `Enum.GarrAutoCombatSpellTutorialFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrAutoCombatSpellTutorialFlag` | = 0 |
| `Single` | `GarrAutoCombatSpellTutorialFlag` | = 1 |
| `Column` | `GarrAutoCombatSpellTutorialFlag` | = 2 |
| `Row` | `GarrAutoCombatSpellTutorialFlag` | = 3 |
| `All` | `GarrAutoCombatSpellTutorialFlag` | = 4 |

### GarrAutoCombatTutorial

*Enumeration* · 11 values, 1..1024

Access values as `Enum.GarrAutoCombatTutorial.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SelectMission` | `GarrAutoCombatTutorial` | = 1 |
| `PlaceCompanion` | `GarrAutoCombatTutorial` | = 2 |
| `HealCompanion` | `GarrAutoCombatTutorial` | = 4 |
| `LevelHeal` | `GarrAutoCombatTutorial` | = 8 |
| `BeneficialEffect` | `GarrAutoCombatTutorial` | = 16 |
| `AttackSingle` | `GarrAutoCombatTutorial` | = 32 |
| `AttackColumn` | `GarrAutoCombatTutorial` | = 64 |
| `AttackRow` | `GarrAutoCombatTutorial` | = 128 |
| `AttackAll` | `GarrAutoCombatTutorial` | = 256 |
| `TroopTutorial` | `GarrAutoCombatTutorial` | = 512 |
| `EnvironmentalEffect` | `GarrAutoCombatTutorial` | = 1024 |

### GarrAutoCombatantRole

*Enumeration* · 6 values, 0..5

Access values as `Enum.GarrAutoCombatantRole.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrAutoCombatantRole` | = 0 |
| `Melee` | `GarrAutoCombatantRole` | = 1 |
| `RangedPhysical` | `GarrAutoCombatantRole` | = 2 |
| `RangedMagic` | `GarrAutoCombatantRole` | = 3 |
| `HealSupport` | `GarrAutoCombatantRole` | = 4 |
| `Tank` | `GarrAutoCombatantRole` | = 5 |

### GarrAutoEventFlags

*Enumeration* · 4 values, 0..4

Access values as `Enum.GarrAutoEventFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrAutoEventFlags` | = 0 |
| `AutoAttack` | `GarrAutoEventFlags` | = 1 |
| `Passive` | `GarrAutoEventFlags` | = 2 |
| `Environment` | `GarrAutoEventFlags` | = 4 |

### GarrAutoMissionEventType

*Enumeration* · 10 values, 0..9

Access values as `Enum.GarrAutoMissionEventType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MeleeDamage` | `GarrAutoMissionEventType` | = 0 |
| `RangeDamage` | `GarrAutoMissionEventType` | = 1 |
| `SpellMeleeDamage` | `GarrAutoMissionEventType` | = 2 |
| `SpellRangeDamage` | `GarrAutoMissionEventType` | = 3 |
| `Heal` | `GarrAutoMissionEventType` | = 4 |
| `PeriodicDamage` | `GarrAutoMissionEventType` | = 5 |
| `PeriodicHeal` | `GarrAutoMissionEventType` | = 6 |
| `ApplyAura` | `GarrAutoMissionEventType` | = 7 |
| `RemoveAura` | `GarrAutoMissionEventType` | = 8 |
| `Died` | `GarrAutoMissionEventType` | = 9 |

### GarrAutoPreviewTargetType

*Enumeration* · 5 values, 0..8

Access values as `Enum.GarrAutoPreviewTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrAutoPreviewTargetType` | = 0 |
| `Damage` | `GarrAutoPreviewTargetType` | = 1 |
| `Heal` | `GarrAutoPreviewTargetType` | = 2 |
| `Buff` | `GarrAutoPreviewTargetType` | = 4 |
| `Debuff` | `GarrAutoPreviewTargetType` | = 8 |

### GarrFollowerMissionCompleteState

*Enumeration* · 4 values, 0..3

Access values as `Enum.GarrFollowerMissionCompleteState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Alive` | `GarrFollowerMissionCompleteState` | = 0 |
| `KilledByMissionFailure` | `GarrFollowerMissionCompleteState` | = 1 |
| `SavedByPreventDeath` | `GarrFollowerMissionCompleteState` | = 2 |
| `OutOfDurability` | `GarrFollowerMissionCompleteState` | = 3 |

### GarrFollowerQuality

*Enumeration* · 7 values, 0..6

Access values as `Enum.GarrFollowerQuality.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrFollowerQuality` | = 0 |
| `Common` | `GarrFollowerQuality` | = 1 |
| `Uncommon` | `GarrFollowerQuality` | = 2 |
| `Rare` | `GarrFollowerQuality` | = 3 |
| `Epic` | `GarrFollowerQuality` | = 4 |
| `Legendary` | `GarrFollowerQuality` | = 5 |
| `Title` | `GarrFollowerQuality` | = 6 |

### GarrTalentCostType

*Enumeration* · 4 values, 0..3

Access values as `Enum.GarrTalentCostType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Initial` | `GarrTalentCostType` | = 0 |
| `Respec` | `GarrTalentCostType` | = 1 |
| `MakePermanent` | `GarrTalentCostType` | = 2 |
| `TreeReset` | `GarrTalentCostType` | = 3 |

### GarrTalentFeatureSubtype

*Enumeration* · 5 values, 0..4

Access values as `Enum.GarrTalentFeatureSubtype.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Generic` | `GarrTalentFeatureSubtype` | = 0 |
| `Bastion` | `GarrTalentFeatureSubtype` | = 1 |
| `Revendreth` | `GarrTalentFeatureSubtype` | = 2 |
| `Ardenweald` | `GarrTalentFeatureSubtype` | = 3 |
| `Maldraxxus` | `GarrTalentFeatureSubtype` | = 4 |

### GarrTalentFeatureType

*Enumeration* · 9 values, 0..8

Access values as `Enum.GarrTalentFeatureType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Generic` | `GarrTalentFeatureType` | = 0 |
| `AnimaDiversion` | `GarrTalentFeatureType` | = 1 |
| `TravelPortals` | `GarrTalentFeatureType` | = 2 |
| `Adventures` | `GarrTalentFeatureType` | = 3 |
| `ReservoirUpgrades` | `GarrTalentFeatureType` | = 4 |
| `SanctumUnique` | `GarrTalentFeatureType` | = 5 |
| `SoulBinds` | `GarrTalentFeatureType` | = 6 |
| `AnimaDiversionMap` | `GarrTalentFeatureType` | = 7 |
| `Cyphers` | `GarrTalentFeatureType` | = 8 |

### GarrTalentResearchCostSource

*Enumeration* · 2 values, 0..1

Access values as `Enum.GarrTalentResearchCostSource.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Talent` | `GarrTalentResearchCostSource` | = 0 |
| `Tree` | `GarrTalentResearchCostSource` | = 1 |

### GarrTalentSocketType

*Enumeration* · 3 values, 0..2

Access values as `Enum.GarrTalentSocketType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GarrTalentSocketType` | = 0 |
| `Spell` | `GarrTalentSocketType` | = 1 |
| `Conduit` | `GarrTalentSocketType` | = 2 |

### GarrTalentTreeType

*Enumeration* · 2 values, 0..1

Access values as `Enum.GarrTalentTreeType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Tiers` | `GarrTalentTreeType` | = 0 |
| `Classic` | `GarrTalentTreeType` | = 1 |

### GarrTalentType

*Enumeration* · 4 values, 0..3

Access values as `Enum.GarrTalentType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Standard` | `GarrTalentType` | = 0 |
| `Minor` | `GarrTalentType` | = 1 |
| `Major` | `GarrTalentType` | = 2 |
| `Socket` | `GarrTalentType` | = 3 |

### GarrTalentUI

*Enumeration* · 4 values, 0..3

Access values as `Enum.GarrTalentUI.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Generic` | `GarrTalentUI` | = 0 |
| `CovenantSanctum` | `GarrTalentUI` | = 1 |
| `SoulBinds` | `GarrTalentUI` | = 2 |
| `AnimaDiversionMap` | `GarrTalentUI` | = 3 |

### GarrisonTalentAvailability

*Enumeration* · 9 values, 0..8

Access values as `Enum.GarrisonTalentAvailability.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `GarrisonTalentAvailability` | = 0 |
| `Unavailable` | `GarrisonTalentAvailability` | = 1 |
| `UnavailableAnotherIsResearching` | `GarrisonTalentAvailability` | = 2 |
| `UnavailableNotEnoughResources` | `GarrisonTalentAvailability` | = 3 |
| `UnavailableNotEnoughGold` | `GarrisonTalentAvailability` | = 4 |
| `UnavailableTierUnavailable` | `GarrisonTalentAvailability` | = 5 |
| `UnavailablePlayerCondition` | `GarrisonTalentAvailability` | = 6 |
| `UnavailableAlreadyHave` | `GarrisonTalentAvailability` | = 7 |
| `UnavailableRequiresPrerequisiteTalent` | `GarrisonTalentAvailability` | = 8 |
