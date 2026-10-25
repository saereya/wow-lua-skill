# Input

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/inputdocumentation.lua` (FileDataID 5200988)

## Functions

### GetCursorCenterPosition

```lua
GetCursorCenterPosition() -> posX: number, posY: number
```

### GetCursorDelta

```lua
GetCursorDelta() -> deltaX: number, deltaY: number
```

### GetCursorPosition

```lua
GetCursorPosition() -> posX: number, posY: number
```

### GetMouseButtonClicked

```lua
GetMouseButtonClicked() -> buttonName: cstring
```

### GetMouseButtonName

```lua
GetMouseButtonName(button: mouseButton) -> buttonName: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetMouseFoci

```lua
GetMouseFoci() -> region: ScriptRegion[]
```

### GetStringFromModifiers

```lua
GetStringFromModifiers(modifiers: number) -> modifierString: string
```

`SecretArguments=AllowedWhenUntainted`

### IsAltKeyDown

```lua
IsAltKeyDown() -> down: bool
```

### IsControlKeyDown

```lua
IsControlKeyDown() -> down: bool
```

### IsCursorVisible

```lua
IsCursorVisible() -> visible: bool
```

### IsKeyDown

```lua
IsKeyDown(keyOrMouseName: cstring, excludeBindingState: bool) -> down: bool?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `keyOrMouseName` | `cstring` |  |
| `excludeBindingState` | `bool` | default `false` |

### IsLeftAltKeyDown

```lua
IsLeftAltKeyDown() -> down: bool
```

### IsLeftControlKeyDown

```lua
IsLeftControlKeyDown() -> down: bool
```

### IsLeftMetaKeyDown

```lua
IsLeftMetaKeyDown() -> down: bool
```

### IsLeftShiftKeyDown

```lua
IsLeftShiftKeyDown() -> down: bool
```

### IsMetaKeyDown

```lua
IsMetaKeyDown() -> down: bool
```

### IsModifierKeyDown

```lua
IsModifierKeyDown() -> down: bool
```

### IsMouseButtonDown

```lua
IsMouseButtonDown(button: mouseButton?) -> down: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRightAltKeyDown

```lua
IsRightAltKeyDown() -> down: bool
```

### IsRightControlKeyDown

```lua
IsRightControlKeyDown() -> down: bool
```

### IsRightMetaKeyDown

```lua
IsRightMetaKeyDown() -> down: bool
```

### IsRightShiftKeyDown

```lua
IsRightShiftKeyDown() -> down: bool
```

### IsShiftKeyDown

```lua
IsShiftKeyDown() -> down: bool
```

### IsUsingGamepad

```lua
IsUsingGamepad() -> down: bool
```

### IsUsingMouse

```lua
IsUsingMouse() -> down: bool
```

### MakeModifiers

```lua
MakeModifiers() -> modifiers: number
```

### SetCursorPosition

```lua
SetCursorPosition(xPosition: uiUnit, yPosition: uiUnit)
```

Insecure code can only call this once in response to gamepad input hardware events.

`SecretArguments=AllowedWhenUntainted` `RequiresLimitedInput`

### SimulateMouseClick

```lua
SimulateMouseClick(button: mouseButton)
```

Effectively the same as SimulateMouseDown plus SimulateMouseUp and consumes limited input for both.

`SecretArguments=AllowedWhenUntainted` `RequiresLimitedInput` `MouseFocusValidForLimitedInput`

### SimulateMouseDown

```lua
SimulateMouseDown(button: mouseButton)
```

Insecure code can only call this once in response to gamepad input hardware events.

`SecretArguments=AllowedWhenUntainted` `RequiresLimitedInput` `MouseFocusValidForLimitedInput`

### SimulateMouseUp

```lua
SimulateMouseUp(button: mouseButton)
```

Insecure code can only call this once in response to gamepad input hardware events.

`SecretArguments=AllowedWhenUntainted` `RequiresLimitedInput` `MouseFocusValidForLimitedInput`

### SimulateMouseWheel

```lua
SimulateMouseWheel(delta: number)
```

Insecure code can only call this once in response to gamepad input hardware events.

`SecretArguments=AllowedWhenUntainted` `RequiresLimitedInput` `MouseFocusValidForLimitedInput`

## Events

### INPUT_DEVICE_INTERFACE_TRANSITION

```lua
INPUT_DEVICE_INTERFACE_TRANSITION(newMode: InputDeviceInterfaceType, oldMode: InputDeviceInterfaceType)
```

`SynchronousEvent`

## Predicates

Conditions referenced by the flags above.

- `MouseFocusValidForLimitedInput` *Precondition* (failure mode: ReturnNothing): Requires that all mouse foci are not forbidden, hidden from the global environment, fully locked down, script inaccessible, or protected frames (while in combat)
- `RequiresLimitedInput` *Precondition* (failure mode: Error)
