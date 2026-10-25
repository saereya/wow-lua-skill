# SpellDiminishUI

Namespace `C_SpellDiminish` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/spelldiminishuidocumentation.lua` (FileDataID 7506127)

## Functions

### GetAllSpellDiminishCategories

```lua
C_SpellDiminish.GetAllSpellDiminishCategories(ruleset: SpellDiminishRuleset?) -> categories: SpellDiminishCategoryInfo[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresSpellDiminishUI`

### GetSpellDiminishCategoryInfo

```lua
C_SpellDiminish.GetSpellDiminishCategoryInfo(category: SpellDiminishCategory) -> categoryInfo: SpellDiminishCategoryInfo?
```

`SecretArguments=AllowedWhenUntainted` `RequiresSpellDiminishUI`

### IsSystemSupported

```lua
C_SpellDiminish.IsSystemSupported() -> isSystemSupported: bool
```

### ShouldTrackSpellDiminishCategory

```lua
C_SpellDiminish.ShouldTrackSpellDiminishCategory(category: SpellDiminishCategory, ruleset: SpellDiminishRuleset) -> isTracked: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresSpellDiminishUI` `SecretReturns`

## Events

### UNIT_SPELL_DIMINISH_CATEGORY_STATE_UPDATED

```lua
UNIT_SPELL_DIMINISH_CATEGORY_STATE_UPDATED(unitTarget: UnitTokenVariant, trackerInfo: SpellDiminishTrackerInfo)
```

`SecretPayloads` `SynchronousEvent`

## Types

### SpellDiminishCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `category` | `SpellDiminishCategory` |  |
| `name` | `cstring` |  |
| `icon` | `fileID?` |  |

### SpellDiminishTrackerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `category` | `SpellDiminishCategory` |  |
| `startTime` | `number` |  |
| `duration` | `number` |  |
| `showCountdown` | `bool` |  |
| `isImmune` | `bool` |  |

## Predicates

Conditions referenced by the flags above.

- `RequiresSpellDiminishUI` *Precondition* (failure mode: ReturnNothing)
