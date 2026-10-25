# EquipmentSet

Namespace `C_EquipmentSet` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/equipmentmanagerdocumentation.lua` (FileDataID 4637086)

## Functions

### AssignSpecToEquipmentSet

```lua
C_EquipmentSet.AssignSpecToEquipmentSet(equipmentSetID: number, specIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### CanUseEquipmentSets

```lua
C_EquipmentSet.CanUseEquipmentSets() -> canUseEquipmentSets: bool
```

### ClearIgnoredSlotsForSave

```lua
C_EquipmentSet.ClearIgnoredSlotsForSave()
```

### CreateEquipmentSet

```lua
C_EquipmentSet.CreateEquipmentSet(equipmentSetName: cstring, icon: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

### DeleteEquipmentSet

```lua
C_EquipmentSet.DeleteEquipmentSet(equipmentSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### EquipmentSetContainsLockedItems

```lua
C_EquipmentSet.EquipmentSetContainsLockedItems(equipmentSetID: number) -> hasLockedItems: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetEquipmentSetAssignedSpec

```lua
C_EquipmentSet.GetEquipmentSetAssignedSpec(equipmentSetID: number) -> specIndex: luaIndex
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEquipmentSetForSpec

```lua
C_EquipmentSet.GetEquipmentSetForSpec(specIndex: luaIndex) -> equipmentSetID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEquipmentSetID

```lua
C_EquipmentSet.GetEquipmentSetID(equipmentSetName: cstring) -> equipmentSetID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEquipmentSetIDs

```lua
C_EquipmentSet.GetEquipmentSetIDs() -> equipmentSetIDs: number[]
```

### GetEquipmentSetInfo

```lua
C_EquipmentSet.GetEquipmentSetInfo(equipmentSetID: number) -> name: string, iconFileID: number, setID: number, isEquipped: bool, numItems: number, numEquipped: number, numInInventory: number, numLost: number, numIgnored: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetIgnoredSlots

```lua
C_EquipmentSet.GetIgnoredSlots(equipmentSetID: number) -> slotIgnored: bool[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `slotIgnored` | `bool[]` | `NilableContents` |

### GetItemIDs

```lua
C_EquipmentSet.GetItemIDs(equipmentSetID: number) -> itemIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemIDs` | `number[]` | `NilableContents` |

### GetItemLocations

```lua
C_EquipmentSet.GetItemLocations(equipmentSetID: number) -> locations: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `locations` | `number[]` | `NilableContents` |

### GetNumEquipmentSets

```lua
C_EquipmentSet.GetNumEquipmentSets() -> numEquipmentSets: number
```

### IgnoreSlotForSave

```lua
C_EquipmentSet.IgnoreSlotForSave(slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### IsSlotIgnoredForSave

```lua
C_EquipmentSet.IsSlotIgnoredForSave(slot: luaIndex) -> isSlotIgnored: bool
```

`SecretArguments=AllowedWhenUntainted`

### ModifyEquipmentSet

```lua
C_EquipmentSet.ModifyEquipmentSet(equipmentSetID: number, newName: cstring, newIcon: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

### PickupEquipmentSet

```lua
C_EquipmentSet.PickupEquipmentSet(equipmentSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SaveEquipmentSet

```lua
C_EquipmentSet.SaveEquipmentSet(equipmentSetID: number, icon: cstring?)
```

`SecretArguments=AllowedWhenUntainted`

### UnassignEquipmentSetSpec

```lua
C_EquipmentSet.UnassignEquipmentSetSpec(equipmentSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### UnignoreSlotForSave

```lua
C_EquipmentSet.UnignoreSlotForSave(slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### UseEquipmentSet

```lua
C_EquipmentSet.UseEquipmentSet(equipmentSetID: number) -> setWasEquipped: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### EQUIPMENT_SETS_CHANGED

```lua
EQUIPMENT_SETS_CHANGED()
```

`SynchronousEvent`

### EQUIPMENT_SWAP_FINISHED

```lua
EQUIPMENT_SWAP_FINISHED(result: bool, setID: number?)
```

`SynchronousEvent`

### EQUIPMENT_SWAP_PENDING

```lua
EQUIPMENT_SWAP_PENDING()
```

`SynchronousEvent`

### TRANSMOG_CUSTOM_SETS_CHANGED

```lua
TRANSMOG_CUSTOM_SETS_CHANGED()
```

`SynchronousEvent`
