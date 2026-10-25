# UIMacros

Namespace `C_Macro` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uimacrosdocumentation.lua` (FileDataID 4637281)

## Functions

### GetMacroName

```lua
C_Macro.GetMacroName(macroId: luaIndex) -> name: cstring?
```

`SecretArguments=AllowedWhenUntainted`

### GetSelectedMacroIcon

```lua
C_Macro.GetSelectedMacroIcon(macroId: luaIndex) -> textureNum: fileID
```

`SecretArguments=AllowedWhenUntainted`

### RunMacroText

```lua
C_Macro.RunMacroText(text: cstring, button: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetMacroExecuteLineCallback

```lua
C_Macro.SetMacroExecuteLineCallback(cb: MacroExecuteLineCallback)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### UPDATE_MACROS

```lua
UPDATE_MACROS()
```

`SynchronousEvent`

## Types

### MacroExecuteLineCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `macroLine` | `cstring` |  |
