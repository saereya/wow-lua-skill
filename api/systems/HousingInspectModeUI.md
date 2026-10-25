# HousingInspectModeUI

Namespace `C_HousingInspectMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housinginspectmodeuidocumentation.lua` (FileDataID 7753903)

## Functions

### EnterInspectMode

```lua
C_HousingInspectMode.EnterInspectMode()
```

Enters inspect mode, enabling decor inspection

### ExitInspectMode

```lua
C_HousingInspectMode.ExitInspectMode()
```

Exits inspect mode, disabling decor inspection

### GetHoveredDecorGUID

```lua
C_HousingInspectMode.GetHoveredDecorGUID() -> decorGUID: WOWGUID
```

Returns the GUID of the decor instance currently being hovered, if there is one

### IsHoveringDecor

```lua
C_HousingInspectMode.IsHoveringDecor() -> isHoveringDecor: bool
```

Returns true if a decor instance is currently being hovered in inspect mode

### IsInInspectMode

```lua
C_HousingInspectMode.IsInInspectMode() -> isInInspectMode: bool
```

Returns true if the player is currently in inspect mode

## Events

### HOUSING_INSPECT_MODE_DECOR_HOVERED_CHANGED

```lua
HOUSING_INSPECT_MODE_DECOR_HOVERED_CHANGED()
```

`SynchronousEvent`

### HOUSING_INSPECT_MODE_STATE_UPDATED

```lua
HOUSING_INSPECT_MODE_STATE_UPDATED()
```

`SynchronousEvent`
