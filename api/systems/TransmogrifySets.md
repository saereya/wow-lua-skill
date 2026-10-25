# TransmogrifySets

Namespace `C_TransmogSets` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/transmogsetsdocumentation.lua` (FileDataID 4637278)

## Functions

### ClearLatestSource

```lua
C_TransmogSets.ClearLatestSource()
```

### ClearNewSource

```lua
C_TransmogSets.ClearNewSource(sourceID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ClearSetNewSourcesForSlot

```lua
C_TransmogSets.ClearSetNewSourcesForSlot(transmogSetID: number, slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetAllSets

```lua
C_TransmogSets.GetAllSets() -> sets: TransmogSetInfo[]
```

### GetAllSourceIDs

```lua
C_TransmogSets.GetAllSourceIDs(transmogSetID: number) -> sources: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAvailableSets

```lua
C_TransmogSets.GetAvailableSets() -> sets: TransmogSetInfo[]
```

### GetBaseSetID

```lua
C_TransmogSets.GetBaseSetID(transmogSetID: number) -> baseTransmogSetID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBaseSets

```lua
C_TransmogSets.GetBaseSets() -> sets: TransmogSetInfo[]
```

### GetBaseSetsFilter

```lua
C_TransmogSets.GetBaseSetsFilter(index: luaIndex) -> isChecked: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCameraIDs

```lua
C_TransmogSets.GetCameraIDs() -> detailsCameraID: number?, vendorCameraID: number?
```

### GetFilteredBaseSetsCounts

```lua
C_TransmogSets.GetFilteredBaseSetsCounts() -> numCollected: number, numTotal: number
```

### GetFullBaseSetsCounts

```lua
C_TransmogSets.GetFullBaseSetsCounts() -> numCollected: number, numTotal: number
```

### GetIsFavorite

```lua
C_TransmogSets.GetIsFavorite(transmogSetID: number) -> isFavorite: bool, isGroupFavorite: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLatestSource

```lua
C_TransmogSets.GetLatestSource() -> sourceID: number
```

### GetSetInfo

```lua
C_TransmogSets.GetSetInfo(transmogSetID: number) -> set: TransmogSetInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSetNewSources

```lua
C_TransmogSets.GetSetNewSources(transmogSetID: number) -> sourceIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSetPrimaryAppearances

```lua
C_TransmogSets.GetSetPrimaryAppearances(transmogSetID: number) -> apppearances: TransmogSetPrimaryAppearanceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSetsContainingSourceID

```lua
C_TransmogSets.GetSetsContainingSourceID(sourceID: number) -> setIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSetsFilter

```lua
C_TransmogSets.GetSetsFilter(index: luaIndex) -> isChecked: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourceIDsForSlot

```lua
C_TransmogSets.GetSourceIDsForSlot(transmogSetID: number, slot: luaIndex) -> sources: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourcesForSlot

```lua
C_TransmogSets.GetSourcesForSlot(transmogSetID: number, slot: luaIndex) -> sources: AppearanceSourceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTransmogSetsClassFilter

```lua
C_TransmogSets.GetTransmogSetsClassFilter() -> classID: number
```

### GetUsableSets

```lua
C_TransmogSets.GetUsableSets() -> sets: TransmogSetInfo[]
```

### GetValidBaseSetsCountsForCharacter

```lua
C_TransmogSets.GetValidBaseSetsCountsForCharacter() -> numCollected: number, numTotal: number
```

### GetValidClassForSet

```lua
C_TransmogSets.GetValidClassForSet(transmogSetID: number) -> classID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetVariantSets

```lua
C_TransmogSets.GetVariantSets(transmogSetID: number) -> sets: TransmogSetInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasAnyValidSets

```lua
C_TransmogSets.HasAnyValidSets() -> hasAnyValidSets: bool
```

### HasAvailableSets

```lua
C_TransmogSets.HasAvailableSets() -> hasAvailableSets: bool
```

### HasUsableSets

```lua
C_TransmogSets.HasUsableSets() -> hasUsableSets: bool
```

### IsBaseSetCollected

```lua
C_TransmogSets.IsBaseSetCollected(transmogSetID: number) -> isCollected: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsNewSource

```lua
C_TransmogSets.IsNewSource(sourceID: number) -> isNew: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSetVisible

```lua
C_TransmogSets.IsSetVisible(transmogSetID: number) -> isVisible: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultBaseSetsFilters

```lua
C_TransmogSets.IsUsingDefaultBaseSetsFilters() -> isUsingDefaultBaseSetsFilters: bool
```

### IsUsingDefaultSetsFilters

```lua
C_TransmogSets.IsUsingDefaultSetsFilters() -> isUsingDefaultSetsFilters: bool
```

### SetBaseSetsFilter

```lua
C_TransmogSets.SetBaseSetsFilter(index: luaIndex, isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultBaseSetsFilters

```lua
C_TransmogSets.SetDefaultBaseSetsFilters()
```

### SetDefaultSetsFilters

```lua
C_TransmogSets.SetDefaultSetsFilters()
```

### SetHasNewSources

```lua
C_TransmogSets.SetHasNewSources(transmogSetID: number) -> hasNewSources: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetHasNewSourcesForSlot

```lua
C_TransmogSets.SetHasNewSourcesForSlot(transmogSetID: number, slot: luaIndex) -> hasNewSources: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetIsFavorite

```lua
C_TransmogSets.SetIsFavorite(transmogSetID: number, isFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSetsFilter

```lua
C_TransmogSets.SetSetsFilter(index: luaIndex, isChecked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetTransmogSetsClassFilter

```lua
C_TransmogSets.SetTransmogSetsClassFilter(classID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### TransmogSetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `setID` | `number` |  |
| `name` | `string` |  |
| `baseSetID` | `number?` |  |
| `description` | `cstring?` |  |
| `label` | `cstring?` |  |
| `expansionID` | `number` |  |
| `patchID` | `number` |  |
| `uiOrder` | `number` |  |
| `classMask` | `number` |  |
| `hiddenUntilCollected` | `bool` |  |
| `requiredFaction` | `cstring?` |  |
| `collected` | `bool` |  |
| `favorite` | `bool` |  |
| `limitedTimeSet` | `bool` |  |
| `validForCharacter` | `bool` |  |
| `grantAsPrecedingVariant` | `bool` |  |

### TransmogSetPrimaryAppearanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `appearanceID` | `number` |  |
| `collected` | `bool` |  |
