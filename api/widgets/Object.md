# Object

Widget methods (`SimpleObjectAPI`) · inherits [`FrameScriptObject`](FrameScriptObject.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleobjectapidocumentation.lua` (FileDataID 4637235)

## Methods

### ClearParentKey

```lua
Object:ClearParentKey()
```

### GetDebugName

```lua
Object:GetDebugName(preferParentKey: bool) -> debugName: string
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `preferParentKey` | `bool` | default `false` |

### GetParent

```lua
Object:GetParent() -> parent: CScriptObject
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

### GetParentKey

```lua
Object:GetParentKey() -> parentKey: cstring
```

### SetParentKey

```lua
Object:SetParentKey(parentKey: cstring, clearOtherKeys: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `parentKey` | `cstring` |  |
| `clearOtherKeys` | `bool` | default `false` |
