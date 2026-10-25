# DelvesUI

Namespace `C_DelvesUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/delvesuidocumentation.lua` (FileDataID 5920189)

## Functions

### GetActiveDelveTier

```lua
C_DelvesUI.GetActiveDelveTier() -> tierInfo: TieredEntranceTierInfo
```

Returns the entrance tier information for the active Delve (via party data). Assumes only Delves use this type for now.

### GetCompanionInfoForActivePlayer

```lua
C_DelvesUI.GetCompanionInfoForActivePlayer() -> playerCompanionInfoID: number
```

### GetCreatureDisplayInfoForCompanion

```lua
C_DelvesUI.GetCreatureDisplayInfoForCompanion(companionID: number?) -> creatureDisplayInfoID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCurioLink

```lua
C_DelvesUI.GetCurioLink(spellID: SpellIdentifier, rarity: CurioRarity) -> curioLink: cstring
```

Given the spell ID for an owned curio and its rarity, return a spell link style hyperlink for the curio spell, since they aren't items when learned

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` |  |
| `rarity` | `CurioRarity` | `NeverSecret` |

### GetCurioNodeForCompanion

```lua
C_DelvesUI.GetCurioNodeForCompanion(curioType: CurioType, companionID: number?) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCurioRarityByTraitCondAccountElementID

```lua
C_DelvesUI.GetCurioRarityByTraitCondAccountElementID(traitCondAccountElementID: number) -> rarity: CurioRarity
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentDelvesSeasonNumber

```lua
C_DelvesUI.GetCurrentDelvesSeasonNumber() -> seasonNumber: number
```

### GetDelveEntranceBackgroundWidgetSetID

```lua
C_DelvesUI.GetDelveEntranceBackgroundWidgetSetID() -> backgroundWidgetSetID: number
```

### GetDelveEntranceDescriptionString

```lua
C_DelvesUI.GetDelveEntranceDescriptionString() -> description: string?
```

### GetDelveEntranceHeaderString

```lua
C_DelvesUI.GetDelveEntranceHeaderString() -> header: string?
```

### GetDelveEntranceMapID

```lua
C_DelvesUI.GetDelveEntranceMapID() -> mapID: number
```

### GetDelveEntranceTiers

```lua
C_DelvesUI.GetDelveEntranceTiers() -> levelInfo: TieredEntranceTierInfo[]
```

### GetDelveEntranceTitleString

```lua
C_DelvesUI.GetDelveEntranceTitleString() -> title: cstring?
```

### GetDelvesAffixSpellsForSeason

```lua
C_DelvesUI.GetDelvesAffixSpellsForSeason() -> affixSpellIDs: number[]
```

### GetDelvesFactionForSeason

```lua
C_DelvesUI.GetDelvesFactionForSeason() -> factionID: number
```

### GetDelvesMinRequiredLevel

```lua
C_DelvesUI.GetDelvesMinRequiredLevel() -> minRequiredLevel: number?
```

Players must be at or above the min level + offset to enter Delves. This function returns that min level.

### GetFactionForCompanion

```lua
C_DelvesUI.GetFactionForCompanion(companionID: number?) -> factionID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetFlavorNodeForCompanion

```lua
C_DelvesUI.GetFlavorNodeForCompanion(companionID: number?) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetFlavorNodeNameForCompanion

```lua
C_DelvesUI.GetFlavorNodeNameForCompanion(companionID: number?) -> name: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetLockedTextForCompanion

```lua
C_DelvesUI.GetLockedTextForCompanion(companionID: number?) -> text: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetModelSceneForCompanion

```lua
C_DelvesUI.GetModelSceneForCompanion(companionID: number?) -> modelSceneID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerCompanionPDEID

```lua
C_DelvesUI.GetPlayerCompanionPDEID(companionID: number?) -> pdeID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRoleNodeForCompanion

```lua
C_DelvesUI.GetRoleNodeForCompanion(companionID: number?) -> nodeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetRoleSubtreeForCompanion

```lua
C_DelvesUI.GetRoleSubtreeForCompanion(roleType: CompanionRoleType, companionID: number?) -> subTreeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTieredEntranceOptionalAffixTraitTreeID

```lua
C_DelvesUI.GetTieredEntranceOptionalAffixTraitTreeID() -> treeID: number?
```

### GetTieredEntrancePDEID

```lua
C_DelvesUI.GetTieredEntrancePDEID() -> pdeID: number
```

### GetTieredEntranceType

```lua
C_DelvesUI.GetTieredEntranceType() -> entranceType: TieredEntranceType
```

### GetTraitTreeForCompanion

```lua
C_DelvesUI.GetTraitTreeForCompanion(companionID: number?) -> treeID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetUnseenCuriosBySlotType

```lua
C_DelvesUI.GetUnseenCuriosBySlotType(slotType: CompanionConfigSlotTypes, ownedCurioNodeIDs: number[]) -> unseenCurioNodeIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetWorldTierDifficultyForActivePlayer

```lua
C_DelvesUI.GetWorldTierDifficultyForActivePlayer() -> difficulty: WorldTierDifficulty
```

### HasActiveDelve

```lua
C_DelvesUI.HasActiveDelve() -> result: bool
```

### HasActiveLair

```lua
C_DelvesUI.HasActiveLair() -> result: bool
```

### HasActiveLFGLair

```lua
C_DelvesUI.HasActiveLFGLair() -> result: bool
```

### IsDelveEntranceTierEnabled

```lua
C_DelvesUI.IsDelveEntranceTierEnabled(tier: number) -> isEnabled: bool, failureReason: string?
```

`SecretArguments=AllowedWhenUntainted`

### IsEligibleForActiveDelveRewards

```lua
C_DelvesUI.IsEligibleForActiveDelveRewards(unit: UnitToken) -> result: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsInLair

```lua
C_DelvesUI.IsInLair() -> result: bool
```

### IsTraitTreeForCompanion

```lua
C_DelvesUI.IsTraitTreeForCompanion(traitTreeID: number) -> isForCompanion: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestPartyEligibilityForDelveTiers

```lua
C_DelvesUI.RequestPartyEligibilityForDelveTiers(mapID: number)
```

Queries private party members to see what level they have unlocked for the Delve. Ineligible members are added to the tooltip of dropdown entries.

`SecretArguments=AllowedWhenUntainted`

### SaveSeenCuriosBySlotType

```lua
C_DelvesUI.SaveSeenCuriosBySlotType(slotType: CompanionConfigSlotTypes, ownedCurioNodeIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### SelectDelveEntranceTier

```lua
C_DelvesUI.SelectDelveEntranceTier(tier: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTIVE_DELVE_DATA_UPDATE

```lua
ACTIVE_DELVE_DATA_UPDATE()
```

Signaled when SpellScript calls change the data for players/parties owning a delve or when the delve is shut down.

`SynchronousEvent`

### DELVE_ASSIST_ACTION

```lua
DELVE_ASSIST_ACTION(data: DelveAssistActionData)
```

Signaled when an assist action occurs in a delve.

`SynchronousEvent`

### DELVES_ACCOUNT_DATA_ELEMENT_CHANGED

```lua
DELVES_ACCOUNT_DATA_ELEMENT_CHANGED()
```

Signaled when player account data element(s) have changed. This drives curio ranks, and the UI should update when this is sent.

`SynchronousEvent`

### PARTY_ELIGIBILITY_FOR_DELVE_TIERS_CHANGED

```lua
PARTY_ELIGIBILITY_FOR_DELVE_TIERS_CHANGED(playerName: string, maxEligibleLevel: number)
```

Signaled when responses come in from RequestPartyEligibilityForDelveTiers.

`SynchronousEvent`

### SHOW_DELVES_COMPANION_CONFIGURATION_UI

```lua
SHOW_DELVES_COMPANION_CONFIGURATION_UI()
```

Signaled when SpellScript indicates that a curio has been learned or upgraded. Will show the companion config UI.

`SynchronousEvent`

### WALK_IN_DATA_UPDATE

```lua
WALK_IN_DATA_UPDATE()
```

Signaled when the player or a private party member join a new walk-in instance or when the instance is shut down.

`SynchronousEvent`

## Types

### CompanionRoleType

*Enumeration* · 3 values, 0..2

Access values as `Enum.CompanionRoleType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Dps` | `CompanionRoleType` | = 0 |
| `Heal` | `CompanionRoleType` | = 1 |
| `Tank` | `CompanionRoleType` | = 2 |

### CurioType

*Enumeration* · 2 values, 0..1

Access values as `Enum.CurioType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Combat` | `CurioType` | = 0 |
| `Utility` | `CurioType` | = 1 |

### TieredEntranceRewardType

*Enumeration* · 2 values, 0..1

Access values as `Enum.TieredEntranceRewardType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `TieredEntranceRewardType` | = 0 |
| `Currency` | `TieredEntranceRewardType` | = 1 |

### TieredEntranceRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `quantity` | `number` |  |
| `rewardType` | `TieredEntranceRewardType` |  |
| `context` | `ItemCreationContext` |  |

### TieredEntranceTierInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tier` | `number` |  |
| `suggestedILvl` | `number` |  |
| `overrideTooltipSpellID` | `number` |  |
| `unlocked` | `bool` |  |
| `tierDescription` | `string` |  |
| `rewards` | `TieredEntranceRewardInfo[]` |  |
| `modifierUIWidgetSetID` | `number` |  |
| `lockedReason` | `string?` |  |
| `queueAsLFG` | `bool` |  |
| `difficultyID` | `number` |  |
