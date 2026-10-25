# TransmogOutfitInfo

Namespace `C_TransmogOutfitInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/transmogoutfitinfodocumentation.lua` (FileDataID 7240886)

## Functions

### AddNewOutfit

```lua
C_TransmogOutfitInfo.AddNewOutfit(name: cstring, icon: fileID)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CanPlayerTransmogSlot

```lua
C_TransmogOutfitInfo.CanPlayerTransmogSlot(slot: TransmogOutfitSlot) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### ChangeDisplayedOutfit

```lua
C_TransmogOutfitInfo.ChangeDisplayedOutfit(outfitID: number, trigger: TransmogSituationTrigger, toggleLock: bool, allowRemoveOutfit: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ChangeToOutfit

```lua
C_TransmogOutfitInfo.ChangeToOutfit(playerFacingOutfitIndex: number, allowRemoveOutfit: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ChangeViewedOutfit

```lua
C_TransmogOutfitInfo.ChangeViewedOutfit(outfitID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ClearAllPendingSituations

```lua
C_TransmogOutfitInfo.ClearAllPendingSituations()
```

### ClearAllPendingTransmogs

```lua
C_TransmogOutfitInfo.ClearAllPendingTransmogs()
```

### ClearDisplayedOutfit

```lua
C_TransmogOutfitInfo.ClearDisplayedOutfit(trigger: TransmogSituationTrigger, toggleLock: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ClearOutfit

```lua
C_TransmogOutfitInfo.ClearOutfit()
```

### CommitAndApplyAllPending

```lua
C_TransmogOutfitInfo.CommitAndApplyAllPending(useAvailableDiscount: bool)
```

`SecretArguments=AllowedWhenUntainted`

### CommitOutfitInfo

```lua
C_TransmogOutfitInfo.CommitOutfitInfo(outfitID: number, name: cstring, icon: fileID)
```

`SecretArguments=AllowedWhenUntainted`

### CommitPendingSituations

```lua
C_TransmogOutfitInfo.CommitPendingSituations()
```

### GetActiveOutfitID

```lua
C_TransmogOutfitInfo.GetActiveOutfitID() -> outfitID: number
```

### GetAllSlotLocationInfo

```lua
C_TransmogOutfitInfo.GetAllSlotLocationInfo() -> appearanceSlotInfo: TransmogOutfitSlotInfo[], illusionSlotInfo: TransmogOutfitSlotInfo[]
```

`MayReturnNothing`

### GetAllTransmogOutfitOptionSheatheCategoryInfo

```lua
C_TransmogOutfitInfo.GetAllTransmogOutfitOptionSheatheCategoryInfo(imaID: number) -> categoryInfo: TransmogOutfitOptionSheatheCategoryInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCollectionInfoForSlotAndOption

```lua
C_TransmogOutfitInfo.GetCollectionInfoForSlotAndOption(slot: TransmogOutfitSlot, option: TransmogOutfitSlotOption, collectionType: TransmogCollectionType) -> collectionInfo: TransmogOutfitCollectionInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrentlyViewedOutfitID

```lua
C_TransmogOutfitInfo.GetCurrentlyViewedOutfitID() -> outfitID: number
```

### GetEquippedSlotOptionFromTransmogSlot

```lua
C_TransmogOutfitInfo.GetEquippedSlotOptionFromTransmogSlot(slot: TransmogOutfitSlot) -> option: TransmogOutfitSlotOption
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetIllusionDefaultIMAIDForCollectionType

```lua
C_TransmogOutfitInfo.GetIllusionDefaultIMAIDForCollectionType(collectionType: TransmogCollectionType) -> imaID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemModifiedAppearanceEffectiveCategory

```lua
C_TransmogOutfitInfo.GetItemModifiedAppearanceEffectiveCategory(imaID: number) -> categoryID: TransmogCollectionType
```

`SecretArguments=AllowedWhenUntainted`

### GetLinkedSlotInfo

```lua
C_TransmogOutfitInfo.GetLinkedSlotInfo(slot: TransmogOutfitSlot) -> linkedSlotInfo: TransmogOutfitLinkedSlotInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMaxNumberOfTotalOutfitsForSource

```lua
C_TransmogOutfitInfo.GetMaxNumberOfTotalOutfitsForSource(source: TransmogOutfitEntrySource) -> maxOutfitCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxNumberOfUsableOutfits

```lua
C_TransmogOutfitInfo.GetMaxNumberOfUsableOutfits() -> maxOutfitCount: number
```

### GetNextOutfitCost

```lua
C_TransmogOutfitInfo.GetNextOutfitCost() -> outfitCost: BigUInteger
```

### GetNumberOfOutfitsUnlockedForSource

```lua
C_TransmogOutfitInfo.GetNumberOfOutfitsUnlockedForSource(source: TransmogOutfitEntrySource) -> unlockedOutfitCount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetOptionsForSlot

```lua
C_TransmogOutfitInfo.GetOptionsForSlot(slot: TransmogOutfitSlot) -> options: TransmogOutfitOptionInfo[], artifactOptions: TransmogOutfitOptionInfo[]?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOutfitInfo

```lua
C_TransmogOutfitInfo.GetOutfitInfo(outfitID: number) -> outfitInfo: TransmogOutfitEntryInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOutfitInfoByName

```lua
C_TransmogOutfitInfo.GetOutfitInfoByName(name: cstring) -> outfitInfo: TransmogOutfitEntryInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | Case-insensitive outfit name to search for. If multiple exist with the same name, it is unspecified which outfit will be returned. |

### GetOutfitInfoByPlayerFacingIndex

```lua
C_TransmogOutfitInfo.GetOutfitInfoByPlayerFacingIndex(playerFacingOutfitIndex: number) -> outfitInfo: TransmogOutfitEntryInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetOutfitsInfo

```lua
C_TransmogOutfitInfo.GetOutfitsInfo() -> outfitsInfo: TransmogOutfitEntryInfo[]
```

`MayReturnNothing`

### GetOutfitSituation

```lua
C_TransmogOutfitInfo.GetOutfitSituation(option: TransmogSituationOption) -> value: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetOutfitSituationsEnabled

```lua
C_TransmogOutfitInfo.GetOutfitSituationsEnabled() -> enabled: bool
```

### GetPendingTransmogCost

```lua
C_TransmogOutfitInfo.GetPendingTransmogCost() -> cost: BigUInteger, modifierFlags: number
```

`MayReturnNothing`

### GetSecondarySlotState

```lua
C_TransmogOutfitInfo.GetSecondarySlotState(slot: TransmogOutfitSlot) -> state: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetSetSourcesForSlot

```lua
C_TransmogOutfitInfo.GetSetSourcesForSlot(transmogSetID: number, slot: TransmogOutfitSlot) -> sources: AppearanceSourceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSlotGroupInfo

```lua
C_TransmogOutfitInfo.GetSlotGroupInfo() -> slotGroups: TransmogOutfitSlotGroup[]
```

`MayReturnNothing`

### GetSourceIDsForSlot

```lua
C_TransmogOutfitInfo.GetSourceIDsForSlot(transmogSetID: number, slot: TransmogOutfitSlot) -> sources: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTransmogOutfitSlotForInventoryType

```lua
C_TransmogOutfitInfo.GetTransmogOutfitSlotForInventoryType(inventoryType: luaIndex) -> slot: TransmogOutfitSlot
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTransmogOutfitSlotFromInventorySlot

```lua
C_TransmogOutfitInfo.GetTransmogOutfitSlotFromInventorySlot(inventorySlot: InventorySlots) -> slot: TransmogOutfitSlot
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUISituationCategoriesAndOptions

```lua
C_TransmogOutfitInfo.GetUISituationCategoriesAndOptions() -> categoryData: TransmogSituationCategory[]
```

`MayReturnNothing`

### GetUnassignedAtlasForSlot

```lua
C_TransmogOutfitInfo.GetUnassignedAtlasForSlot(slot: TransmogOutfitSlot) -> atlas: textureAtlas
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUnassignedDisplayAtlasForSlot

```lua
C_TransmogOutfitInfo.GetUnassignedDisplayAtlasForSlot(slot: TransmogOutfitSlot) -> atlas: textureAtlas
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetViewedOutfitSlotInfo

```lua
C_TransmogOutfitInfo.GetViewedOutfitSlotInfo(slot: TransmogOutfitSlot, type: TransmogType, option: TransmogOutfitSlotOption) -> slotInfo: ViewedTransmogOutfitSlotInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasPendingOutfitSituations

```lua
C_TransmogOutfitInfo.HasPendingOutfitSituations() -> hasPending: bool
```

### HasPendingOutfitTransmogs

```lua
C_TransmogOutfitInfo.HasPendingOutfitTransmogs() -> hasPending: bool
```

### InTransmogEvent

```lua
C_TransmogOutfitInfo.InTransmogEvent() -> inTransmogEvent: bool
```

### IsEquippedGearOutfitDisplayed

```lua
C_TransmogOutfitInfo.IsEquippedGearOutfitDisplayed() -> isDisplayed: bool
```

### IsEquippedGearOutfitLocked

```lua
C_TransmogOutfitInfo.IsEquippedGearOutfitLocked() -> isLocked: bool
```

### IsLockedOutfit

```lua
C_TransmogOutfitInfo.IsLockedOutfit(outfitID: number) -> isLocked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSlotWeaponSlot

```lua
C_TransmogOutfitInfo.IsSlotWeaponSlot(slot: TransmogOutfitSlot) -> isWeaponSlot: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsTransmogEnabled

```lua
C_TransmogOutfitInfo.IsTransmogEnabled() -> enabled: bool
```

### IsUsableDiscountAvailable

```lua
C_TransmogOutfitInfo.IsUsableDiscountAvailable() -> isAvailable: bool
```

### IsValidTransmogOutfitName

```lua
C_TransmogOutfitInfo.IsValidTransmogOutfitName(name: cstring) -> isApproved: bool
```

`SecretArguments=AllowedWhenUntainted`

### PickupOutfit

```lua
C_TransmogOutfitInfo.PickupOutfit(outfitID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ResetOutfitSituations

```lua
C_TransmogOutfitInfo.ResetOutfitSituations()
```

### RevertPendingTransmog

```lua
C_TransmogOutfitInfo.RevertPendingTransmog(slot: TransmogOutfitSlot, type: TransmogType, option: TransmogOutfitSlotOption)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutfitSituationsEnabled

```lua
C_TransmogOutfitInfo.SetOutfitSituationsEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutfitToCustomSet

```lua
C_TransmogOutfitInfo.SetOutfitToCustomSet(transmogCustomSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutfitToOutfit

```lua
C_TransmogOutfitInfo.SetOutfitToOutfit(outfitID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutfitToSet

```lua
C_TransmogOutfitInfo.SetOutfitToSet(transmogSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPendingTransmog

```lua
C_TransmogOutfitInfo.SetPendingTransmog(slot: TransmogOutfitSlot, type: TransmogType, option: TransmogOutfitSlotOption, transmogID: number, displayType: TransmogOutfitDisplayType)
```

`SecretArguments=AllowedWhenUntainted`

### SetPendingTransmogSheatheCategory

```lua
C_TransmogOutfitInfo.SetPendingTransmogSheatheCategory(slot: TransmogOutfitSlot, option: TransmogOutfitSlotOption, category: TransmogOutfitSlotOptionSheatheCategory)
```

`SecretArguments=AllowedWhenUntainted`

### SetSecondarySlotState

```lua
C_TransmogOutfitInfo.SetSecondarySlotState(slot: TransmogOutfitSlot, state: bool)
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### SetViewedOptionForSlot

```lua
C_TransmogOutfitInfo.SetViewedOptionForSlot(slot: TransmogOutfitSlot, option: TransmogOutfitSlotOption)
```

`SecretArguments=AllowedWhenUntainted`

### SlotHasSecondary

```lua
C_TransmogOutfitInfo.SlotHasSecondary(slot: TransmogOutfitSlot) -> hasSecondary: bool
```

`SecretArguments=AllowedWhenUntainted`

### TransmogEventActive

```lua
C_TransmogOutfitInfo.TransmogEventActive() -> transmogEventActive: bool
```

### UpdatePendingSituation

```lua
C_TransmogOutfitInfo.UpdatePendingSituation(option: TransmogSituationOption, value: bool)
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### TRANSMOG_DISPLAYED_OUTFIT_CHANGED

```lua
TRANSMOG_DISPLAYED_OUTFIT_CHANGED()
```

`SynchronousEvent`

### TRANSMOG_OUTFITS_CHANGED

```lua
TRANSMOG_OUTFITS_CHANGED(newOutfitID: number?)
```

`SynchronousEvent`

### VIEWED_TRANSMOG_OUTFIT_CHANGED

```lua
VIEWED_TRANSMOG_OUTFIT_CHANGED()
```

`SynchronousEvent`

### VIEWED_TRANSMOG_OUTFIT_SECONDARY_SLOTS_CHANGED

```lua
VIEWED_TRANSMOG_OUTFIT_SECONDARY_SLOTS_CHANGED()
```

`SynchronousEvent`

### VIEWED_TRANSMOG_OUTFIT_SITUATIONS_CHANGED

```lua
VIEWED_TRANSMOG_OUTFIT_SITUATIONS_CHANGED()
```

`SynchronousEvent`

### VIEWED_TRANSMOG_OUTFIT_SLOT_OPTION_CHANGED

```lua
VIEWED_TRANSMOG_OUTFIT_SLOT_OPTION_CHANGED(slot: TransmogOutfitSlot, option: TransmogOutfitSlotOption)
```

`SynchronousEvent`

### VIEWED_TRANSMOG_OUTFIT_SLOT_REFRESH

```lua
VIEWED_TRANSMOG_OUTFIT_SLOT_REFRESH()
```

`UniqueEvent`

### VIEWED_TRANSMOG_OUTFIT_SLOT_SAVE_SUCCESS

```lua
VIEWED_TRANSMOG_OUTFIT_SLOT_SAVE_SUCCESS(slot: TransmogOutfitSlot, type: TransmogType, option: TransmogOutfitSlotOption)
```

`SynchronousEvent`

## Types

### TransmogOutfitCollectionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `isWeapon` | `bool` |  |
| `canHaveIllusions` | `bool` |  |

### TransmogOutfitEntryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `outfitID` | `number` |  |
| `name` | `string` |  |
| `situationCategories` | `cstring[]` |  |
| `icon` | `fileID` |  |
| `isEventOutfit` | `bool` |  |
| `isDisabled` | `bool` |  |
| `playerFacingOutfitIndex` | `number` |  |

### TransmogOutfitLinkedSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `primarySlotInfo` | `TransmogOutfitSlotInfo` |  |
| `secondarySlotInfo` | `TransmogOutfitSlotInfo` |  |

### TransmogOutfitOptionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `TransmogOutfitSlotOption` |  |
| `name` | `cstring` |  |
| `enabled` | `bool` |  |

### TransmogOutfitOptionSheatheCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `sheatheCategory` | `TransmogOutfitSlotOptionSheatheCategory` |  |
| `categoryName` | `cstring` |  |

### TransmogOutfitSlotGroup

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `position` | `TransmogOutfitSlotPosition` |  |
| `appearanceSlotInfo` | `TransmogOutfitSlotInfo[]` |  |
| `illusionSlotInfo` | `TransmogOutfitSlotInfo[]` |  |

### TransmogOutfitSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `slot` | `TransmogOutfitSlot` |  |
| `type` | `TransmogType` |  |
| `collectionType` | `TransmogCollectionType` |  |
| `slotName` | `cstring` |  |
| `isSecondary` | `bool` |  |

### TransmogSituationCategory

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `triggerID` | `number` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `isRadioButton` | `bool` |  |
| `groupData` | `TransmogSituationGroup[]` |  |

### TransmogSituationGroup

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `groupID` | `number` |  |
| `secondaryID` | `number` |  |
| `optionData` | `TransmogSituationOptionData[]` |  |

### TransmogSituationOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `situationID` | `number` |  |
| `specID` | `number` |  |
| `loadoutID` | `number` |  |
| `equipmentSetID` | `number` |  |

### TransmogSituationOptionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `value` | `bool` |  |
| `option` | `TransmogSituationOption` |  |

### ViewedTransmogOutfitSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `transmogID` | `number` |  |
| `displayType` | `TransmogOutfitDisplayType` |  |
| `isTransmogrified` | `bool` |  |
| `hasPending` | `bool` |  |
| `isPendingCollected` | `bool` |  |
| `canTransmogrify` | `bool` |  |
| `warning` | `TransmogOutfitSlotWarning` |  |
| `warningText` | `cstring` |  |
| `error` | `TransmogOutfitSlotError` |  |
| `errorText` | `cstring` |  |
| `texture` | `fileID?` |  |
| `sheatheCategory` | `TransmogOutfitSlotOptionSheatheCategory` |  |
