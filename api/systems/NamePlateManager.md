# NamePlateManager

Namespace `C_NamePlateManager` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/nameplatemanagerdocumentation.lua` (FileDataID 4637154)

## Functions

### GetNamePlateHitTestInsets

```lua
C_NamePlateManager.GetNamePlateHitTestInsets(type: NamePlateType) -> left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit
```

Returns the values used to adjust the hit testing area for nameplates.

`SecretArguments=AllowedWhenUntainted`

### IsNamePlateUnitBehindCamera

```lua
C_NamePlateManager.IsNamePlateUnitBehindCamera(unitToken: UnitTokenNamePlate) -> isBehindCamera: bool
```

Returns whether the unit to which the nameplate is attached is behind the player's camera.

`SecretArguments=AllowedWhenUntainted`

### SetNamePlateHitTestInsets

```lua
C_NamePlateManager.SetNamePlateHitTestInsets(type: NamePlateType, left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit)
```

Provide values to adjust the hit testing area for nameplates. Positive values will decrease the hit test area, negative values will increase it. Note that all hit testing is clamped to the bounds of the nameplate and can not be moved outside it.

`SecretArguments=NotAllowed` `HasRestrictions`

### SetNamePlateSimplified

```lua
C_NamePlateManager.SetNamePlateSimplified(unitToken: UnitTokenNamePlate, isSimplified: bool)
```

Set whether the nameplate attached to a unit is considered simplified, which can change the way it's displayed.

`SecretArguments=AllowedWhenUntainted`

## Events

### FORBIDDEN_NAME_PLATE_CREATED

```lua
FORBIDDEN_NAME_PLATE_CREATED(namePlateFrame: NamePlateFrame)
```

`SynchronousEvent`

### FORBIDDEN_NAME_PLATE_UNIT_ADDED

```lua
FORBIDDEN_NAME_PLATE_UNIT_ADDED(unitToken: UnitTokenType)
```

`SynchronousEvent`

### FORBIDDEN_NAME_PLATE_UNIT_REMOVED

```lua
FORBIDDEN_NAME_PLATE_UNIT_REMOVED(unitToken: UnitTokenType)
```

`SynchronousEvent`

### NAME_PLATE_CREATED

```lua
NAME_PLATE_CREATED(namePlateFrame: NamePlateFrame)
```

`SynchronousEvent`

### NAME_PLATE_UNIT_ADDED

```lua
NAME_PLATE_UNIT_ADDED(unitToken: UnitTokenType)
```

`SynchronousEvent`

### NAME_PLATE_UNIT_BEHIND_CAMERA_CHANGED

```lua
NAME_PLATE_UNIT_BEHIND_CAMERA_CHANGED(unitTarget: UnitTokenVariant, isBehindCamera: bool)
```

`SynchronousEvent`

### NAME_PLATE_UNIT_REMOVED

```lua
NAME_PLATE_UNIT_REMOVED(unitToken: UnitTokenType)
```

`SynchronousEvent`
