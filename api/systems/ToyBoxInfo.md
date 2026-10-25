# ToyBoxInfo

Namespace `C_ToyBoxInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/toyboxinfodocumentation.lua` (FileDataID 4637264)

## Functions

### ClearFanfare

```lua
C_ToyBoxInfo.ClearFanfare(itemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### HasAnyToy

```lua
C_ToyBoxInfo.HasAnyToy() -> hasToy: bool
```

### IsToySourceValid

```lua
C_ToyBoxInfo.IsToySourceValid(source: luaIndex) -> isToySourceValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultFilters

```lua
C_ToyBoxInfo.IsUsingDefaultFilters() -> isUsingDefaultFilters: bool
```

### NeedsFanfare

```lua
C_ToyBoxInfo.NeedsFanfare(itemID: number) -> needsFanfare: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultFilters

```lua
C_ToyBoxInfo.SetDefaultFilters()
```

## Events

### NEW_TOY_ADDED

```lua
NEW_TOY_ADDED(itemID: number)
```

`SynchronousEvent`

### TOYS_UPDATED

```lua
TOYS_UPDATED(itemID: number?, isNew: bool?, hasFanfare: bool?)
```

`SynchronousEvent` `UniqueEvent`
