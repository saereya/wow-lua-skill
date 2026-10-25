# ArtifactUI

Namespace `C_ArtifactUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/artifactuidocumentation.lua` (FileDataID 4637021)

## Functions

### AddPower

```lua
C_ArtifactUI.AddPower(powerID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### ApplyCursorRelicToSlot

```lua
C_ArtifactUI.ApplyCursorRelicToSlot(relicSlotIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### CanApplyArtifactRelic

```lua
C_ArtifactUI.CanApplyArtifactRelic(relicItemID: number, onlyUnlocked: bool) -> canApply: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanApplyCursorRelicToSlot

```lua
C_ArtifactUI.CanApplyCursorRelicToSlot(relicSlotIndex: luaIndex) -> canApply: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanApplyRelicItemIDToEquippedArtifactSlot

```lua
C_ArtifactUI.CanApplyRelicItemIDToEquippedArtifactSlot(relicItemID: number, relicSlotIndex: luaIndex) -> canApply: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanApplyRelicItemIDToSlot

```lua
C_ArtifactUI.CanApplyRelicItemIDToSlot(relicItemID: number, relicSlotIndex: luaIndex) -> canApply: bool
```

`SecretArguments=AllowedWhenUntainted`

### CheckRespecNPC

```lua
C_ArtifactUI.CheckRespecNPC() -> canRespec: bool
```

### Clear

```lua
C_ArtifactUI.Clear()
```

### ClearForgeCamera

```lua
C_ArtifactUI.ClearForgeCamera()
```

### ConfirmRespec

```lua
C_ArtifactUI.ConfirmRespec()
```

### DoesEquippedArtifactHaveAnyRelicsSlotted

```lua
C_ArtifactUI.DoesEquippedArtifactHaveAnyRelicsSlotted() -> hasAnyRelicsSlotted: bool
```

### GetAppearanceInfo

```lua
C_ArtifactUI.GetAppearanceInfo(appearanceSetIndex: number, appearanceIndex: number) -> artifactAppearanceID: number, appearanceName: string, displayIndex: number, unlocked: bool, failureDescription: string?, uiCameraID: number, altHandCameraID: number?, swatchColorR: number, swatchColorG: number, swatchColorB: number, modelOpacity: number, modelSaturation: number, obtainable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAppearanceInfoByID

```lua
C_ArtifactUI.GetAppearanceInfoByID(artifactAppearanceID: number) -> artifactAppearanceSetID: number, artifactAppearanceID: number, appearanceName: string, displayIndex: number, unlocked: bool, failureDescription: string?, uiCameraID: number, altHandCameraID: number?, swatchColorR: number, swatchColorG: number, swatchColorB: number, modelOpacity: number, modelSaturation: number, obtainable: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAppearanceSetInfo

```lua
C_ArtifactUI.GetAppearanceSetInfo(appearanceSetIndex: number) -> artifactAppearanceSetID: number, appearanceSetName: string, appearanceSetDescription: string, numAppearances: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetArtifactArtInfo

```lua
C_ArtifactUI.GetArtifactArtInfo() -> artifactArtInfo: ArtifactArtInfo
```

`MayReturnNothing`

### GetArtifactInfo

```lua
C_ArtifactUI.GetArtifactInfo() -> itemID: number, altItemID: number?, name: string, icon: fileID, xp: number, pointsSpent: number, quality: number, artifactAppearanceID: number, appearanceModID: number, itemAppearanceID: number?, altItemAppearanceID: number?, altOnTop: bool, tier: ArtifactTiers
```

`MayReturnNothing`

### GetArtifactItemID

```lua
C_ArtifactUI.GetArtifactItemID() -> itemID: number
```

`MayReturnNothing`

### GetArtifactTier

```lua
C_ArtifactUI.GetArtifactTier() -> tier: ArtifactTiers?
```

### GetArtifactXPRewardTargetInfo

```lua
C_ArtifactUI.GetArtifactXPRewardTargetInfo(artifactCategoryID: number) -> name: string, icon: fileID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCostForPointAtRank

```lua
C_ArtifactUI.GetCostForPointAtRank(rank: number, tier: ArtifactTiers) -> cost: number
```

`SecretArguments=AllowedWhenUntainted`

### GetEquippedArtifactArtInfo

```lua
C_ArtifactUI.GetEquippedArtifactArtInfo() -> artifactArtInfo: ArtifactArtInfo
```

`MayReturnNothing`

### GetEquippedArtifactInfo

```lua
C_ArtifactUI.GetEquippedArtifactInfo() -> itemID: number, altItemID: number?, name: string, icon: fileID, xp: number, pointsSpent: number, quality: number, artifactAppearanceID: number, appearanceModID: number, itemAppearanceID: number?, altItemAppearanceID: number?, altOnTop: bool, tier: ArtifactTiers
```

`MayReturnNothing`

### GetEquippedArtifactItemID

```lua
C_ArtifactUI.GetEquippedArtifactItemID() -> itemID: number
```

`MayReturnNothing`

### GetEquippedArtifactNumRelicSlots

```lua
C_ArtifactUI.GetEquippedArtifactNumRelicSlots(onlyUnlocked: bool) -> numRelicSlots: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `onlyUnlocked` | `bool` | default `false`; If true then only the relic slots that are unlocked will be considered. |

### GetEquippedArtifactRelicInfo

```lua
C_ArtifactUI.GetEquippedArtifactRelicInfo(relicSlotIndex: luaIndex) -> name: string, icon: fileID, slotTypeName: cstring, link: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `slotTypeName` | `cstring` | Matches the socket identifiers used in the socketing system. |
| `link` | `string` |  |

### GetEquippedRelicLockedReason

```lua
C_ArtifactUI.GetEquippedRelicLockedReason(relicSlotIndex: luaIndex) -> lockedReason: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetForgeRotation

```lua
C_ArtifactUI.GetForgeRotation() -> forgeRotationX: number, forgeRotationY: number, forgeRotationZ: number
```

### GetItemLevelIncreaseProvidedByRelic

```lua
C_ArtifactUI.GetItemLevelIncreaseProvidedByRelic(itemLinkOrID: ItemInfo) -> itemIevelIncrease: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMetaPowerInfo

```lua
C_ArtifactUI.GetMetaPowerInfo() -> spellID: number, powerCost: number, currentRank: number
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` | `StrideIndex=1` |
| `powerCost` | `number` | `StrideIndex=2` |
| `currentRank` | `number` | `StrideIndex=3` |

### GetNumAppearanceSets

```lua
C_ArtifactUI.GetNumAppearanceSets() -> numAppearanceSets: number
```

### GetNumObtainedArtifacts

```lua
C_ArtifactUI.GetNumObtainedArtifacts() -> numObtainedArtifacts: number
```

### GetNumRelicSlots

```lua
C_ArtifactUI.GetNumRelicSlots(onlyUnlocked: bool) -> numRelicSlots: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `onlyUnlocked` | `bool` | default `false`; If true then only the relic slots that are unlocked will be considered. |

### GetPointsRemaining

```lua
C_ArtifactUI.GetPointsRemaining() -> pointsRemaining: number
```

### GetPowerHyperlink

```lua
C_ArtifactUI.GetPowerHyperlink(powerID: number) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetPowerInfo

```lua
C_ArtifactUI.GetPowerInfo(powerID: number) -> powerInfo: ArtifactPowerInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPowerLinks

```lua
C_ArtifactUI.GetPowerLinks(powerID: number) -> linkingPowerID: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetPowers

```lua
C_ArtifactUI.GetPowers() -> powerID: number[]
```

`MayReturnNothing`

### GetPowersAffectedByRelic

```lua
C_ArtifactUI.GetPowersAffectedByRelic(relicSlotIndex: luaIndex) -> powerIDs: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `powerIDs` | `number` | `StrideIndex=1` |

### GetPowersAffectedByRelicItemLink

```lua
C_ArtifactUI.GetPowersAffectedByRelicItemLink(relicItemInfo: ItemInfo) -> powerIDs: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `powerIDs` | `number` | `StrideIndex=1` |

### GetPreviewAppearance

```lua
C_ArtifactUI.GetPreviewAppearance() -> artifactAppearanceID: number?
```

### GetRelicInfo

```lua
C_ArtifactUI.GetRelicInfo(relicSlotIndex: luaIndex) -> name: string, icon: fileID, slotTypeName: cstring, link: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `slotTypeName` | `cstring` | Matches the socket identifiers used in the socketing system. |
| `link` | `string` |  |

### GetRelicInfoByItemID

```lua
C_ArtifactUI.GetRelicInfoByItemID(itemID: number) -> name: string, icon: fileID, slotTypeName: cstring, link: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `slotTypeName` | `cstring` | Matches the socket identifiers used in the socketing system. |
| `link` | `string` |  |

### GetRelicLockedReason

```lua
C_ArtifactUI.GetRelicLockedReason(relicSlotIndex: luaIndex) -> lockedReason: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetRelicSlotType

```lua
C_ArtifactUI.GetRelicSlotType(relicSlotIndex: luaIndex) -> slotTypeName: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetRespecArtifactArtInfo

```lua
C_ArtifactUI.GetRespecArtifactArtInfo() -> artifactArtInfo: ArtifactArtInfo
```

`MayReturnNothing`

### GetRespecArtifactInfo

```lua
C_ArtifactUI.GetRespecArtifactInfo() -> itemID: number, altItemID: number?, name: string, icon: fileID, xp: number, pointsSpent: number, quality: number, artifactAppearanceID: number, appearanceModID: number, itemAppearanceID: number?, altItemAppearanceID: number?, altOnTop: bool, tier: ArtifactTiers
```

`MayReturnNothing`

### GetRespecCost

```lua
C_ArtifactUI.GetRespecCost() -> cost: number
```

### GetTotalPowerCost

```lua
C_ArtifactUI.GetTotalPowerCost(startingTrait: luaIndex, numTraits: number, artifactTier: ArtifactTiers) -> totalArtifactPowerCost: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTotalPurchasedRanks

```lua
C_ArtifactUI.GetTotalPurchasedRanks() -> totalPurchasedRanks: number
```

### IsArtifactDisabled

```lua
C_ArtifactUI.IsArtifactDisabled() -> artifactDisabled: bool
```

### IsArtifactItem

```lua
C_ArtifactUI.IsArtifactItem(itemLocation: ItemLocation) -> isArtifact: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsAtForge

```lua
C_ArtifactUI.IsAtForge() -> isAtForge: bool
```

### IsEquippedArtifactDisabled

```lua
C_ArtifactUI.IsEquippedArtifactDisabled() -> artifactDisabled: bool
```

### IsEquippedArtifactMaxed

```lua
C_ArtifactUI.IsEquippedArtifactMaxed() -> artifactMaxed: bool
```

### IsMaxedByRulesOrEffect

```lua
C_ArtifactUI.IsMaxedByRulesOrEffect() -> isEffectivelyMaxed: bool
```

### IsPowerKnown

```lua
C_ArtifactUI.IsPowerKnown(powerID: number) -> known: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsViewedArtifactEquipped

```lua
C_ArtifactUI.IsViewedArtifactEquipped() -> isViewedArtifactEquipped: bool
```

### SetAppearance

```lua
C_ArtifactUI.SetAppearance(artifactAppearanceID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetForgeCamera

```lua
C_ArtifactUI.SetForgeCamera()
```

### SetForgeRotation

```lua
C_ArtifactUI.SetForgeRotation(forgeRotationX: number, forgeRotationY: number, forgeRotationZ: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPreviewAppearance

```lua
C_ArtifactUI.SetPreviewAppearance(artifactAppearanceID: number)
```

Call without an argument to clear the preview.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `artifactAppearanceID` | `number` | default `0` |

### ShouldSuppressForgeRotation

```lua
C_ArtifactUI.ShouldSuppressForgeRotation() -> shouldSuppressForgeRotation: bool
```

## Events

### ARTIFACT_CLOSE

```lua
ARTIFACT_CLOSE()
```

`SynchronousEvent`

### ARTIFACT_ENDGAME_REFUND

```lua
ARTIFACT_ENDGAME_REFUND(numRefundedPowers: number, refundedTier: ArtifactTiers, bagOrSlotIndex: luaIndex, slotIndex: luaIndex?)
```

`SynchronousEvent`

### ARTIFACT_RELIC_FORGE_CLOSE

```lua
ARTIFACT_RELIC_FORGE_CLOSE()
```

`SynchronousEvent`

### ARTIFACT_RELIC_FORGE_PREVIEW_RELIC_CHANGED

```lua
ARTIFACT_RELIC_FORGE_PREVIEW_RELIC_CHANGED()
```

`SynchronousEvent`

### ARTIFACT_RELIC_FORGE_UPDATE

```lua
ARTIFACT_RELIC_FORGE_UPDATE()
```

`SynchronousEvent`

### ARTIFACT_RELIC_INFO_RECEIVED

```lua
ARTIFACT_RELIC_INFO_RECEIVED()
```

`SynchronousEvent`

### ARTIFACT_RESPEC_PROMPT

```lua
ARTIFACT_RESPEC_PROMPT()
```

`SynchronousEvent`

### ARTIFACT_TIER_CHANGED

```lua
ARTIFACT_TIER_CHANGED(newTier: luaIndex, bagOrSlotIndex: luaIndex, slotIndex: luaIndex?)
```

`SynchronousEvent`

### ARTIFACT_UPDATE

```lua
ARTIFACT_UPDATE(newItem: bool)
```

`SynchronousEvent`

### ARTIFACT_XP_UPDATE

```lua
ARTIFACT_XP_UPDATE()
```

`SynchronousEvent`

## Types

### ArtifactAppearanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `artifactAppearanceID` | `number` |  |
| `appearanceName` | `string` |  |
| `displayIndex` | `number` |  |
| `unlocked` | `bool` |  |
| `failureDescription` | `string?` |  |
| `uiCameraID` | `number` |  |
| `altHandCameraID` | `number?` |  |
| `swatchColor` | `colorRGB` | `Mixin=ColorMixin` |
| `modelOpacity` | `number` |  |
| `modelSaturation` | `number` |  |
| `obtainable` | `bool` |  |

### ArtifactAppearanceSetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `artifactAppearanceSetID` | `number` |  |
| `appearanceSetName` | `string` |  |
| `appearanceSetDescription` | `string` |  |
| `numAppearances` | `number` |  |

### ArtifactArtInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `titleName` | `string` |  |
| `titleColor` | `colorRGB` | `Mixin=ColorMixin` |
| `barConnectedColor` | `colorRGB` | `Mixin=ColorMixin` |
| `barDisconnectedColor` | `colorRGB` | `Mixin=ColorMixin` |
| `uiModelSceneID` | `number` |  |
| `spellVisualKitID` | `number` |  |

### ArtifactInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `altItemID` | `number?` |  |
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `xp` | `number` |  |
| `pointsSpent` | `number` |  |
| `quality` | `number` |  |
| `artifactAppearanceID` | `number` |  |
| `appearanceModID` | `number` |  |
| `itemAppearanceID` | `number?` |  |
| `altItemAppearanceID` | `number?` |  |
| `altOnTop` | `bool` |  |
| `tier` | `ArtifactTiers` |  |

### ArtifactMetaPowerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `powerCost` | `number` |  |
| `currentRank` | `number` |  |

### ArtifactPowerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `cost` | `number` |  |
| `currentRank` | `number` |  |
| `maxRank` | `number` |  |
| `bonusRanks` | `number` |  |
| `numMaxRankBonusFromTier` | `number` |  |
| `prereqsMet` | `bool` |  |
| `isStart` | `bool` |  |
| `isGoldMedal` | `bool` |  |
| `isFinal` | `bool` |  |
| `tier` | `luaIndex` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `offset` | `vector2?` | `Mixin=Vector2DMixin` |
| `linearIndex` | `luaIndex?` |  |

### ArtifactRelicInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `slotTypeName` | `cstring` | Matches the socket identifiers used in the socketing system. |
| `link` | `string` |  |
