# KeyBindings

Namespace `C_KeyBindings` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/keybindingsdocumentation.lua` (FileDataID 4637125)

## Functions

### ActivateBindingContext

```lua
C_KeyBindings.ActivateBindingContext(newContext: BindingContext)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### DeactivateBindingContext

```lua
C_KeyBindings.DeactivateBindingContext(context: BindingContext)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetBindingByKey

```lua
C_KeyBindings.GetBindingByKey(action: cstring, context: BindingContext?) -> binding: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetBindingContextForAction

```lua
C_KeyBindings.GetBindingContextForAction(action: cstring) -> context: BindingContext?
```

`SecretArguments=AllowedWhenUntainted`

### GetBindingIndex

```lua
C_KeyBindings.GetBindingIndex(action: cstring) -> bindingIndex: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### GetCustomBindingType

```lua
C_KeyBindings.GetCustomBindingType(bindingIndex: luaIndex) -> customBindingType: CustomBindingType?
```

`SecretArguments=AllowedWhenUntainted`

### GetSearchTagsForAction

```lua
C_KeyBindings.GetSearchTagsForAction(action: cstring) -> searchTags: string[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetTurnStrafeStyle

```lua
C_KeyBindings.GetTurnStrafeStyle() -> style: TurnStrafeStyle
```

### IsBindingContextActive

```lua
C_KeyBindings.IsBindingContextActive(context: BindingContext) -> isActive: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTurnStrafeStyle

```lua
C_KeyBindings.SetTurnStrafeStyle(style: TurnStrafeStyle)
```

Can only set to Modern or Legacy.

`SecretArguments=AllowedWhenUntainted`

### UpdateTurnStrafeBindingsForCharacter

```lua
C_KeyBindings.UpdateTurnStrafeBindingsForCharacter()
```

## Events

### BINDINGS_LOADED

```lua
BINDINGS_LOADED()
```

`SynchronousEvent`

### MODIFIER_STATE_CHANGED

```lua
MODIFIER_STATE_CHANGED(key: cstring, down: number)
```

`SynchronousEvent`

### NOTIFY_TURN_STRAFE_CHANGE

```lua
NOTIFY_TURN_STRAFE_CHANGE()
```

`SynchronousEvent`

### UPDATE_BINDINGS

```lua
UPDATE_BINDINGS()
```

`SynchronousEvent`

## Types

### BindingContext

*Enumeration* · 10 values, 0..9

Access values as `Enum.BindingContext.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `BindingContext` | = 0 |
| `HousingEditor` | `BindingContext` | = 1 |
| `HousingEditorBasicDecorMode` | `BindingContext` | = 2 |
| `HousingEditorExpertDecorMode` | `BindingContext` | = 3 |
| `HousingEditorCustomizeMode` | `BindingContext` | = 4 |
| `HousingEditorCleanupMode` | `BindingContext` | = 5 |
| `HousingEditorLayoutMode` | `BindingContext` | = 6 |
| `HousingEditorBasicAndExpertDecorMode` | `BindingContext` | = 7 |
| `HousingEditorExteriorCustomizationMode` | `BindingContext` | = 8 |
| `GamepadModeInGameCore` | `BindingContext` | = 9 |

### BindingSet

*Enumeration* · 4 values, 0..3

Access values as `Enum.BindingSet.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `BindingSet` | = 0 |
| `Account` | `BindingSet` | = 1 |
| `Character` | `BindingSet` | = 2 |
| `Current` | `BindingSet` | = 3 |

### CustomBindingType

*Enumeration* · 1 values, 0..0

Access values as `Enum.CustomBindingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `VoicePushToTalk` | `CustomBindingType` | = 0 |

### TurnStrafeStyle

*Enumeration* · 3 values, 0..2

Access values as `Enum.TurnStrafeStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Modern` | `TurnStrafeStyle` | = 0 |
| `Legacy` | `TurnStrafeStyle` | = 1 |
| `Custom` | `TurnStrafeStyle` | = 2 |

### InputCommandCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `keystate` | `cstring` |  |
