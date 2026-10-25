# NamePlate

Namespace `C_NamePlate` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/nameplatedocumentation.lua` (FileDataID 4637145)

## Functions

### GetNamePlateForUnit

```lua
C_NamePlate.GetNamePlateForUnit(unitToken: UnitTokenNamePlate, includeForbidden: bool) -> nameplate: NamePlateFrame
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unitToken` | `UnitTokenNamePlate` |  |
| `includeForbidden` | `bool` | default `false` |

### GetNamePlates

```lua
C_NamePlate.GetNamePlates() -> nameplates: NamePlateFrame[]
```

### GetNamePlateSize

```lua
C_NamePlate.GetNamePlateSize() -> width: uiUnit, height: uiUnit
```

### SetNamePlateSize

```lua
C_NamePlate.SetNamePlateSize(width: uiUnit, height: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`
