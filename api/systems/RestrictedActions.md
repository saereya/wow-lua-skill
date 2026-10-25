# RestrictedActions

Namespace `C_RestrictedActions` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/restrictedactionsdocumentation.lua` (FileDataID 4637191)

## Functions

### CheckAllowProtectedFunctions

```lua
C_RestrictedActions.CheckAllowProtectedFunctions(object: FrameScriptObject, silent: bool) -> protectedFunctionsAllowed: bool
```

Returns true if the calling context has permissions to call protected functions on the supplied object.

`SecretArguments=AllowedWhenUntainted` `SecureHooksAllowed=False`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `object` | `FrameScriptObject` |  |
| `silent` | `bool` | default `false`; If true, don't signal blocked action errors if protected function calls are disallowed. |

### GetAddOnRestrictionState

```lua
C_RestrictedActions.GetAddOnRestrictionState(type: AddOnRestrictionType) -> state: AddOnRestrictionState
```

Returns the current state of an addon restriction type.

`SecretArguments=AllowedWhenUntainted`

### InCombatLockdown

```lua
C_RestrictedActions.InCombatLockdown() -> inCombatLockdown: bool
```

`Namespace=`

### IsAddOnRestrictionActive

```lua
C_RestrictedActions.IsAddOnRestrictionActive(type: AddOnRestrictionType) -> active: bool
```

Returns true if an addon restriction type is in an active state. Will always return false during dispatch of ADDON_RESTRICTION_STATE_CHANGED.

`SecretArguments=AllowedWhenUntainted`

## Events

### ADDON_ACTION_BLOCKED

```lua
ADDON_ACTION_BLOCKED(isTainted: cstring, function: cstring)
```

`SynchronousEvent`

### ADDON_ACTION_FORBIDDEN

```lua
ADDON_ACTION_FORBIDDEN(isTainted: cstring, function: cstring)
```

`SynchronousEvent`

### ADDON_RESTRICTION_STATE_CHANGED

```lua
ADDON_RESTRICTION_STATE_CHANGED(type: AddOnRestrictionType, state: AddOnRestrictionState)
```

Fired when the state of an addon restriction type is changing. This event is sequenced such that it will always be fired before a restriction becomes active, or after it is deactivated.

`SynchronousEvent`

### MACRO_ACTION_BLOCKED

```lua
MACRO_ACTION_BLOCKED(function: cstring)
```

`SynchronousEvent`

### MACRO_ACTION_FORBIDDEN

```lua
MACRO_ACTION_FORBIDDEN(function: cstring)
```

`SynchronousEvent`
