# UI

Namespace `C_UI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uimanagerdocumentation.lua` (FileDataID 4637283)

## Functions

### DoesAnyDisplayHaveNotch

```lua
C_UI.DoesAnyDisplayHaveNotch() -> notchPresent: bool
```

True if any display attached has a notch. This does not mean the current view intersects the notch.

### GetTopLeftNotchSafeRegion

```lua
C_UI.GetTopLeftNotchSafeRegion() -> left: number, right: number, top: number, bottom: number
```

Region of screen left of screen notch. Zeros if no notch.

### GetTopRightNotchSafeRegion

```lua
C_UI.GetTopRightNotchSafeRegion() -> left: number, right: number, top: number, bottom: number
```

Region of screen right of screen notch. Zeros if no notch.

### GetUIParent

```lua
C_UI.GetUIParent() -> uiParent: SimpleFrame
```

### GetWorldFrame

```lua
C_UI.GetWorldFrame() -> worldFrame: SimpleFrame
```

### Reload

```lua
C_UI.Reload()
```

### ShouldUIParentAvoidNotch

```lua
C_UI.ShouldUIParentAvoidNotch() -> willAvoidNotch: bool
```

UIParent will shift down to avoid notch if true. This does not mean there is a notch.

## Events

### NOTCHED_DISPLAY_MODE_CHANGED

```lua
NOTCHED_DISPLAY_MODE_CHANGED()
```

`SynchronousEvent`

### UI_SCALE_CHANGED

```lua
UI_SCALE_CHANGED()
```

`SynchronousEvent`
