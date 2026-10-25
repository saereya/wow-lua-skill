# CVarScripts

Namespace `C_CVar` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/cvardocumentation.lua` (FileDataID 4637082)

## Functions

### AreCVarsLoaded

```lua
C_CVar.AreCVarsLoaded() -> loaded: bool
```

### GetCVar

```lua
C_CVar.GetCVar(name: cstring) -> value: string?
```

`SecretArguments=NotAllowed`

### GetCVarBitfield

```lua
C_CVar.GetCVarBitfield(name: cstring, index: luaIndex) -> value: bool?
```

`SecretArguments=NotAllowed`

### GetCVarBool

```lua
C_CVar.GetCVarBool(name: cstring) -> value: bool?
```

`SecretArguments=NotAllowed`

### GetCVarDefault

```lua
C_CVar.GetCVarDefault(name: cstring) -> defaultValue: string?
```

`SecretArguments=NotAllowed` `RequiresValidAndPublicCVar`

### GetCVarInfo

```lua
C_CVar.GetCVarInfo(name: cstring) -> value: cstring, defaultValue: cstring, isStoredServerAccount: bool, isStoredServerCharacter: bool, isLockedFromUser: bool, isSecure: bool, isReadOnly: bool
```

`SecretArguments=NotAllowed`

### RegisterCVar

```lua
C_CVar.RegisterCVar(name: cstring, value: cstring?)
```

`SecretArguments=NotAllowed`

### RemoveTempCVar

```lua
C_CVar.RemoveTempCVar(name: cstring)
```

`SecretArguments=NotAllowed` `RequiresValidAndPublicCVar` `RequiresNonReadOnlyCVar` `RequiresNonSecureCVar`

### ResetTestCVars

```lua
C_CVar.ResetTestCVars()
```

### SetCVar

```lua
C_CVar.SetCVar(name: cstring, value: cstring?) -> success: bool
```

`SecretArguments=NotAllowed` `RequiresValidAndPublicCVar` `RequiresNonReadOnlyCVar` `RequiresNonSecureCVar`

### SetCVarBitfield

```lua
C_CVar.SetCVarBitfield(name: cstring, index: luaIndex, value: bool) -> success: bool
```

`SecretArguments=NotAllowed` `RequiresValidAndPublicCVar` `RequiresNonReadOnlyCVar` `RequiresNonSecureCVar` `RequiresIndexInRange`

### SetTempCVar

```lua
C_CVar.SetTempCVar(name: cstring, value: cstring?)
```

`SecretArguments=NotAllowed` `RequiresValidAndPublicCVar` `RequiresNonReadOnlyCVar` `RequiresNonSecureCVar`

## Types

### CVarInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `value` | `cstring` |  |
| `defaultValue` | `cstring` |  |
| `isStoredServerAccount` | `bool` |  |
| `isStoredServerCharacter` | `bool` |  |
| `isLockedFromUser` | `bool` |  |
| `isSecure` | `bool` |  |
| `isReadOnly` | `bool` |  |

## Predicates

Conditions referenced by the flags above.

- `RequiresIndexInRange` *Precondition* (failure mode: Error)
- `RequiresNonReadOnlyCVar` *Precondition* (failure mode: ReturnNothing)
- `RequiresNonSecureCVar` *Precondition* (failure mode: ReturnNothing)
- `RequiresValidAndPublicCVar` *Precondition* (failure mode: ReturnNothing)
