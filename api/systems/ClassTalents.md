# ClassTalents

Namespace `C_ClassTalents` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/classtalentsdocumentation.lua` (FileDataID 4637046)

## Functions

### CanChangeTalents

```lua
C_ClassTalents.CanChangeTalents() -> canChange: bool, canAdd: bool, changeError: string?
```

Returns true only if the player has staged changes and can commit their talents in their current state.

### CanCreateNewConfig

```lua
C_ClassTalents.CanCreateNewConfig() -> canCreate: bool
```

### CanEditTalents

```lua
C_ClassTalents.CanEditTalents() -> canEdit: bool, changeError: cstring
```

Returns true if the player could switch talents if they staged a proper loadout.

### CommitConfig

```lua
C_ClassTalents.CommitConfig(savedConfigID: number?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### DeleteConfig

```lua
C_ClassTalents.DeleteConfig(configID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetActiveConfigID

```lua
C_ClassTalents.GetActiveConfigID() -> activeConfigID: number?
```

### GetActiveHeroTalentSpec

```lua
C_ClassTalents.GetActiveHeroTalentSpec() -> heroSpecID: number?
```

Returns the SubTreeID of the player's active Hero Talent Specialization SubTree.

Returns:

| Name | Type | Notes |
|---|---|---|
| `heroSpecID` | `number?` | SubTreeID of the player's active Hero Talent Specialization or nil if no Specialization is active. |

### GetConfigIDsBySpecID

```lua
C_ClassTalents.GetConfigIDsBySpecID(specID: number?) -> configIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetHasStarterBuild

```lua
C_ClassTalents.GetHasStarterBuild() -> hasStarterBuild: bool
```

### GetHeroTalentSpecsForClassSpec

```lua
C_ClassTalents.GetHeroTalentSpecsForClassSpec(configID: number?, classSpecID: number?) -> subTreeIDs: number[]?, requiredPlayerLevel: number?
```

Returns the SubTreeIDs of the Hero Talent Specializations available to a Class Specialization and config; Returns nothing if none available

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `configID` | `number?` | If not supplied, defaults to the player's active config |
| `classSpecID` | `number?` | If not supplied, defaults to the player's active spec |

Returns:

| Name | Type | Notes |
|---|---|---|
| `subTreeIDs` | `number[]?` | SubTreeIDs of each Hero Talent Specialization |
| `requiredPlayerLevel` | `number?` | The player level at which one of the Hero Talent Specializations can be activated |

### GetLastSelectedSavedConfigID

```lua
C_ClassTalents.GetLastSelectedSavedConfigID(specID: number) -> configID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetNextStarterBuildPurchase

```lua
C_ClassTalents.GetNextStarterBuildPurchase() -> nodeID: number?, entryID: number?
```

### GetStarterBuildActive

```lua
C_ClassTalents.GetStarterBuildActive() -> isActive: bool
```

### GetTraitTreeForSpec

```lua
C_ClassTalents.GetTraitTreeForSpec(specID: number) -> treeID: number?
```

`SecretArguments=AllowedWhenUntainted`

### HasUnspentHeroTalentPoints

```lua
C_ClassTalents.HasUnspentHeroTalentPoints() -> hasUnspentPoints: bool, numHeroPoints: number
```

Returns whether the player has any unspent talent points in their active hero talent tree. If hasUnspentPoints is true, numHeroPoints will be greater than zero.

### HasUnspentTalentPoints

```lua
C_ClassTalents.HasUnspentTalentPoints() -> hasUnspentPoints: bool, numClassPoints: number, numSpecPoints: number
```

Returns whether the player has any unspent talent points in their class or spec talent trees. If hasUnspentPoints is true, the number of unspent points for at least one of the trees will be greater than zero. Hero talent points are not included by this function.

### ImportLoadout

```lua
C_ClassTalents.ImportLoadout(configID: number, entries: ImportLoadoutEntryInfo[], name: string, importString: string?) -> success: bool, importError: cstring
```

`SecretArguments=AllowedWhenUntainted`

### InitializeViewLoadout

```lua
C_ClassTalents.InitializeViewLoadout(specID: number, level: number)
```

`SecretArguments=AllowedWhenUntainted`

### IsConfigPopulated

```lua
C_ClassTalents.IsConfigPopulated(configID: number) -> isPopulated: bool
```

New configs may or may not be populated and ready to load immediately after creation. Avoid calling for configs intentionally created empty.

`SecretArguments=AllowedWhenUntainted`

### LoadConfig

```lua
C_ClassTalents.LoadConfig(configID: number, autoApply: bool) -> result: LoadConfigResult, changeError: string?, newLearnedNodeIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### RenameConfig

```lua
C_ClassTalents.RenameConfig(configID: number, name: string) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestNewConfig

```lua
C_ClassTalents.RequestNewConfig(name: string) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SaveConfig

```lua
C_ClassTalents.SaveConfig(configID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetStarterBuildActive

```lua
C_ClassTalents.SetStarterBuildActive(active: bool) -> result: LoadConfigResult
```

`SecretArguments=AllowedWhenUntainted`

### SetUsesSharedActionBars

```lua
C_ClassTalents.SetUsesSharedActionBars(configID: number, usesShared: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SwitchToLoadoutByIndex

```lua
C_ClassTalents.SwitchToLoadoutByIndex(loadoutIndex: number)
```

Loads loadout for the current specialization by dropdown index. Indices start at 1.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SwitchToLoadoutByName

```lua
C_ClassTalents.SwitchToLoadoutByName(loadoutName: cstring)
```

Loads loadout for the current specialization by name. Loads the first one found in the case of duplicate names.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SwitchToSpecializationByIndex

```lua
C_ClassTalents.SwitchToSpecializationByIndex(specIndex: number)
```

Activates specialization for the current class by index in the order within the Specializations tab. Indices start at 1.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SwitchToSpecializationByName

```lua
C_ClassTalents.SwitchToSpecializationByName(specName: cstring)
```

Activates specialization for the current class by spec name.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### UpdateLastSelectedSavedConfigID

```lua
C_ClassTalents.UpdateLastSelectedSavedConfigID(specID: number, configID: number?)
```

`SecretArguments=AllowedWhenUntainted`

### ViewLoadout

```lua
C_ClassTalents.ViewLoadout(entries: ImportLoadoutEntryInfo[], importString: string?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACTIVE_COMBAT_CONFIG_CHANGED

```lua
ACTIVE_COMBAT_CONFIG_CHANGED(configID: number)
```

`SynchronousEvent`

### CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_INDEX

```lua
CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_INDEX(loadoutIndex: number)
```

`CallbackEvent`

### CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_NAME

```lua
CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_NAME(loadoutName: cstring)
```

`CallbackEvent`

### CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_INDEX

```lua
CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_INDEX(specIndex: number)
```

`CallbackEvent`

### CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_NAME

```lua
CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_NAME(specName: cstring)
```

`CallbackEvent`

### SELECTED_LOADOUT_CHANGED

```lua
SELECTED_LOADOUT_CHANGED()
```

`SynchronousEvent`

### SPECIALIZATION_CHANGE_CAST_FAILED

```lua
SPECIALIZATION_CHANGE_CAST_FAILED()
```

`SynchronousEvent`

### STARTER_BUILD_ACTIVATION_FAILED

```lua
STARTER_BUILD_ACTIVATION_FAILED()
```

`SynchronousEvent`

## Types

### LoadConfigResult

*Enumeration* · 4 values, 0..3

Access values as `Enum.LoadConfigResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Error` | `LoadConfigResult` | = 0 |
| `NoChangesNecessary` | `LoadConfigResult` | = 1 |
| `LoadInProgress` | `LoadConfigResult` | = 2 |
| `Ready` | `LoadConfigResult` | = 3 |

### ImportLoadoutEntryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `nodeID` | `number` |  |
| `ranksGranted` | `number` |  |
| `ranksPurchased` | `number` |  |
| `selectionEntryID` | `number` |  |
