# CooldownViewer

Namespace `C_CooldownViewer` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/cooldownviewerdocumentation.lua` (FileDataID 6438302)

## Functions

### GetCooldownViewerCategorySet

```lua
C_CooldownViewer.GetCooldownViewerCategorySet(category: CooldownViewerCategory, allowUnlearned: bool) -> cooldownIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `category` | `CooldownViewerCategory` |  |
| `allowUnlearned` | `bool` | default `false` |

### GetCooldownViewerCooldownInfo

```lua
C_CooldownViewer.GetCooldownViewerCooldownInfo(cooldownID: number) -> cooldownInfo: CooldownViewerCooldown
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGroupBuffItems

```lua
C_CooldownViewer.GetGroupBuffItems() -> groupBuffItems: GroupBuffItem[]
```

### GetLayoutData

```lua
C_CooldownViewer.GetLayoutData() -> data: cstring
```

### GetValidAlertTypes

```lua
C_CooldownViewer.GetValidAlertTypes(cooldownID: number) -> validAlertTypes: CooldownViewerAlertEventType[]
```

`SecretArguments=AllowedWhenUntainted`

### IsCooldownViewerAvailable

```lua
C_CooldownViewer.IsCooldownViewerAvailable() -> isAvailable: bool, failureReason: string
```

### SetLayoutData

```lua
C_CooldownViewer.SetLayoutData(data: cstring)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### COOLDOWN_VIEWER_DATA_LOADED

```lua
COOLDOWN_VIEWER_DATA_LOADED()
```

`SynchronousEvent`

### COOLDOWN_VIEWER_SPELL_OVERRIDE_UPDATED

```lua
COOLDOWN_VIEWER_SPELL_OVERRIDE_UPDATED(baseSpellID: number, overrideSpellID: number?)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `baseSpellID` | `number` | The base spell that is either being overridden or losing its override spell. |
| `overrideSpellID` | `number?` | The spell overriding the base spell. A nil value indicates that the override spell is being removed from the base spell. |

### COOLDOWN_VIEWER_TABLE_HOTFIXED

```lua
COOLDOWN_VIEWER_TABLE_HOTFIXED()
```

`SynchronousEvent`

## Types

### CooldownViewerCooldown

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `cooldownID` | `number` |  |
| `spellID` | `number?` |  |
| `spellCategoryID` | `number?` |  |
| `overrideSpellID` | `number?` |  |
| `overrideTooltipSpellID` | `number?` |  |
| `equipSlot` | `luaIndex?` |  |
| `buffSlot` | `luaIndex?` |  |
| `linkedSpellIDs` | `number[]` |  |
| `selfAura` | `bool` |  |
| `hasAura` | `bool` |  |
| `charges` | `bool` |  |
| `isKnown` | `bool` |  |
| `isInvisible` | `bool` |  |
| `flags` | `CooldownSetSpellFlags` |  |
| `category` | `CooldownViewerCategory` |  |

### GroupBuffItem

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` | The persisted key for this item, shared by every rank of the spell. |
| `displaySpellID` | `number` | The spell used for name, icon and tooltip: the highest known rank, or the lowest rank if none are known. |
| `name` | `cstring` |  |
| `iconID` | `fileID` |  |
| `flags` | `GroupBuffItemFlags` |  |
| `isKnown` | `bool` |  |
