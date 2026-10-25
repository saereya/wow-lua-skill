# Unit

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/unitdocumentation.lua` (FileDataID 4637296)

## Functions

### CanEjectPassengerFromSeat

```lua
CanEjectPassengerFromSeat(virtualSeatIndex: luaIndex) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanSwitchVehicleSeat

```lua
CanSwitchVehicleSeat() -> result: bool
```

### ClosestGameObjectPosition

```lua
ClosestGameObjectPosition(gameObjectID: number) -> xPos: number, yPos: number, distance: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretReturns`

### ClosestUnitPosition

```lua
ClosestUnitPosition(creatureID: number) -> xPos: number, yPos: number, distance: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretReturns`

### CreateUnitHealPredictionCalculator

```lua
CreateUnitHealPredictionCalculator() -> healPredictionCalculator: UnitHealPredictionCalculator
```

### EjectPassengerFromSeat

```lua
EjectPassengerFromSeat(virtualSeatIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetComboPoints

```lua
GetComboPoints(unit: UnitTokenPvPRestrictedForAddOns, target: UnitTokenPvPRestrictedForAddOns) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerRestricted`

### GetNegativeCorruptionEffectInfo

```lua
GetNegativeCorruptionEffectInfo() -> corruptionEffects: CorruptionEffectInfo[]
```

### GetUnitChargedPowerPoints

```lua
GetUnitChargedPowerPoints(unit: UnitToken) -> pointIndices: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitPowerRestricted`

### GetUnitEmpowerHoldAtMaxTime

```lua
GetUnitEmpowerHoldAtMaxTime(unit: UnitToken) -> holdAtMaxTime: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitSpellCastRestricted`

### GetUnitEmpowerMinHoldTime

```lua
GetUnitEmpowerMinHoldTime(unit: UnitToken) -> minHoldTime: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitSpellCastRestricted`

### GetUnitEmpowerStageDuration

```lua
GetUnitEmpowerStageDuration(unit: UnitToken, index: number) -> duration: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitSpellCastRestricted`

### GetUnitHealthModifier

```lua
GetUnitHealthModifier(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitMaxHealthModifier

```lua
GetUnitMaxHealthModifier(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitPowerBarInfo

```lua
GetUnitPowerBarInfo(unitToken: UnitToken) -> info: UnitPowerBarInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUnitPowerBarInfoByID

```lua
GetUnitPowerBarInfoByID(barID: number) -> info: UnitPowerBarInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUnitPowerBarStrings

```lua
GetUnitPowerBarStrings(unitToken: UnitToken) -> name: cstring?, tooltip: cstring?, cost: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitPowerBarStringsByID

```lua
GetUnitPowerBarStringsByID(barID: number) -> name: cstring?, tooltip: cstring?, cost: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitPowerBarTextureInfo

```lua
GetUnitPowerBarTextureInfo(unitToken: UnitToken, textureIndex: luaIndex, timerIndex: luaIndex?) -> texture: fileID, colorR: number, colorG: number, colorB: number, colorA: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitPowerBarTextureInfoByID

```lua
GetUnitPowerBarTextureInfoByID(barID: number, textureIndex: luaIndex) -> texture: fileID, colorR: number, colorG: number, colorB: number, colorA: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitPowerModifier

```lua
GetUnitPowerModifier(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnitSpeed

```lua
GetUnitSpeed(unit: UnitToken) -> currentSpeed: number, runSpeed: number, flightSpeed: number, swimSpeed: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### GetUnitTotalModifiedMaxHealthPercent

```lua
GetUnitTotalModifiedMaxHealthPercent(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetVehicleUIIndicator

```lua
GetVehicleUIIndicator(vehicleIndicatorID: number) -> backgroundTextureID: fileID, numSeatIndicators: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetVehicleUIIndicatorSeat

```lua
GetVehicleUIIndicatorSeat(vehicleIndicatorID: number, indicatorSeatIndex: luaIndex) -> virtualSeatIndex: number, xPos: number, yPos: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### IsFalling

```lua
IsFalling(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFlying

```lua
IsFlying(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPlayerInGuildFromGUID

```lua
IsPlayerInGuildFromGUID(playerGUID: WOWGUID) -> IsInGuild: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSubmerged

```lua
IsSubmerged(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSwimming

```lua
IsSwimming(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUnitModelReadyForUI

```lua
IsUnitModelReadyForUI(unitToken: UnitToken) -> isReady: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerIsPVPInactive

```lua
PlayerIsPVPInactive(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerIsSpellTarget

```lua
PlayerIsSpellTarget(unit: UnitToken) -> result: bool
```

If the unit is currently casting a spell, returns whether spell's target unit is the player. Returns false if the unit is not casting a spell or the spell has no target.

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### PlayerVehicleHasComboPoints

```lua
PlayerVehicleHasComboPoints() -> vehicleHasComboPoints: bool
```

### RegionalUniqueNamesEnabled

```lua
RegionalUniqueNamesEnabled() -> result: bool
```

### ReportPlayerIsPVPAFK

```lua
ReportPlayerIsPVPAFK(unit: UnitToken)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ResistancePercent

```lua
ResistancePercent(resistance: number, casterLevel: number) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### SetPortraitTexture

```lua
SetPortraitTexture(textureObject: SimpleTexture, unitToken: UnitToken, disableMasking: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `textureObject` | `SimpleTexture` |  |
| `unitToken` | `UnitToken` |  |
| `disableMasking` | `bool` | default `false` |

### SetPortraitTextureFromCreatureDisplayID

```lua
SetPortraitTextureFromCreatureDisplayID(textureObject: SimpleTexture, creatureDisplayID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetUnitCursorTexture

```lua
SetUnitCursorTexture(textureObject: SimpleTexture, unit: UnitToken, style: CursorStyle?, includeLowPriority: bool?, preferGamepadIcon: bool?) -> hasCursor: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitAffectingCombat

```lua
UnitAffectingCombat(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitAlliedRaceInfo

```lua
UnitAlliedRaceInfo(unit: UnitToken) -> isAlliedRace: bool, hasHeritageArmorUnlocked: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitArmor

```lua
UnitArmor(unit: UnitToken) -> base: number, effective: number, real: number, bonus: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitAttackPower

```lua
UnitAttackPower(unit: UnitToken) -> attackPower: number, posBuff: number, negBuff: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitAttackSpeed

```lua
UnitAttackSpeed(unit: UnitToken) -> attackSpeed: number, offhandAttackSpeed: number?, rangedAttackSpeed: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitBattlePetLevel

```lua
UnitBattlePetLevel(unit: UnitToken) -> result: number?
```

`SecretArguments=AllowedWhenUntainted`

### UnitBattlePetSpeciesID

```lua
UnitBattlePetSpeciesID(unit: UnitToken) -> result: number?
```

`SecretArguments=AllowedWhenUntainted`

### UnitBattlePetType

```lua
UnitBattlePetType(unit: UnitToken) -> result: number?
```

`SecretArguments=AllowedWhenUntainted`

### UnitCanAssist

```lua
UnitCanAssist(unit: UnitToken, target: UnitToken, canAssistImmunePC: bool, canAssistUninteractable: bool) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `target` | `UnitToken` |  |
| `canAssistImmunePC` | `bool` | default `false` |
| `canAssistUninteractable` | `bool` | default `false` |

### UnitCanAttack

```lua
UnitCanAttack(unit: UnitToken, target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitCanCooperate

```lua
UnitCanCooperate(unit: UnitToken, target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitCanPetBattle

```lua
UnitCanPetBattle(unit: UnitToken, target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitCastingDuration

```lua
UnitCastingDuration(unit: UnitTokenPvPRestrictedForAddOns) -> duration: LuaDurationObject
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretReturns`

### UnitCastingInfo

```lua
UnitCastingInfo(unit: UnitTokenPvPRestrictedForAddOns) -> name: cstring, displayName: string, textureID: fileID, startTimeMs: number, endTimeMs: number, isTradeskill: bool, castID: WOWGUID, notInterruptible: bool?, castingSpellID: number, castBarID: UnitCastBarID?, delayTimeMs: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitSpellCastRestricted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayName` | `string` |  |
| `textureID` | `fileID` |  |
| `startTimeMs` | `number` |  |
| `endTimeMs` | `number` |  |
| `isTradeskill` | `bool` | `NeverSecret` |
| `castID` | `WOWGUID` |  |
| `notInterruptible` | `bool?` |  |
| `castingSpellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |
| `delayTimeMs` | `number` | `NeverSecret` |

### UnitChannelDuration

```lua
UnitChannelDuration(unit: UnitTokenPvPRestrictedForAddOns) -> duration: LuaDurationObject
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### UnitChannelInfo

```lua
UnitChannelInfo(unit: UnitTokenPvPRestrictedForAddOns) -> name: cstring, displayName: cstring, textureID: fileID, startTimeMs: number, endTimeMs: number, isTradeskill: bool, notInterruptible: bool?, spellID: number, isEmpowered: bool, numEmpowerStages: number, castBarID: UnitCastBarID?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitSpellCastRestricted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayName` | `cstring` |  |
| `textureID` | `fileID` |  |
| `startTimeMs` | `number` |  |
| `endTimeMs` | `number` |  |
| `isTradeskill` | `bool` | `NeverSecret` |
| `notInterruptible` | `bool?` |  |
| `spellID` | `number` |  |
| `isEmpowered` | `bool` | `NeverSecret` |
| `numEmpowerStages` | `number` | `NeverSecret` |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UnitChromieTimeID

```lua
UnitChromieTimeID(unit: UnitToken) -> ID: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitClass

```lua
UnitClass(unit: UnitToken) -> className: cstring, classFilename: cstring, classID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitIdentityRestricted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `className` | `cstring` | `ConditionalSecret` |
| `classFilename` | `cstring` |  |
| `classID` | `number` |  |

### UnitClassBase

```lua
UnitClassBase(unit: UnitToken) -> classFilename: cstring, classID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitIdentityRestricted`

### UnitClassFromGUID

```lua
UnitClassFromGUID(unitGUID: WOWGUID) -> className: cstring, classFilename: cstring, classID: number
```

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `className` | `cstring` | `ConditionalSecret` |
| `classFilename` | `cstring` |  |
| `classID` | `number` |  |

### UnitClassification

```lua
UnitClassification(unit: UnitToken) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

### UnitControllingVehicle

```lua
UnitControllingVehicle(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitCreatureFamily

```lua
UnitCreatureFamily(unit: UnitToken) -> name: cstring, id: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitCreatureID

```lua
UnitCreatureID(unit: UnitToken) -> creatureID: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted` `RequiresUnitIdentityAccess`

### UnitCreatureType

```lua
UnitCreatureType(unit: UnitToken) -> name: cstring, id: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitDamage

```lua
UnitDamage(unit: UnitToken) -> minDamage: number, maxDamage: number, offhandMinDamage: number, offhandMaxDamage: number, posBuff: number, negBuff: number, percent: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitDefenseSkill

```lua
UnitDefenseSkill(unit: UnitToken) -> base: number, modifier: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitDetailedThreatSituation

```lua
UnitDetailedThreatSituation(unit: UnitToken, mobGUID: UnitToken) -> isTanking: bool, status: number, scaledPercentage: number, rawPercentage: number, rawThreat: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitThreatValuesRestricted`

### UnitDistanceSquared

```lua
UnitDistanceSquared(unit: UnitToken) -> distance: number, checkedDistance: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitEffectiveLevel

```lua
UnitEffectiveLevel(name: cstring) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitEmpoweredChannelDuration

```lua
UnitEmpoweredChannelDuration(unit: UnitToken, includeHoldAtMaxTime: bool) -> duration: LuaDurationObject
```

Returns a duration object that includes the duration of an empowered cast channel.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `includeHoldAtMaxTime` | `bool` | default `true`; If true, include the hold-at-max time of the empowered channel in the total duration. |

### UnitEmpoweredStageDurations

```lua
UnitEmpoweredStageDurations(unit: UnitToken) -> duration: LuaDurationObject[]
```

Returns a vector of duration objects that measure the time spans for each individual stage in an empowered channel, with hold-at-max time included as the last element.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### UnitEmpoweredStagePercentages

```lua
UnitEmpoweredStagePercentages(unit: UnitToken, includeHoldAtMaxTime: bool) -> percentages: number[]
```

Returns a vector of percentages that describe how much of the total duration of an empowered channel is occupied by a stage.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `includeHoldAtMaxTime` | `bool` | default `true`; If true, include the hold-at-max time of the empowered channel in the total duration and add a percentage value for it. |

### UnitExists

```lua
UnitExists(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitFactionGroup

```lua
UnitFactionGroup(unitName: cstring, checkDisplayRace: bool) -> factionGroupTag: cstring, localized: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitName` | `cstring` |  |
| `checkDisplayRace` | `bool` | default `false` |

### UnitFullName

```lua
UnitFullName(unit: UnitToken) -> unitName: cstring, unitServer: cstring
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitGetDetailedHealPrediction

```lua
UnitGetDetailedHealPrediction(unit: UnitTokenPvPRestrictedForAddOns, healerUnit: UnitTokenPvPRestrictedForAddOns?, healPredictionCalculator: UnitHealPredictionCalculator)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenPvPRestrictedForAddOns` |  |
| `healerUnit` | `UnitTokenPvPRestrictedForAddOns?` | If specified, a unit to evaluate as the 'healer' for incoming heal values. If nil, healer values will be zero. |
| `healPredictionCalculator` | `UnitHealPredictionCalculator` |  |

### UnitGetIncomingHeals

```lua
UnitGetIncomingHeals(unit: UnitTokenPvPRestrictedForAddOns, healerGUID: UnitTokenPvPRestrictedForAddOns?) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### UnitGetTotalAbsorbs

```lua
UnitGetTotalAbsorbs(unit: UnitTokenPvPRestrictedForAddOns) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### UnitGetTotalHealAbsorbs

```lua
UnitGetTotalHealAbsorbs(unit: UnitTokenPvPRestrictedForAddOns) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### UnitGroupRolesAssigned

```lua
UnitGroupRolesAssigned(unit: UnitToken?) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitGroupRolesAssignedEnum

```lua
UnitGroupRolesAssignedEnum(unit: UnitToken?) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitGUID

```lua
UnitGUID(unit: UnitTokenPvPRestrictedForAddOns) -> result: WOWGUID?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitHasEffectivelyTankAura

```lua
UnitHasEffectivelyTankAura(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitHasLootInteraction

```lua
UnitHasLootInteraction(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHasMouseoverHighlight

```lua
UnitHasMouseoverHighlight(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHasPowerType

```lua
UnitHasPowerType(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType) -> hasPower: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHasRelicSlot

```lua
UnitHasRelicSlot(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHasVehiclePlayerFrameUI

```lua
UnitHasVehiclePlayerFrameUI(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHasVehicleUI

```lua
UnitHasVehicleUI(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitHealth

```lua
UnitHealth(unit: UnitTokenPvPRestrictedForAddOns, usePredicted: bool) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenPvPRestrictedForAddOns` |  |
| `usePredicted` | `bool` | default `true` |

### UnitHealthMax

```lua
UnitHealthMax(unit: UnitTokenPvPRestrictedForAddOns) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitHealthMaxRestricted`

### UnitHealthMissing

```lua
UnitHealthMissing(unit: UnitTokenPvPRestrictedForAddOns, usePredicted: bool) -> result: number
```

Result of UnitHealthMax() - UnitHealth()

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenPvPRestrictedForAddOns` |  |
| `usePredicted` | `bool` | default `true` |

### UnitHealthPercent

```lua
UnitHealthPercent(unit: UnitTokenPvPRestrictedForAddOns, usePredicted: bool, curve: LuaCurveObjectBase?) -> result: LuaCurveEvaluatedResult
```

Returns percent of health remaining - can be scaled via a curve for display purposes

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret` `SecretReturns`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenPvPRestrictedForAddOns` |  |
| `usePredicted` | `bool` | default `true` |
| `curve` | `LuaCurveObjectBase?` |  |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `LuaCurveEvaluatedResult` | If no curve is specified, a floating point percentage value. Else, the result of evaluating the curve with the percentage as the input. |

### UnitHonor

```lua
UnitHonor(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitHonorLevel

```lua
UnitHonorLevel(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitHonorMax

```lua
UnitHonorMax(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitHPPerStamina

```lua
UnitHPPerStamina(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitInAnyGroup

```lua
UnitInAnyGroup(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInBattleground

```lua
UnitInBattleground(unit: UnitToken?, partyIndex: luaIndex?) -> result: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### UnitInOtherParty

```lua
UnitInOtherParty(unit: UnitToken) -> inOtherParty: bool
```

Checks whether this unit cannot see your party chat because it is in an instance group

`SecretArguments=AllowedWhenUntainted`

### UnitInParty

```lua
UnitInParty(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInPartyIsAI

```lua
UnitInPartyIsAI(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInPartyShard

```lua
UnitInPartyShard(unit: UnitToken) -> inPartyShard: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInRaid

```lua
UnitInRaid(unit: UnitToken?, partyIndex: luaIndex?) -> result: luaIndex?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitInRange

```lua
UnitInRange(unit: UnitToken) -> inRange: bool, checkedRange: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### UnitInSubgroup

```lua
UnitInSubgroup(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInVehicle

```lua
UnitInVehicle(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInVehicleControlSeat

```lua
UnitInVehicleControlSeat(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitInVehicleHidesPetFrame

```lua
UnitInVehicleHidesPetFrame(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsAFK

```lua
UnitIsAFK(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### UnitIsBattlePet

```lua
UnitIsBattlePet(unit: UnitToken) -> result: bool?
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsBattlePetCompanion

```lua
UnitIsBattlePetCompanion(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsBossMob

```lua
UnitIsBossMob(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsCharmed

```lua
UnitIsCharmed(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPossessionRestricted`

### UnitIsConnected

```lua
UnitIsConnected(unit: UnitToken) -> isConnected: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsControlling

```lua
UnitIsControlling(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsCorpse

```lua
UnitIsCorpse(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsDead

```lua
UnitIsDead(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsDeadOrGhost

```lua
UnitIsDeadOrGhost(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsDND

```lua
UnitIsDND(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### UnitIsEnemy

```lua
UnitIsEnemy(unit: UnitToken, target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsFeignDeath

```lua
UnitIsFeignDeath(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsFriend

```lua
UnitIsFriend(unit: UnitToken, target: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsGameObject

```lua
UnitIsGameObject(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsGhost

```lua
UnitIsGhost(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsGroupAssistant

```lua
UnitIsGroupAssistant(unit: UnitToken) -> isAssistant: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitIsGroupLeader

```lua
UnitIsGroupLeader(unit: UnitToken, partyCategory: luaIndex?) -> isLeader: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitIsHumanPlayer

```lua
UnitIsHumanPlayer(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsInInteractRange

```lua
UnitIsInInteractRange(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsInMyGuild

```lua
UnitIsInMyGuild(unit: cstring) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsInteractable

```lua
UnitIsInteractable(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsLieutenant

```lua
UnitIsLieutenant(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsMercenary

```lua
UnitIsMercenary(name: cstring) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsMinion

```lua
UnitIsMinion(unit: UnitToken) -> result: bool
```

Returns whether the unit is considered a minion of a player, such as a pet, totem, or guardian.

`SecretArguments=AllowedWhenUntainted`

### UnitIsNPCAsPlayer

```lua
UnitIsNPCAsPlayer(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsOtherPlayersBattlePet

```lua
UnitIsOtherPlayersBattlePet(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsOtherPlayersPet

```lua
UnitIsOtherPlayersPet(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsOwnerOrControllerOfUnit

```lua
UnitIsOwnerOrControllerOfUnit(controllingUnit: UnitToken, controlledUnit: UnitToken) -> unitIsOwnerOrControllerOfUnit: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitIsPlayer

```lua
UnitIsPlayer(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsPlayerControlledOrGroupMember

```lua
UnitIsPlayerControlledOrGroupMember(unit: UnitToken) -> result: bool
```

Returns true for 'player', 'pet', 'vehicle', or any of 'partyn', 'partypetn', 'raidn', 'raidpetn'

`SecretArguments=AllowedWhenUntainted`

### UnitIsPossessed

```lua
UnitIsPossessed(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPossessionRestricted`

### UnitIsPVP

```lua
UnitIsPVP(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitIsPVPFreeForAll

```lua
UnitIsPVPFreeForAll(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsPVPSanctuary

```lua
UnitIsPVPSanctuary(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsQuestBoss

```lua
UnitIsQuestBoss(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsRaidOfficer

```lua
UnitIsRaidOfficer(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitIsSameServer

```lua
UnitIsSameServer(unitName: cstring) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsTapDenied

```lua
UnitIsTapDenied(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsTrivial

```lua
UnitIsTrivial(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsUnconscious

```lua
UnitIsUnconscious(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsUnit

```lua
UnitIsUnit(unit1: UnitToken, unit2: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresComparableUnitTokens` `SecretWhenUnitComparisonRestricted`

### UnitIsVisible

```lua
UnitIsVisible(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitIsWildBattlePet

```lua
UnitIsWildBattlePet(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitLeadsAnyGroup

```lua
UnitLeadsAnyGroup(unit: UnitToken) -> isLeader: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitLevel

```lua
UnitLevel(name: cstring) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitName

```lua
UnitName(unit: UnitToken) -> unitName: cstring, unitServer: cstring
```

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitNameIdentityRestricted`

### UnitNameFromGUID

```lua
UnitNameFromGUID(unitGUID: WOWGUID) -> unitName: cstring, unitServer: cstring
```

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitIdentityRestricted`

### UnitNameplateShowsWidgetsOnly

```lua
UnitNameplateShowsWidgetsOnly(unit: UnitToken) -> nameplateShowsWidgetsOnly: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitNameUnmodified

```lua
UnitNameUnmodified(unit: UnitToken) -> unitName: cstring, unitServer: cstring
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitNumPowerBarTimers

```lua
UnitNumPowerBarTimers(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitOnTaxi

```lua
UnitOnTaxi(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitOwnerGUID

```lua
UnitOwnerGUID(unit: UnitTokenPvPRestrictedForAddOns) -> ownerGUID: WOWGUID
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitPartialPower

```lua
UnitPartialPower(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType?, unmodified: bool) -> partialPower: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenPvPRestrictedForAddOns` |  |
| `powerType` | `PowerType?` |  |
| `unmodified` | `bool` | default `false` |

### UnitPercentHealthFromGUID

```lua
UnitPercentHealthFromGUID(unitGUID: WOWGUID) -> percentHealth: number?
```

`SecretArguments=AllowedWhenTainted` `SecretReturns`

### UnitPhaseReason

```lua
UnitPhaseReason(unit: UnitToken) -> reason: PhaseReason?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitPlayerControlled

```lua
UnitPlayerControlled(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitPlayerOrPetInParty

```lua
UnitPlayerOrPetInParty(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitPlayerOrPetInRaid

```lua
UnitPlayerOrPetInRaid(unit: UnitToken?, partyIndex: luaIndex?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitPosition

```lua
UnitPosition(unit: UnitToken) -> positionX: number, positionY: number, positionZ: number, mapID: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitPower

```lua
UnitPower(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType?, unmodified: bool) -> power: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenPvPRestrictedForAddOns` |  |
| `powerType` | `PowerType?` |  |
| `unmodified` | `bool` | default `false` |

### UnitPowerBarID

```lua
UnitPowerBarID(unitToken: UnitToken) -> barID: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitPowerBarTimerInfo

```lua
UnitPowerBarTimerInfo(unit: UnitToken, index: luaIndex) -> duration: number, expiration: number, barID: number, auraID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretReturns`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `index` | `luaIndex` | default `0` |

### UnitPowerDisplayMod

```lua
UnitPowerDisplayMod(powerType: PowerType) -> displayMod: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitPowerMax

```lua
UnitPowerMax(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType?, unmodified: bool) -> maxPower: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerMaxRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenPvPRestrictedForAddOns` |  |
| `powerType` | `PowerType?` |  |
| `unmodified` | `bool` | default `false` |

### UnitPowerMissing

```lua
UnitPowerMissing(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType?, unmodified: bool) -> result: number
```

Result of UnitPowerMax() - UnitPower()

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerRestricted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenPvPRestrictedForAddOns` |  |
| `powerType` | `PowerType?` |  |
| `unmodified` | `bool` | default `false` |

### UnitPowerPercent

```lua
UnitPowerPercent(unitToken: UnitTokenPvPRestrictedForAddOns, powerType: PowerType?, unmodified: bool, curve: LuaCurveObjectBase?) -> result: LuaCurveEvaluatedResult
```

Queries the percent of power remaining, optionally evaluating it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitPowerRestricted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenPvPRestrictedForAddOns` |  |
| `powerType` | `PowerType?` |  |
| `unmodified` | `bool` | default `false` |
| `curve` | `LuaCurveObjectBase?` |  |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `LuaCurveEvaluatedResult` | If no curve is specified, a floating point percentage value. Else, the result of evaluating the curve with the percentage as the input. |

### UnitPowerType

```lua
UnitPowerType(unit: UnitTokenPvPRestrictedForAddOns, index: number) -> powerType: PowerType, powerTypeToken: string, rgbX: number, rgbY: number, rgbZ: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitTokenPvPRestrictedForAddOns` |  |
| `index` | `number` | default `0` |

### UnitPvpClassification

```lua
UnitPvpClassification(unit: UnitTokenPvPRestrictedForAddOns) -> classification: PvPUnitClassification?
```

`SecretArguments=AllowedWhenUntainted`

### UnitPVPName

```lua
UnitPVPName(unit: UnitToken) -> result: string
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitQuestTrivialLevelRange

```lua
UnitQuestTrivialLevelRange(unit: UnitToken) -> levelRange: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitQuestTrivialLevelRangeScaling

```lua
UnitQuestTrivialLevelRangeScaling(unit: UnitToken) -> levelRange: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitRace

```lua
UnitRace(unit: UnitToken) -> localizedRaceName: cstring, englishRaceName: cstring, raceID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenUnitIdentityRestricted`

### UnitRangedAttackPower

```lua
UnitRangedAttackPower(unit: UnitToken) -> attackPower: number, posBuff: number, negBuff: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitRangedDamage

```lua
UnitRangedDamage(unit: UnitToken) -> speed: number, minDamage: number, maxDamage: number, posBuff: number, negBuff: number, percent: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitReaction

```lua
UnitReaction(unit: UnitToken, target: UnitToken) -> result: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### UnitRealmRelationship

```lua
UnitRealmRelationship(unit: UnitToken) -> realmRelationship: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### UnitResistance

```lua
UnitResistance(unit: UnitToken, damageClass: Damageclass) -> baseResistance: number, realResistance: number, effectiveResistance: number, bonusResistance: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitSelectionColor

```lua
UnitSelectionColor(unit: UnitToken, useExtendedColors: bool) -> resultR: number, resultG: number, resultB: number, resultA: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `useExtendedColors` | `bool` | default `false` |

### UnitSelectionType

```lua
UnitSelectionType(unit: UnitToken, useExtendedColors: bool) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `UnitToken` |  |
| `useExtendedColors` | `bool` | default `false` |

### UnitSex

```lua
UnitSex(unit: UnitToken) -> sex: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitSexBase

```lua
UnitSexBase(unit: UnitToken) -> sex: UnitSex?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitIdentityRestricted`

### UnitShouldDisplayName

```lua
UnitShouldDisplayName(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitShouldDisplaySpellTargetName

```lua
UnitShouldDisplaySpellTargetName(unit: UnitToken) -> result: bool
```

If the unit is currently casting a spell, returns whether the target's name should be displayed. Returns false if the unit is not casting a spell or the spell has no target.

`SecretArguments=AllowedWhenUntainted`

### UnitSpellHaste

```lua
UnitSpellHaste(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitSpellTargetClass

```lua
UnitSpellTargetClass(unit: UnitToken) -> classFilename: cstring
```

If the unit is currently casting a spell, returns the class of the spell's target unit. Returns nil if the unit is not casting a spell or the spell has no target.

`SecretArguments=AllowedWhenUntainted` `SecretReturns`

### UnitSpellTargetName

```lua
UnitSpellTargetName(unit: UnitToken) -> targetName: string
```

If the unit is currently casting a spell, returns the name of the spell's target unit. Returns nil if the unit is not casting a spell or the spell has no target.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretReturns`

### UnitStagger

```lua
UnitStagger(unit: UnitTokenPvPRestrictedForAddOns) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `number` | `ConditionalSecret` |

### UnitStat

```lua
UnitStat(unit: UnitToken, index: luaIndex) -> currentStat: number, effectiveStat: number, statPositiveBuff: number, statNegativeBuff: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitSwitchToVehicleSeat

```lua
UnitSwitchToVehicleSeat(unit: UnitToken, virtualSeatIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### UnitTargetsVehicleInRaidUI

```lua
UnitTargetsVehicleInRaidUI(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitThreatLeadSituation

```lua
UnitThreatLeadSituation(unit: UnitToken, mobGUID: UnitToken) -> result: number?
```

Returns a threat state (0-3; representing none, yellow, orange, red) that indicates how far the provided unit is above the secondmost threat on the provided mob. If the unit is not first on threat, will always return red. Can return nil if the provided mob does not exist.

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitThreatStateRestricted`

### UnitThreatPercentageOfLead

```lua
UnitThreatPercentageOfLead(unit: UnitToken, mobGUID: UnitToken) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitThreatValuesRestricted`

### UnitThreatSituation

```lua
UnitThreatSituation(unit: UnitToken, mobGUID: UnitToken?) -> result: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitThreatStateRestricted`

### UnitTokenFromGUID

```lua
UnitTokenFromGUID(unitGUID: WOWGUID) -> unitToken: string?
```

`SecretArguments=AllowedWhenTainted` `SecretWhenUnitIdentityRestricted`

### UnitTreatAsPlayerForDisplay

```lua
UnitTreatAsPlayerForDisplay(unit: UnitToken) -> treatAsPlayer: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitTrialBankedLevels

```lua
UnitTrialBankedLevels(unit: UnitToken) -> bankedLevels: number, xpIntoCurrentLevel: number, xpForNextLevel: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitTrialXP

```lua
UnitTrialXP(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitUsesAmmo

```lua
UnitUsesAmmo(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitUsingVehicle

```lua
UnitUsingVehicle(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### UnitVehicleSeatCount

```lua
UnitVehicleSeatCount(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitVehicleSeatInfo

```lua
UnitVehicleSeatInfo(unit: UnitToken, virtualSeatIndex: luaIndex) -> controlType: cstring, occupantName: cstring, serverName: cstring, ejectable: bool, canSwitchSeats: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### UnitVehicleSkin

```lua
UnitVehicleSkin(unit: UnitToken?) -> result: fileID
```

`SecretArguments=AllowedWhenUntainted`

### UnitWeaponAttackPower

```lua
UnitWeaponAttackPower(unit: UnitToken) -> mainHandWeaponAttackPower: number, offHandWeaponAttackPower: number, rangedWeaponAttackPower: number
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenUnitStatsRestricted`

### UnitWidgetSet

```lua
UnitWidgetSet(unit: UnitToken) -> uiWidgetSet: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### UnitXP

```lua
UnitXP(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### UnitXPMax

```lua
UnitXPMax(unit: UnitToken) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### WorldLootObjectExists

```lua
WorldLootObjectExists(unit: UnitToken?) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTIVE_PLAYER_SPECIALIZATION_CHANGED

```lua
ACTIVE_PLAYER_SPECIALIZATION_CHANGED()
```

`SynchronousEvent`

### ARENA_COOLDOWNS_UPDATE

```lua
ARENA_COOLDOWNS_UPDATE()
```

`SynchronousEvent`

### ARENA_CROWD_CONTROL_SPELL_UPDATE

```lua
ARENA_CROWD_CONTROL_SPELL_UPDATE(unitTarget: UnitTokenVariant, spellID: number)
```

`SecretWhenLossOfControlInfoRestricted` `SynchronousEvent`

### AUTOFOLLOW_BEGIN

```lua
AUTOFOLLOW_BEGIN(name: cstring)
```

`SynchronousEvent`

### AUTOFOLLOW_END

```lua
AUTOFOLLOW_END()
```

`SynchronousEvent`

### CANCEL_SUMMON

```lua
CANCEL_SUMMON()
```

`SynchronousEvent`

### COMBO_TARGET_CHANGED

```lua
COMBO_TARGET_CHANGED()
```

`SynchronousEvent`

### CONFIRM_BINDER

```lua
CONFIRM_BINDER(areaName: cstring)
```

`SynchronousEvent`

### CONFIRM_SUMMON

```lua
CONFIRM_SUMMON(summonReason: number, skippingStartExperience: bool)
```

`SynchronousEvent`

### ECLIPSE_DIRECTION_CHANGE

```lua
ECLIPSE_DIRECTION_CHANGE(direction: cstring)
```

`SynchronousEvent`

### HEARTHSTONE_BOUND

```lua
HEARTHSTONE_BOUND()
```

`SynchronousEvent`

### HONOR_XP_UPDATE

```lua
HONOR_XP_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### INCOMING_RESURRECT_CHANGED

```lua
INCOMING_RESURRECT_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### INCOMING_SUMMON_CHANGED

```lua
INCOMING_SUMMON_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### KNOWN_TITLES_UPDATE

```lua
KNOWN_TITLES_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### LOCALPLAYER_PET_RENAMED

```lua
LOCALPLAYER_PET_RENAMED()
```

`SynchronousEvent`

### MIRROR_TIMER_PAUSE

```lua
MIRROR_TIMER_PAUSE(timerName: cstring, paused: number)
```

`SynchronousEvent`

### MIRROR_TIMER_START

```lua
MIRROR_TIMER_START(timerName: cstring, value: number, maxValue: number, scale: number, paused: number, timerLabel: cstring)
```

`SynchronousEvent`

### MIRROR_TIMER_STOP

```lua
MIRROR_TIMER_STOP(timerName: cstring)
```

`SynchronousEvent`

### NEUTRAL_FACTION_SELECT_RESULT

```lua
NEUTRAL_FACTION_SELECT_RESULT(success: bool)
```

`SynchronousEvent`

### OBJECT_ENTERED_AOI

```lua
OBJECT_ENTERED_AOI(guid: WOWGUID)
```

`SynchronousEvent`

### OBJECT_LEFT_AOI

```lua
OBJECT_LEFT_AOI(guid: WOWGUID)
```

`SynchronousEvent`

### PARTY_KILL

```lua
PARTY_KILL(attackerGUID: WOWGUID, targetGUID: WOWGUID)
```

`SecretWhenUnitIdentityRestricted` `SynchronousEvent`

### PET_BAR_UPDATE_USABLE

```lua
PET_BAR_UPDATE_USABLE()
```

`SynchronousEvent`

### PET_UI_UPDATE

```lua
PET_UI_UPDATE()
```

`SynchronousEvent`

### PLAYER_CAN_GLIDE_CHANGED

```lua
PLAYER_CAN_GLIDE_CHANGED(canGlide: bool)
```

`SynchronousEvent`

### PLAYER_DAMAGE_DONE_MODS

```lua
PLAYER_DAMAGE_DONE_MODS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_ENTER_COMBAT

```lua
PLAYER_ENTER_COMBAT()
```

`SynchronousEvent`

### PLAYER_FARSIGHT_FOCUS_CHANGED

```lua
PLAYER_FARSIGHT_FOCUS_CHANGED()
```

`SynchronousEvent`

### PLAYER_FLAGS_CHANGED

```lua
PLAYER_FLAGS_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_FOCUS_CHANGED

```lua
PLAYER_FOCUS_CHANGED()
```

`SynchronousEvent`

### PLAYER_IMPULSE_APPLIED

```lua
PLAYER_IMPULSE_APPLIED()
```

`SynchronousEvent`

### PLAYER_IS_GLIDING_CHANGED

```lua
PLAYER_IS_GLIDING_CHANGED(isGliding: bool)
```

`SynchronousEvent`

### PLAYER_LEAVE_COMBAT

```lua
PLAYER_LEAVE_COMBAT()
```

`SynchronousEvent`

### PLAYER_LEVEL_CHANGED

```lua
PLAYER_LEVEL_CHANGED(oldLevel: number, newLevel: number, real: bool)
```

`SynchronousEvent`

### PLAYER_LEVEL_UP

```lua
PLAYER_LEVEL_UP(level: number, healthDelta: number, powerDelta: number, numNewTalents: number, numNewPvpTalentSlots: number, strengthDelta: number, agilityDelta: number, staminaDelta: number, intellectDelta: number, spiritDelta: number)
```

`SynchronousEvent`

### PLAYER_MAX_LEVEL_UPDATE

```lua
PLAYER_MAX_LEVEL_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_MOUNT_DISPLAY_CHANGED

```lua
PLAYER_MOUNT_DISPLAY_CHANGED()
```

`SynchronousEvent`

### PLAYER_PVP_KILLS_CHANGED

```lua
PLAYER_PVP_KILLS_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_PVP_RANK_CHANGED

```lua
PLAYER_PVP_RANK_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_REGEN_DISABLED

```lua
PLAYER_REGEN_DISABLED()
```

`SynchronousEvent`

### PLAYER_REGEN_ENABLED

```lua
PLAYER_REGEN_ENABLED()
```

`SynchronousEvent`

### PLAYER_SOFT_ENEMY_CHANGED

```lua
PLAYER_SOFT_ENEMY_CHANGED()
```

`SynchronousEvent`

### PLAYER_SOFT_FRIEND_CHANGED

```lua
PLAYER_SOFT_FRIEND_CHANGED()
```

`SynchronousEvent`

### PLAYER_SOFT_INTERACT_CHANGED

```lua
PLAYER_SOFT_INTERACT_CHANGED(oldTarget: WOWGUID, newTarget: WOWGUID)
```

`SecretWhenUnitIdentityRestricted` `SynchronousEvent`

### PLAYER_SOFT_TARGET_INTERACTION

```lua
PLAYER_SOFT_TARGET_INTERACTION()
```

`SynchronousEvent`

### PLAYER_SPECIALIZATION_CHANGED

```lua
PLAYER_SPECIALIZATION_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### PLAYER_STARTED_LOOKING

```lua
PLAYER_STARTED_LOOKING()
```

`SynchronousEvent`

### PLAYER_STARTED_MOVING

```lua
PLAYER_STARTED_MOVING()
```

`SynchronousEvent`

### PLAYER_STARTED_TURNING

```lua
PLAYER_STARTED_TURNING()
```

`SynchronousEvent`

### PLAYER_STOPPED_LOOKING

```lua
PLAYER_STOPPED_LOOKING()
```

`SynchronousEvent`

### PLAYER_STOPPED_MOVING

```lua
PLAYER_STOPPED_MOVING()
```

`SynchronousEvent`

### PLAYER_STOPPED_TURNING

```lua
PLAYER_STOPPED_TURNING()
```

`SynchronousEvent`

### PLAYER_TARGET_CHANGED

```lua
PLAYER_TARGET_CHANGED()
```

`SynchronousEvent`

### PLAYER_TRIAL_XP_UPDATE

```lua
PLAYER_TRIAL_XP_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_UPDATE_RESTING

```lua
PLAYER_UPDATE_RESTING()
```

`SynchronousEvent`

### PLAYER_XP_UPDATE

```lua
PLAYER_XP_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PORTRAITS_UPDATED

```lua
PORTRAITS_UPDATED()
```

`UniqueEvent`

### PROVING_GROUNDS_SCORE_UPDATE

```lua
PROVING_GROUNDS_SCORE_UPDATE(points: number)
```

`SynchronousEvent`

### PVP_TIMER_UPDATE

```lua
PVP_TIMER_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### RUNE_POWER_UPDATE

```lua
RUNE_POWER_UPDATE(runeIndex: number, added: bool?)
```

`SecretPayloads` `SynchronousEvent`

### RUNE_TYPE_UPDATE

```lua
RUNE_TYPE_UPDATE(runeIndex: number)
```

`SecretPayloads` `SynchronousEvent`

### SHOW_FACTION_SELECT_UI

```lua
SHOW_FACTION_SELECT_UI()
```

`SynchronousEvent`

### SPELL_CONFIRMATION_PROMPT

```lua
SPELL_CONFIRMATION_PROMPT(spellID: number, effectValue: number, message: cstring, duration: number, currencyTypesID: number, currencyCost: number, currentDifficulty: number, displayItemID: number, itemContext: number, treasureContextLevel: number)
```

`SynchronousEvent`

### SPELL_CONFIRMATION_TIMEOUT

```lua
SPELL_CONFIRMATION_TIMEOUT(spellID: number, effectValue: number)
```

`SynchronousEvent`

### UNIT_ABSORB_AMOUNT_CHANGED

```lua
UNIT_ABSORB_AMOUNT_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_AREA_CHANGED

```lua
UNIT_AREA_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_ARENA_COOLDOWNS_UPDATE

```lua
UNIT_ARENA_COOLDOWNS_UPDATE(unitTarget: UnitTokenVariant)
```

Only signaled when the active player is a commentator or spectator.

`SynchronousEvent` `UniqueEvent`

### UNIT_ATTACK

```lua
UNIT_ATTACK(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_ATTACK_POWER

```lua
UNIT_ATTACK_POWER(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_ATTACK_SPEED

```lua
UNIT_ATTACK_SPEED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_CHEAT_TOGGLE_EVENT

```lua
UNIT_CHEAT_TOGGLE_EVENT()
```

`SynchronousEvent`

### UNIT_CLASSIFICATION_CHANGED

```lua
UNIT_CLASSIFICATION_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_COMBAT

```lua
UNIT_COMBAT(unitTarget: UnitTokenVariant, event: cstring, flagText: cstring, amount: number, schoolMask: number)
```

`SynchronousEvent`

### UNIT_CONNECTION

```lua
UNIT_CONNECTION(unitTarget: UnitTokenVariant, isConnected: bool)
```

`SynchronousEvent`

### UNIT_CTR_OPTIONS

```lua
UNIT_CTR_OPTIONS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_DAMAGE

```lua
UNIT_DAMAGE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_DEFENSE

```lua
UNIT_DEFENSE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_DIED

```lua
UNIT_DIED(unitGUID: WOWGUID)
```

`SecretWhenUnitIdentityRestricted` `SynchronousEvent`

### UNIT_DISPLAYPOWER

```lua
UNIT_DISPLAYPOWER(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_DISTANCE_CHECK_UPDATE

```lua
UNIT_DISTANCE_CHECK_UPDATE(unitTarget: UnitTokenVariant, isInDistance: bool)
```

`SecretPayloads` `SynchronousEvent`

### UNIT_FACTION

```lua
UNIT_FACTION(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_FLAGS

```lua
UNIT_FLAGS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_FORM_CHANGED

```lua
UNIT_FORM_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_HAPPINESS

```lua
UNIT_HAPPINESS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_HEAL_ABSORB_AMOUNT_CHANGED

```lua
UNIT_HEAL_ABSORB_AMOUNT_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_HEAL_PREDICTION

```lua
UNIT_HEAL_PREDICTION(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_HEALTH

```lua
UNIT_HEALTH(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_IN_RANGE_UPDATE

```lua
UNIT_IN_RANGE_UPDATE(unitTarget: UnitTokenVariant, isInRange: bool)
```

`SecretPayloads` `SynchronousEvent`

### UNIT_INVENTORY_CHANGED

```lua
UNIT_INVENTORY_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_LEVEL

```lua
UNIT_LEVEL(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_LOOT

```lua
UNIT_LOOT(unitGUID: WOWGUID, hasLoot: bool)
```

`SynchronousEvent`

### UNIT_MANA

```lua
UNIT_MANA(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_MAXHEALTH

```lua
UNIT_MAXHEALTH(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_MAX_HEALTH_MODIFIERS_CHANGED

```lua
UNIT_MAX_HEALTH_MODIFIERS_CHANGED(unitTarget: UnitTokenVariant, percentMaxHealthAdjusted: number)
```

`SecretPayloads` `SynchronousEvent` `UniqueEvent`

### UNIT_MAXPOWER

```lua
UNIT_MAXPOWER(unitTarget: UnitTokenVariant, powerType: cstring)
```

`SynchronousEvent`

### UNIT_MODEL_CHANGED

```lua
UNIT_MODEL_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_NAME_UPDATE

```lua
UNIT_NAME_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_OTHER_PARTY_CHANGED

```lua
UNIT_OTHER_PARTY_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_PET

```lua
UNIT_PET(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_PET_EXPERIENCE

```lua
UNIT_PET_EXPERIENCE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_PET_TRAINING_POINTS

```lua
UNIT_PET_TRAINING_POINTS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_PHASE

```lua
UNIT_PHASE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_PORTRAIT_UPDATE

```lua
UNIT_PORTRAIT_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_POWER_BAR_HIDE

```lua
UNIT_POWER_BAR_HIDE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_POWER_BAR_SHOW

```lua
UNIT_POWER_BAR_SHOW(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_POWER_BAR_TIMER_UPDATE

```lua
UNIT_POWER_BAR_TIMER_UPDATE(unitTarget: UnitTokenVariant)
```

`UniqueEvent`

### UNIT_POWER_FREQUENT

```lua
UNIT_POWER_FREQUENT(unitTarget: UnitTokenVariant, powerType: cstring)
```

`SynchronousEvent`

### UNIT_POWER_POINT_CHARGE

```lua
UNIT_POWER_POINT_CHARGE(unitTarget: UnitTokenVariant)
```

`SecretWhenUnitPowerRestricted` `UniqueEvent`

### UNIT_POWER_UPDATE

```lua
UNIT_POWER_UPDATE(unitTarget: UnitTokenVariant, powerType: cstring)
```

`SynchronousEvent`

### UNIT_QUEST_LOG_CHANGED

```lua
UNIT_QUEST_LOG_CHANGED(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_RANGED_ATTACK_POWER

```lua
UNIT_RANGED_ATTACK_POWER(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_RANGEDDAMAGE

```lua
UNIT_RANGEDDAMAGE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_RESISTANCES

```lua
UNIT_RESISTANCES(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_SPELLCAST_CHANNEL_START

```lua
UNIT_SPELLCAST_CHANNEL_START(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_CHANNEL_STOP

```lua
UNIT_SPELLCAST_CHANNEL_STOP(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, interruptedBy: WOWGUID, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `interruptedBy` | `WOWGUID` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_CHANNEL_UPDATE

```lua
UNIT_SPELLCAST_CHANNEL_UPDATE(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_DELAYED

```lua
UNIT_SPELLCAST_DELAYED(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_EMPOWER_START

```lua
UNIT_SPELLCAST_EMPOWER_START(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_EMPOWER_STOP

```lua
UNIT_SPELLCAST_EMPOWER_STOP(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, complete: bool, interruptedBy: WOWGUID, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `complete` | `bool` |  |
| `interruptedBy` | `WOWGUID` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_EMPOWER_UPDATE

```lua
UNIT_SPELLCAST_EMPOWER_UPDATE(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_FAILED

```lua
UNIT_SPELLCAST_FAILED(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_FAILED_QUIET

```lua
UNIT_SPELLCAST_FAILED_QUIET(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_INTERRUPTED

```lua
UNIT_SPELLCAST_INTERRUPTED(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, interruptedBy: WOWGUID, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `interruptedBy` | `WOWGUID` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_INTERRUPTIBLE

```lua
UNIT_SPELLCAST_INTERRUPTIBLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_SPELLCAST_NOT_INTERRUPTIBLE

```lua
UNIT_SPELLCAST_NOT_INTERRUPTIBLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_SPELLCAST_RETICLE_CLEAR

```lua
UNIT_SPELLCAST_RETICLE_CLEAR(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

### UNIT_SPELLCAST_RETICLE_TARGET

```lua
UNIT_SPELLCAST_RETICLE_TARGET(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

### UNIT_SPELLCAST_SENT

```lua
UNIT_SPELLCAST_SENT(unitTarget: UnitTokenVariant, target: cstring, castGUID: WOWGUID, spellID: number)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `target` | `cstring` | `ConditionalSecret` |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |

### UNIT_SPELLCAST_START

```lua
UNIT_SPELLCAST_START(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_STOP

```lua
UNIT_SPELLCAST_STOP(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELLCAST_SUCCEEDED

```lua
UNIT_SPELLCAST_SUCCEEDED(unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?)
```

`SecretWhenUnitSpellCastRestricted` `SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `unitTarget` | `UnitTokenVariant` |  |
| `castGUID` | `WOWGUID` |  |
| `spellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UNIT_SPELL_HASTE

```lua
UNIT_SPELL_HASTE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_STATS

```lua
UNIT_STATS(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_TARGET

```lua
UNIT_TARGET(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### UNIT_TARGETABLE_CHANGED

```lua
UNIT_TARGETABLE_CHANGED(unitTarget: UnitTokenVariant)
```

`UniqueEvent`

### UNIT_THREAT_LIST_UPDATE

```lua
UNIT_THREAT_LIST_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UNIT_THREAT_SITUATION_UPDATE

```lua
UNIT_THREAT_SITUATION_UPDATE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent` `UniqueEvent`

### UPDATE_EXHAUSTION

```lua
UPDATE_EXHAUSTION()
```

`SynchronousEvent`

### UPDATE_MOUSEOVER_UNIT

```lua
UPDATE_MOUSEOVER_UNIT()
```

`SynchronousEvent`

### UPDATE_STEALTH

```lua
UPDATE_STEALTH()
```

`SynchronousEvent`

### VEHICLE_ANGLE_UPDATE

```lua
VEHICLE_ANGLE_UPDATE(normalizedPitch: number, radians: number)
```

`SynchronousEvent`

## Types

### PhaseReason

*Enumeration* · 6 values, 0..5

Access values as `Enum.PhaseReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Phasing` | `PhaseReason` | = 0 |
| `Sharding` | `PhaseReason` | = 1 |
| `WarMode` | `PhaseReason` | = 2 |
| `ChromieTime` | `PhaseReason` | = 3 |
| `TimerunningHwt` | `PhaseReason` | = 4 |
| `RuleSet` | `PhaseReason` | = 5 |

### PvPUnitClassification

*Enumeration* · 11 values, 0..10

Access values as `Enum.PvPUnitClassification.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FlagCarrierHorde` | `PvPUnitClassification` | = 0 |
| `FlagCarrierAlliance` | `PvPUnitClassification` | = 1 |
| `FlagCarrierNeutral` | `PvPUnitClassification` | = 2 |
| `CartRunnerHorde` | `PvPUnitClassification` | = 3 |
| `CartRunnerAlliance` | `PvPUnitClassification` | = 4 |
| `AssassinHorde` | `PvPUnitClassification` | = 5 |
| `AssassinAlliance` | `PvPUnitClassification` | = 6 |
| `OrbCarrierBlue` | `PvPUnitClassification` | = 7 |
| `OrbCarrierGreen` | `PvPUnitClassification` | = 8 |
| `OrbCarrierOrange` | `PvPUnitClassification` | = 9 |
| `OrbCarrierPurple` | `PvPUnitClassification` | = 10 |

### CorruptionEffectInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `description` | `string` |  |
| `minCorruption` | `number` |  |

### UnitCastingInfoResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayName` | `string` |  |
| `textureID` | `fileID` |  |
| `startTimeMs` | `number` |  |
| `endTimeMs` | `number` |  |
| `isTradeskill` | `bool` | `NeverSecret` |
| `castID` | `WOWGUID` |  |
| `notInterruptible` | `bool?` |  |
| `castingSpellID` | `number` |  |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |
| `delayTimeMs` | `number` | `NeverSecret` |

### UnitChannelInfoResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `displayName` | `cstring` |  |
| `textureID` | `fileID` |  |
| `startTimeMs` | `number` |  |
| `endTimeMs` | `number` |  |
| `isTradeskill` | `bool` | `NeverSecret` |
| `notInterruptible` | `bool?` |  |
| `spellID` | `number` |  |
| `isEmpowered` | `bool` | `NeverSecret` |
| `numEmpowerStages` | `number` | `NeverSecret` |
| `castBarID` | `UnitCastBarID?` | `NeverSecret` |

### UnitCreatureFamilyResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `id` | `number` |  |

### UnitCreatureTypeResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `id` | `number` |  |

### UnitPowerBarInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `barType` | `number` |  |
| `minPower` | `number` |  |
| `startInset` | `number` |  |
| `endInset` | `number` |  |
| `smooth` | `bool` |  |
| `hideFromOthers` | `bool` |  |
| `showOnRaid` | `bool` |  |
| `opaqueSpark` | `bool` |  |
| `opaqueFlash` | `bool` |  |
| `anchorTop` | `bool` |  |
| `forcePercentage` | `bool` |  |
| `sparkUnderFrame` | `bool` |  |
| `flashAtMinPower` | `bool` |  |
| `fractionalCounter` | `bool` |  |
| `animateNumbers` | `bool` |  |
| `attachTooltipToBar` | `bool` |  |
