# LFGListRoles

Namespace `C_LFGListRoles` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lfglistrolesdocumentation.lua` (FileDataID 6225877)

## Functions

### GetRoles

```lua
C_LFGListRoles.GetRoles() -> roles: LFGRoles
```

`MayReturnNothing`

### GetSavedRoles

```lua
C_LFGListRoles.GetSavedRoles() -> roles: LFGRoles
```

`MayReturnNothing`

### SetRoles

```lua
C_LFGListRoles.SetRoles(roles: LFGRoles, limitToClassRoles: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `roles` | `LFGRoles` |  |
| `limitToClassRoles` | `bool` | default `false` |

## Events

### LFG_LIST_ROLE_UPDATE

```lua
LFG_LIST_ROLE_UPDATE()
```

`SynchronousEvent`
