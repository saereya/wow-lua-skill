# ClickBindings

Namespace `C_ClickBindings` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/clickbindingsdocumentation.lua` (FileDataID 4637056)

## Functions

### CanSpellBeClickBound

```lua
C_ClickBindings.CanSpellBeClickBound(spellID: SpellIdentifier) -> canBeBound: bool
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `SpellIdentifier` | Base spellID for spell, spellID for PetAction |

### ExecuteBinding

```lua
C_ClickBindings.ExecuteBinding(targetToken: cstring, button: cstring, modifiers: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetBindingType

```lua
C_ClickBindings.GetBindingType(button: cstring, modifiers: number) -> type: ClickBindingType
```

`SecretArguments=AllowedWhenUntainted`

### GetEffectiveInteractionButton

```lua
C_ClickBindings.GetEffectiveInteractionButton(button: cstring, modifiers: number) -> effectiveButton: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetProfileInfo

```lua
C_ClickBindings.GetProfileInfo() -> infoVec: ClickBindingInfo[]
```

### GetTutorialShown

```lua
C_ClickBindings.GetTutorialShown() -> tutorialShown: bool
```

### ResetCurrentProfile

```lua
C_ClickBindings.ResetCurrentProfile()
```

`HasRestrictions`

### SetProfileByInfo

```lua
C_ClickBindings.SetProfileByInfo(infoVec: ClickBindingInfo[])
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetTutorialShown

```lua
C_ClickBindings.SetTutorialShown()
```

## Events

### CLICKBINDINGS_SET_HIGHLIGHTS_SHOWN

```lua
CLICKBINDINGS_SET_HIGHLIGHTS_SHOWN(showHighlights: bool)
```

`SynchronousEvent`
