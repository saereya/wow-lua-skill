# AssistedCombat

Namespace `C_AssistedCombat` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/assistedcombatdocumentation.lua` (FileDataID 6797329)

## Functions

### GetActionSpell

```lua
C_AssistedCombat.GetActionSpell() -> spellID: number?
```

### GetNextCastSpell

```lua
C_AssistedCombat.GetNextCastSpell(checkForVisibleButton: bool) -> spellID: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `checkForVisibleButton` | `bool` | default `false` |

### GetRotationSpells

```lua
C_AssistedCombat.GetRotationSpells() -> spellIDs: number[]
```

### IsAvailable

```lua
C_AssistedCombat.IsAvailable() -> isAvailable: bool, failureReason: string
```

## Events

### ASSISTED_COMBAT_ACTION_SPELL_CAST

```lua
ASSISTED_COMBAT_ACTION_SPELL_CAST()
```

`SynchronousEvent`
