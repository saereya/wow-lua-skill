# MountJournal

Namespace `C_MountJournal` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mountjournaldocumentation.lua` (FileDataID 4637144)

## Functions

### ApplyMountEquipment

```lua
C_MountJournal.ApplyMountEquipment(itemLocation: ItemLocation) -> canContinue: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### AreMountEquipmentEffectsSuppressed

```lua
C_MountJournal.AreMountEquipmentEffectsSuppressed() -> areEffectsSuppressed: bool
```

### ClearFanfare

```lua
C_MountJournal.ClearFanfare(mountID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ClearRecentFanfares

```lua
C_MountJournal.ClearRecentFanfares()
```

### Dismiss

```lua
C_MountJournal.Dismiss()
```

### GetAllCreatureDisplayIDsForMountID

```lua
C_MountJournal.GetAllCreatureDisplayIDsForMountID(mountID: number) -> creatureDisplayIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAppliedMountEquipmentID

```lua
C_MountJournal.GetAppliedMountEquipmentID() -> itemID: number?
```

### GetCollectedDragonridingMounts

```lua
C_MountJournal.GetCollectedDragonridingMounts() -> mountIDs: number[]
```

### GetCollectedFilterSetting

```lua
C_MountJournal.GetCollectedFilterSetting(filterIndex: luaIndex) -> isChecked: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayedMountAllCreatureDisplayInfo

```lua
C_MountJournal.GetDisplayedMountAllCreatureDisplayInfo(mountIndex: luaIndex) -> allDisplayInfo: MountCreatureDisplayInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDisplayedMountID

```lua
C_MountJournal.GetDisplayedMountID(displayIndex: luaIndex) -> mountID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetDisplayedMountInfo

```lua
C_MountJournal.GetDisplayedMountInfo(displayIndex: luaIndex) -> name: cstring, spellID: number, icon: fileID, isActive: bool, isUsable: bool, sourceType: number, isFavorite: bool, isFactionSpecific: bool, faction: PvPFaction?, shouldHideOnChar: bool, isCollected: bool, mountID: number, isSteadyFlight: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDisplayedMountInfoExtra

```lua
C_MountJournal.GetDisplayedMountInfoExtra(mountIndex: luaIndex) -> creatureDisplayInfoID: number?, description: cstring, source: cstring, isSelfMount: bool, mountTypeID: number, uiModelSceneID: number, animID: number, spellVisualKitID: number, disablePlayerMountPreview: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDynamicFlightModeSpellID

```lua
C_MountJournal.GetDynamicFlightModeSpellID() -> spellID: number
```

### GetIsFavorite

```lua
C_MountJournal.GetIsFavorite(mountIndex: luaIndex) -> isFavorite: bool, canSetFavorite: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetMountAllCreatureDisplayInfoByID

```lua
C_MountJournal.GetMountAllCreatureDisplayInfoByID(mountID: number) -> allDisplayInfo: MountCreatureDisplayInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMountEquipmentUnlockLevel

```lua
C_MountJournal.GetMountEquipmentUnlockLevel() -> level: number
```

### GetMountFromItem

```lua
C_MountJournal.GetMountFromItem(itemID: number) -> mountID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetMountFromSpell

```lua
C_MountJournal.GetMountFromSpell(spellID: SpellIdentifier) -> mountID: number?
```

`SecretArguments=AllowedWhenTainted`

### GetMountIDs

```lua
C_MountJournal.GetMountIDs() -> mountIDs: number[]
```

### GetMountInfoByID

```lua
C_MountJournal.GetMountInfoByID(mountID: number) -> name: cstring, spellID: number, icon: fileID, isActive: bool, isUsable: bool, sourceType: number, isFavorite: bool, isFactionSpecific: bool, faction: PvPFaction?, shouldHideOnChar: bool, isCollected: bool, mountID: number, isSteadyFlight: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMountInfoExtraByID

```lua
C_MountJournal.GetMountInfoExtraByID(mountID: number) -> creatureDisplayInfoID: number?, description: cstring, source: cstring, isSelfMount: bool, mountTypeID: number, uiModelSceneID: number, animID: number, spellVisualKitID: number, disablePlayerMountPreview: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMountLink

```lua
C_MountJournal.GetMountLink(spellID: number) -> mountCreatureDisplayInfoLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetMountUsabilityByID

```lua
C_MountJournal.GetMountUsabilityByID(mountID: number, checkIndoors: bool) -> isUsable: bool, useError: cstring?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetNumDisplayedMounts

```lua
C_MountJournal.GetNumDisplayedMounts() -> numMounts: number
```

### GetNumMounts

```lua
C_MountJournal.GetNumMounts() -> numMounts: number
```

### GetNumMountsNeedingFanfare

```lua
C_MountJournal.GetNumMountsNeedingFanfare() -> numMountsNeedingFanfare: number
```

### HasDisplayableMount

```lua
C_MountJournal.HasDisplayableMount() -> hasMount: bool
```

### IsDragonridingUnlocked

```lua
C_MountJournal.IsDragonridingUnlocked() -> isUnlocked: bool
```

Returns whether the player has unlocked the ability to switch between Skyriding and steady flight styles for flying mounts .

### IsItemMountEquipment

```lua
C_MountJournal.IsItemMountEquipment(itemLocation: ItemLocation) -> isMountEquipment: bool
```

Determines if the item is mount equipment based on its class and subclass.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsMountEquipmentApplied

```lua
C_MountJournal.IsMountEquipmentApplied() -> isApplied: bool
```

### IsSourceChecked

```lua
C_MountJournal.IsSourceChecked(filterIndex: luaIndex) -> isChecked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsTypeChecked

```lua
C_MountJournal.IsTypeChecked(filterIndex: luaIndex) -> isChecked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultFilters

```lua
C_MountJournal.IsUsingDefaultFilters() -> isUsingDefaultFilters: bool
```

### IsValidSourceFilter

```lua
C_MountJournal.IsValidSourceFilter(filterIndex: luaIndex) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidTypeFilter

```lua
C_MountJournal.IsValidTypeFilter(filterIndex: luaIndex) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### MountEquipmentAvailable

```lua
C_MountJournal.MountEquipmentAvailable() -> isMountEquipmentAvailable: bool
```

### NeedsFanfare

```lua
C_MountJournal.NeedsFanfare(mountID: number) -> needsFanfare: bool
```

`SecretArguments=AllowedWhenUntainted`

### Pickup

```lua
C_MountJournal.Pickup(displayIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### PickupDynamicFlightMode

```lua
C_MountJournal.PickupDynamicFlightMode()
```

### SetAllSourceFilters

```lua
C_MountJournal.SetAllSourceFilters(isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllTypeFilters

```lua
C_MountJournal.SetAllTypeFilters(isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCollectedFilterSetting

```lua
C_MountJournal.SetCollectedFilterSetting(filterIndex: luaIndex, isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultFilters

```lua
C_MountJournal.SetDefaultFilters()
```

### SetIsFavorite

```lua
C_MountJournal.SetIsFavorite(mountIndex: luaIndex, isFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearch

```lua
C_MountJournal.SetSearch(searchValue: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetSourceFilter

```lua
C_MountJournal.SetSourceFilter(filterIndex: luaIndex, isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetTypeFilter

```lua
C_MountJournal.SetTypeFilter(filterIndex: luaIndex, isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SummonByID

```lua
C_MountJournal.SummonByID(mountID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SwapDynamicFlightMode

```lua
C_MountJournal.SwapDynamicFlightMode()
```

## Events

### MOUNT_EQUIPMENT_APPLY_RESULT

```lua
MOUNT_EQUIPMENT_APPLY_RESULT(success: bool)
```

`SynchronousEvent`

### MOUNT_JOURNAL_SEARCH_UPDATED

```lua
MOUNT_JOURNAL_SEARCH_UPDATED()
```

`SynchronousEvent`

### MOUNT_JOURNAL_USABILITY_CHANGED

```lua
MOUNT_JOURNAL_USABILITY_CHANGED()
```

`SynchronousEvent`

### NEW_MOUNT_ADDED

```lua
NEW_MOUNT_ADDED(mountID: number)
```

`SynchronousEvent`

## Types

### MountCreatureDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureDisplayID` | `number` |  |
| `isVisible` | `bool` |  |

### MountInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `spellID` | `number` |  |
| `icon` | `fileID` |  |
| `isActive` | `bool` |  |
| `isUsable` | `bool` |  |
| `sourceType` | `number` |  |
| `isFavorite` | `bool` |  |
| `isFactionSpecific` | `bool` |  |
| `faction` | `PvPFaction?` |  |
| `shouldHideOnChar` | `bool` |  |
| `isCollected` | `bool` |  |
| `mountID` | `number` |  |
| `isSteadyFlight` | `bool` |  |

### MountInfoExtra

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureDisplayInfoID` | `number?` |  |
| `description` | `cstring` |  |
| `source` | `cstring` |  |
| `isSelfMount` | `bool` |  |
| `mountTypeID` | `number` |  |
| `uiModelSceneID` | `number` |  |
| `animID` | `number` |  |
| `spellVisualKitID` | `number` |  |
| `disablePlayerMountPreview` | `bool` |  |
