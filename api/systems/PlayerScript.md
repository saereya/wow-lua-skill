# PlayerScript

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playerscriptdocumentation.lua` (FileDataID 5524528)

## Functions

### AcceptAreaSpiritHeal

```lua
AcceptAreaSpiritHeal()
```

### AcceptGuild

```lua
AcceptGuild()
```

### AcceptResurrect

```lua
AcceptResurrect()
```

### Ambiguate

```lua
Ambiguate(fullName: cstring, context: cstring) -> result: string
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `fullName` | `cstring` |  |
| `context` | `cstring` | `NeverSecret` |

### AutoEquipCursorItem

```lua
AutoEquipCursorItem()
```

### BeginTrade

```lua
BeginTrade()
```

### CancelAreaSpiritHeal

```lua
CancelAreaSpiritHeal()
```

### CancelPendingEquip

```lua
CancelPendingEquip(index: number)
```

`SecretArguments=AllowedWhenUntainted`

### CancelTrade

```lua
CancelTrade()
```

### CanDualWield

```lua
CanDualWield() -> result: bool
```

### CanInspect

```lua
CanInspect(targetGUID: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanLootUnit

```lua
CanLootUnit(targetUnit: WOWGUID) -> hasLoot: bool, canLoot: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### CanPortGraveyard

```lua
CanPortGraveyard() -> canPortGraveyard: bool
```

### CheckInteractDistance

```lua
CheckInteractDistance(unitGUID: UnitToken, distIndex: luaIndex) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### CheckTalentMasterDist

```lua
CheckTalentMasterDist() -> result: bool
```

### ClearPendingBindConversionItem

```lua
ClearPendingBindConversionItem()
```

### ConfirmTalentWipe

```lua
ConfirmTalentWipe()
```

### ConvertItemToBindToAccount

```lua
ConvertItemToBindToAccount()
```

### DeclineGuild

```lua
DeclineGuild()
```

### DeclineResurrect

```lua
DeclineResurrect()
```

### Dismount

```lua
Dismount()
```

### EquipPendingItem

```lua
EquipPendingItem(index: number)
```

`SecretArguments=AllowedWhenUntainted`

### FollowUnit

```lua
FollowUnit(name: cstring, exactMatch: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `"0"` |
| `exactMatch` | `bool` | default `false` |

### GetAllowLowLevelRaid

```lua
GetAllowLowLevelRaid() -> result: bool
```

### GetAllowRecentAlliesSeeLocation

```lua
GetAllowRecentAlliesSeeLocation() -> allowRecentAlliesSeeLocation: bool
```

### GetAreaSpiritHealerTime

```lua
GetAreaSpiritHealerTime() -> result: number
```

### GetArmorPenetration

```lua
GetArmorPenetration() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetAttackPowerForStat

```lua
GetAttackPowerForStat(stat: luaIndex, value: number) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetAutoDeclineGuildInvites

```lua
GetAutoDeclineGuildInvites() -> result: bool
```

### GetAutoDeclineNeighborhoodInvites

```lua
GetAutoDeclineNeighborhoodInvites() -> result: bool
```

### GetAvoidance

```lua
GetAvoidance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetBindLocation

```lua
GetBindLocation() -> result: cstring
```

### GetBlockChance

```lua
GetBlockChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetCemeteryPreference

```lua
GetCemeteryPreference() -> result: number
```

### GetCollapsingStarCost

```lua
GetCollapsingStarCost() -> cost: number
```

### GetCombatRating

```lua
GetCombatRating(ratingIndex: luaIndex) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetCombatRatingBonus

```lua
GetCombatRatingBonus(ratingIndex: luaIndex) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetCombatRatingBonusForCombatRatingValue

```lua
GetCombatRatingBonusForCombatRatingValue(ratingIndex: luaIndex, value: number) -> result: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetCorpseRecoveryDelay

```lua
GetCorpseRecoveryDelay() -> result: number
```

### GetCorruption

```lua
GetCorruption() -> result: number
```

### GetCorruptionResistance

```lua
GetCorruptionResistance() -> result: number
```

### GetCritChance

```lua
GetCritChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetCritChanceFromStat

```lua
GetCritChanceFromStat(stat: luaIndex, value: number) -> critChance: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetCritChanceProvidesParryEffect

```lua
GetCritChanceProvidesParryEffect() -> result: bool
```

### GetDodgeChance

```lua
GetDodgeChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetDodgeChanceFromAttribute

```lua
GetDodgeChanceFromAttribute() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetEvictionTimeRemaining

```lua
GetEvictionTimeRemaining() -> result: number
```

### GetExpertise

```lua
GetExpertise() -> mainhandExpertise: number, offhandExpertise: number, rangedExpertise: number
```

`SecretWhenUnitStatsRestricted`

### GetExpertisePercent

```lua
GetExpertisePercent() -> mainhandExpertisePercent: number, offhandExpertisePercent: number, rangedExpertisePercent: number
```

`SecretWhenUnitStatsRestricted`

### GetGlancingBlowChance

```lua
GetGlancingBlowChance(playerWeaponSkill: number?, targetDefenseSkill: number) -> result: number
```

If no playerWeaponSkill value is provided, uses the skill value for the player's main hand weapon/shapeshift form.

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetGlancingBlowPenalty

```lua
GetGlancingBlowPenalty(playerWeaponSkill: number?, targetDefenseSkill: number) -> result: number
```

If no playerWeaponSkill value is provided, uses the skill value for the player's main hand weapon/shapeshift form.

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetHaste

```lua
GetHaste() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetHealthRegen

```lua
GetHealthRegen() -> healthRegen: number, combatHealthRegen: number
```

### GetHealthRegenFromSpirit

```lua
GetHealthRegenFromSpirit() -> healthRegen: number, combatHealthRegen: number
```

### GetHitModifier

```lua
GetHitModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetJailersTowerLevel

```lua
GetJailersTowerLevel() -> result: number
```

### GetLifesteal

```lua
GetLifesteal() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetLootSpecialization

```lua
GetLootSpecialization() -> specializationID: number
```

### GetManaRegen

```lua
GetManaRegen() -> baseManaRegen: number, castingManaRegen: number
```

`SecretWhenUnitStatsRestricted`

### GetManaRegenFromSpirit

```lua
GetManaRegenFromSpirit() -> powerRegen: number, combatPowerRegen: number
```

### GetMastery

```lua
GetMastery() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetMasteryEffect

```lua
GetMasteryEffect() -> masteryEffect: number, bonusCoefficient: number
```

`SecretWhenUnitStatsRestricted`

### GetMaxPlayerLevel

```lua
GetMaxPlayerLevel() -> maxPlayerLevel: number
```

### GetMeleeHaste

```lua
GetMeleeHaste() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetModResilienceDamageReduction

```lua
GetModResilienceDamageReduction() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetMoney

```lua
GetMoney() -> result: number
```

### GetNormalizedRealmName

```lua
GetNormalizedRealmName() -> result: cstring
```

### GetOffhandHitModifier

```lua
GetOffhandHitModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetOverrideAPBySpellPower

```lua
GetOverrideAPBySpellPower() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetOverrideSpellPowerByAP

```lua
GetOverrideSpellPowerByAP() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetParryChance

```lua
GetParryChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetParryChanceFromAttribute

```lua
GetParryChanceFromAttribute() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPetCritChance

```lua
GetPetCritChance() -> meleeCrit: number, spellCrit: number
```

`SecretWhenUnitStatsRestricted`

### GetPetDodgeChance

```lua
GetPetDodgeChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPetHitChanceModifier

```lua
GetPetHitChanceModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPetMeleeHaste

```lua
GetPetMeleeHaste() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPetSpellBonusDamage

```lua
GetPetSpellBonusDamage() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPetSpellHitChanceModifier

```lua
GetPetSpellHitChanceModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPlayerFacing

```lua
GetPlayerFacing() -> result: number?
```

### GetPlayerInfoByGUID

```lua
GetPlayerInfoByGUID(guid: WOWGUID) -> localizedClass: cstring, englishClass: cstring, localizedRace: cstring, englishRace: cstring, sex: number, name: string, realmName: cstring, level: number?
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

### GetPowerRegen

```lua
GetPowerRegen() -> basePowerRegen: number, castingPowerRegen: number
```

`SecretWhenUnitStatsRestricted`

### GetPowerRegenForPowerType

```lua
GetPowerRegenForPowerType(powerType: number) -> basePowerRegen: number, castingPowerRegen: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetPVPDesired

```lua
GetPVPDesired() -> result: bool
```

### GetPVPGearStatRules

```lua
GetPVPGearStatRules() -> result: bool
```

### GetPVPLifetimeStats

```lua
GetPVPLifetimeStats() -> lifetimeHonorableKills: number, lifetimeMaxPVPRank: PvPRanks
```

### GetPvpPowerDamage

```lua
GetPvpPowerDamage() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPvpPowerHealing

```lua
GetPvpPowerHealing() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetPVPSessionStats

```lua
GetPVPSessionStats() -> honorableKills: number, dishonorableKills: number
```

### GetPVPTimer

```lua
GetPVPTimer() -> result: number
```

### GetPVPYesterdayStats

```lua
GetPVPYesterdayStats() -> honorableKills: number, dishonorableKills: number
```

### GetRangedAttackPowerForStat

```lua
GetRangedAttackPowerForStat(stat: luaIndex, value: number) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetRangedCritChance

```lua
GetRangedCritChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetRangedHaste

```lua
GetRangedHaste() -> result: number, quiverHaste: number
```

`SecretWhenUnitStatsRestricted`

### GetRangedHitModifier

```lua
GetRangedHitModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetReleaseTimeRemaining

```lua
GetReleaseTimeRemaining() -> result: number
```

### GetResSicknessDuration

```lua
GetResSicknessDuration() -> result: string?
```

### GetRestrictedAccountData

```lua
GetRestrictedAccountData() -> maxLevel: number, maxMoney: WOWMONEY, professionCap: number
```

### GetRestState

```lua
GetRestState() -> exhaustionID: number, name: cstring, factor: number
```

`MayReturnNothing`

### GetRuneCooldown

```lua
GetRuneCooldown(runeIndex: luaIndex) -> startTime: number, duration: number, isRuneReady: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRuneCount

```lua
GetRuneCount(runeIndex: luaIndex) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSheathState

```lua
GetSheathState() -> result: number?
```

### GetShieldBlock

```lua
GetShieldBlock() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSpeed

```lua
GetSpeed() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSpellBonusDamage

```lua
GetSpellBonusDamage(school: luaIndex) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetSpellBonusHealing

```lua
GetSpellBonusHealing() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSpellCritChance

```lua
GetSpellCritChance() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSpellCritChanceFromStat

```lua
GetSpellCritChanceFromStat(stat: luaIndex, value: number) -> spellCritChance: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetSpellHitModifier

```lua
GetSpellHitModifier() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSpellPenetration

```lua
GetSpellPenetration() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetSturdiness

```lua
GetSturdiness() -> result: number
```

`SecretWhenUnitStatsRestricted`

### GetTaxiBenchmarkMode

```lua
GetTaxiBenchmarkMode() -> result: bool
```

### GetVersatilityBonus

```lua
GetVersatilityBonus(combatRating: luaIndex) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetXPExhaustion

```lua
GetXPExhaustion() -> result: number?
```

### HasAPEffectsSpellPower

```lua
HasAPEffectsSpellPower() -> result: bool
```

### HasDualWieldPenalty

```lua
HasDualWieldPenalty() -> result: bool
```

### HasFullControl

```lua
HasFullControl() -> result: bool
```

### HasIgnoreDualWieldWeapon

```lua
HasIgnoreDualWieldWeapon() -> result: bool
```

### HasKey

```lua
HasKey() -> hasKey: bool
```

### HasNoReleaseAura

```lua
HasNoReleaseAura() -> hasCannotReleaseEffect: bool, longestDuration: number, hasUntilCancelledDuration: bool
```

### HasSPEffectsAttackPower

```lua
HasSPEffectsAttackPower() -> result: bool
```

### InitiateTrade

```lua
InitiateTrade(guid: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### IsAccountSecured

```lua
IsAccountSecured() -> result: bool
```

### IsAdvancedFlyableArea

```lua
IsAdvancedFlyableArea() -> result: bool
```

### IsCemeterySelectionAvailable

```lua
IsCemeterySelectionAvailable() -> result: bool
```

### IsCharacterNewlyBoosted

```lua
IsCharacterNewlyBoosted() -> newlyBoosted: bool
```

### IsDrivableArea

```lua
IsDrivableArea() -> result: bool
```

### IsDualWielding

```lua
IsDualWielding() -> result: bool
```

### IsFlyableArea

```lua
IsFlyableArea() -> result: bool
```

### IsGuildLeader

```lua
IsGuildLeader() -> result: bool
```

### IsIndoors

```lua
IsIndoors() -> result: bool
```

### IsInGuild

```lua
IsInGuild() -> result: bool
```

### IsInJailersTower

```lua
IsInJailersTower() -> result: bool
```

### IsInsane

```lua
IsInsane() -> result: bool
```

### IsItemPreferredArmorType

```lua
IsItemPreferredArmorType(itemLocation: ItemLocation) -> isItemPreferredArmorType: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsJailersTowerLayerTimeLocked

```lua
IsJailersTowerLayerTimeLocked(layerLevel: number) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### IsLoggedIn

```lua
IsLoggedIn() -> result: bool
```

### IsMounted

```lua
IsMounted() -> result: bool
```

### IsOnGroundFloorInJailersTower

```lua
IsOnGroundFloorInJailersTower() -> result: bool
```

### IsOutdoors

```lua
IsOutdoors() -> result: bool
```

### IsOutOfBounds

```lua
IsOutOfBounds() -> result: bool
```

### IsPlayerInWorld

```lua
IsPlayerInWorld() -> result: bool
```

### IsPlayerMoving

```lua
IsPlayerMoving() -> result: bool
```

### IsPVPTimerRunning

```lua
IsPVPTimerRunning() -> result: bool
```

### IsRangedWeapon

```lua
IsRangedWeapon() -> result: bool
```

### IsResting

```lua
IsResting() -> result: bool
```

### IsRestrictedAccount

```lua
IsRestrictedAccount() -> result: bool
```

### IsStealthed

```lua
IsStealthed() -> result: bool
```

### IsXPUserDisabled

```lua
IsXPUserDisabled() -> result: bool
```

### NoPlayTime

```lua
NoPlayTime() -> result: bool?
```

### NotifyInspect

```lua
NotifyInspect(targetGUID: UnitToken)
```

`SecretArguments=AllowedWhenUntainted`

### PartialPlayTime

```lua
PartialPlayTime() -> result: bool?
```

### PlayerCanTeleport

```lua
PlayerCanTeleport() -> result: bool
```

### PlayerEffectiveAttackPower

```lua
PlayerEffectiveAttackPower() -> mainHandAttackPower: number, offHandAttackPower: number, rangedAttackPower: number, baseAttackPower: number, baseRangedAttackPower: number
```

`MayReturnNothing` `SecretWhenUnitStatsRestricted`

### PlayerGetTimerunningSeasonID

```lua
PlayerGetTimerunningSeasonID() -> timerunningSeasonID: number?
```

### PlayerIsInCombat

```lua
PlayerIsInCombat() -> playerIsInCombat: bool
```

### PlayerIsTimerunning

```lua
PlayerIsTimerunning() -> playerIsTimerunning: bool
```

### PortGraveyard

```lua
PortGraveyard()
```

### RandomRoll

```lua
RandomRoll(min: number, max: number)
```

`SecretArguments=AllowedWhenUntainted`

### ReagentsFromBankAllowed

```lua
ReagentsFromBankAllowed() -> allowed: bool
```

### RepopMe

```lua
RepopMe()
```

### RequestTimePlayed

```lua
RequestTimePlayed()
```

### RespondInstanceLock

```lua
RespondInstanceLock(acceptLock: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ResurrectGetOfferer

```lua
ResurrectGetOfferer() -> name: cstring
```

### ResurrectHasSickness

```lua
ResurrectHasSickness() -> result: bool
```

### ResurrectHasTimer

```lua
ResurrectHasTimer() -> result: bool
```

### RetrieveCorpse

```lua
RetrieveCorpse()
```

### SetAllowLowLevelRaid

```lua
SetAllowLowLevelRaid(allow: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `allow` | `bool` | default `false` |

### SetAllowRecentAlliesSeeLocation

```lua
SetAllowRecentAlliesSeeLocation(allowRecentAlliesSeeLocation: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAutoDeclineGuildInvites

```lua
SetAutoDeclineGuildInvites(allow: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `allow` | `bool` | default `false` |

### SetAutoDeclineNeighborhoodInvites

```lua
SetAutoDeclineNeighborhoodInvites(allow: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `allow` | `bool` | default `false` |

### SetCemeteryPreference

```lua
SetCemeteryPreference(cemetaryID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetLootSpecialization

```lua
SetLootSpecialization(specializationID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTaxiBenchmarkMode

```lua
SetTaxiBenchmarkMode(enable: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### ShouldDisplayRaidRolesInSocialFrame

```lua
ShouldDisplayRaidRolesInSocialFrame() -> result: bool
```

### ShouldDisplayStoryModeTooltipInSocialFrame

```lua
ShouldDisplayStoryModeTooltipInSocialFrame() -> result: bool
```

### ShouldShowIslandsWeeklyPOI

```lua
ShouldShowIslandsWeeklyPOI() -> result: bool
```

### ShouldShowSpecialSplashScreen

```lua
ShouldShowSpecialSplashScreen() -> result: bool
```

### ShowCloak

```lua
ShowCloak(show: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShowHelm

```lua
ShowHelm(show: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShowingCloak

```lua
ShowingCloak() -> result: bool
```

### ShowingHelm

```lua
ShowingHelm() -> result: bool
```

### SitStandOrDescendStart

```lua
SitStandOrDescendStart()
```

`HasRestrictions`

### SplashFrameCanBeShown

```lua
SplashFrameCanBeShown() -> result: bool
```

### StartAttack

```lua
StartAttack(name: cstring, exactMatch: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `"0"` |
| `exactMatch` | `bool` | default `false` |

### StopAttack

```lua
StopAttack()
```

### Stuck

```lua
Stuck()
```

### TimeoutResurrect

```lua
TimeoutResurrect()
```

### ToggleSelfHighlight

```lua
ToggleSelfHighlight() -> enabled: bool
```

### ToggleSheath

```lua
ToggleSheath()
```

### ToggleSit

```lua
ToggleSit()
```

`HasRestrictions`

## Events

### PLAYER_IN_COMBAT_CHANGED

```lua
PLAYER_IN_COMBAT_CHANGED(inCombat: bool)
```

`SynchronousEvent`

### PLAYER_TARGET_DIED

```lua
PLAYER_TARGET_DIED()
```

`SynchronousEvent`

## Types

### PlayerAttackPowerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mainHandAttackPower` | `number` |  |
| `offHandAttackPower` | `number` |  |
| `rangedAttackPower` | `number` |  |
| `baseAttackPower` | `number` |  |
| `baseRangedAttackPower` | `number` |  |
