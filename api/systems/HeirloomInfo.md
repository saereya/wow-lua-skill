# HeirloomInfo

Namespace `C_HeirloomInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/heirloominfodocumentation.lua` (FileDataID 4637143)

## Functions

### AreAllCollectionFiltersChecked

```lua
C_HeirloomInfo.AreAllCollectionFiltersChecked() -> areAllCollectionFiltersChecked: bool
```

### AreAllSourceFiltersChecked

```lua
C_HeirloomInfo.AreAllSourceFiltersChecked() -> areAllSourceFiltersChecked: bool
```

### HeirloomsAvailable

```lua
C_HeirloomInfo.HeirloomsAvailable() -> areHeirloomsAvailable: bool
```

### IsHeirloomSourceValid

```lua
C_HeirloomInfo.IsHeirloomSourceValid(source: luaIndex) -> isHeirloomSourceValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultFilters

```lua
C_HeirloomInfo.IsUsingDefaultFilters() -> isUsingDefaultFilters: bool
```

### SetAllCollectionFilters

```lua
C_HeirloomInfo.SetAllCollectionFilters(checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllSourceFilters

```lua
C_HeirloomInfo.SetAllSourceFilters(checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultFilters

```lua
C_HeirloomInfo.SetDefaultFilters()
```

## Events

### HEIRLOOMS_UPDATED

```lua
HEIRLOOMS_UPDATED(itemID: number?, updateReason: cstring?, hideUntilLearned: bool?)
```

`SynchronousEvent` `UniqueEvent`

### HEIRLOOM_UPGRADE_TARGETING_CHANGED

```lua
HEIRLOOM_UPGRADE_TARGETING_CHANGED(pendingHeirloomUpgradeSpellcast: bool)
```

`SynchronousEvent`
