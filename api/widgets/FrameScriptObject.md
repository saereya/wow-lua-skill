# FrameScriptObject

Widget methods (`SimpleFrameScriptObjectAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleframescriptobjectapidocumentation.lua` (FileDataID 4637223)

## Methods

### AddAccessRestrictions

```lua
FrameScriptObject:AddAccessRestrictions(restrictions: ScriptObjectAccessRestriction)
```

Adds access restrictions to a script object, preventing it from being used in API calls when enforced.

`SecretArguments=NotAllowed` `HasRestrictions`

### AddForbiddenAspects

```lua
FrameScriptObject:AddForbiddenAspects(aspects: ForbiddenAspect)
```

Adds forbidden aspects to a script object, restricting access to various functionalities such as script bindings.

`SecretArguments=NotAllowed` `HasRestrictions`

### AddSecretAspect

```lua
FrameScriptObject:AddSecretAspect(aspect: SecretAspect)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `aspect` | `SecretAspect` | `NeverSecret` |

### CanBeAccessedInContext

```lua
FrameScriptObject:CanBeAccessedInContext() -> canAccess: bool
```

Returns whether the current Lua execution context has permission to access this object.

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `canAccess` | `bool` | False if access is denied, such as when execution is tainted and the object is forbidden or enforcing access restrictions. |

### GetAccessRestrictions

```lua
FrameScriptObject:GetAccessRestrictions() -> restrictions: ScriptObjectAccessRestriction
```

Returns the mask of all access restrictions applied to this object.

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### GetForbiddenAspects

```lua
FrameScriptObject:GetForbiddenAspects() -> aspects: ForbiddenAspect
```

Returns the mask of all forbidden aspects applied to this object.

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### GetInheritableForbiddenAspects

```lua
FrameScriptObject:GetInheritableForbiddenAspects(path: ScriptObjectPropagationPath) -> aspects: ForbiddenAspect
```

Returns the mask of all forbidden aspects applied to this object that can propagate to others.

`SecretArguments=NotAllowed` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### GetName

```lua
FrameScriptObject:GetName() -> name: cstring
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectName }`

### GetObjectTable

```lua
FrameScriptObject:GetObjectTable() -> objectTable: FrameScriptObject
```

### GetObjectType

```lua
FrameScriptObject:GetObjectType() -> objectType: cstring
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectType }`

### HasAccessConstraints

```lua
FrameScriptObject:HasAccessConstraints() -> hasAccessConstraints: bool
```

Returns whether this object has any access constraints that may limit access from some Lua execution contexts.

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `hasAccessConstraints` | `bool` | True if this object is forbidden or subject to conditional access restrictions. |

### HasAnyAccessRestrictions

```lua
FrameScriptObject:HasAnyAccessRestrictions(restrictions: ScriptObjectAccessRestriction?) -> hasAnyAccessRestriction: bool
```

Returns true if this object has any of the supplied access restrictions applied.

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### HasAnyForbiddenAspects

```lua
FrameScriptObject:HasAnyForbiddenAspects(aspects: ForbiddenAspect?) -> hasAnyForbiddenAspect: bool
```

Returns true if this object has any of the supplied forbidden aspects added.

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### HasAnySecretAspect

```lua
FrameScriptObject:HasAnySecretAspect() -> hasSecretAspect: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecrets }`

### HasSecretAspect

```lua
FrameScriptObject:HasSecretAspect(aspect: SecretAspect) -> hasSecretAspect: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecrets }` `ConstSecretAccessor`

### HasSecretValues

```lua
FrameScriptObject:HasSecretValues() -> hasSecretValues: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecrets }`

### IsForbidden

```lua
FrameScriptObject:IsForbidden() -> isForbidden: bool
```

Returns whether this object has been explicitly marked as forbidden.

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isForbidden` | `bool` | True if this object has been explicitly marked as forbidden, regardless of the current Lua execution context. |

### IsObjectType

```lua
FrameScriptObject:IsObjectType(objectType: cstring) -> isType: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectType }` `ConstSecretAccessor`

### IsPreventingSecretValues

```lua
FrameScriptObject:IsPreventingSecretValues() -> isPreventingSecretValues: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecrets }`

### SetForbidden

```lua
FrameScriptObject:SetForbidden()
```

`HasRestrictions`

### SetToDefaults

```lua
FrameScriptObject:SetToDefaults()
```

Reset all script accessible values to their default values. If possible, clears secret states.

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.
