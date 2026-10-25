# TargetScript

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/targetscriptdocumentation.lua` (FileDataID 5545762)

## Functions

### AssistUnit

```lua
AssistUnit(name: cstring, exactMatch: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `""` |
| `exactMatch` | `bool` | default `false` |

### AttackTarget

```lua
AttackTarget()
```

### ClearFocus

```lua
ClearFocus()
```

### ClearTarget

```lua
ClearTarget() -> willMakeChange: bool
```

### FocusUnit

```lua
FocusUnit(name: cstring)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `""` |

### IsTargetLoose

```lua
IsTargetLoose() -> isTargetLoose: bool
```

### SetPreferredGamepadInteractTarget

```lua
SetPreferredGamepadInteractTarget(unit: UnitToken?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### TargetDirectionEnemy

```lua
TargetDirectionEnemy(facing: number, coneAngle: number?)
```

`SecretArguments=AllowedWhenUntainted`

### TargetDirectionFinished

```lua
TargetDirectionFinished()
```

### TargetDirectionFriend

```lua
TargetDirectionFriend(facing: number, coneAngle: number?)
```

`SecretArguments=AllowedWhenUntainted`

### TargetLastEnemy

```lua
TargetLastEnemy()
```

### TargetLastFriend

```lua
TargetLastFriend()
```

### TargetLastTarget

```lua
TargetLastTarget()
```

### TargetNearest

```lua
TargetNearest(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestEnemy

```lua
TargetNearestEnemy(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestEnemyPlayer

```lua
TargetNearestEnemyPlayer(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestFriend

```lua
TargetNearestFriend(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestFriendPlayer

```lua
TargetNearestFriendPlayer(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestPartyMember

```lua
TargetNearestPartyMember(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetNearestRaidMember

```lua
TargetNearestRaidMember(reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `reverse` | `bool` | default `false` |

### TargetPriorityHighlightEnd

```lua
TargetPriorityHighlightEnd()
```

### TargetPriorityHighlightStart

```lua
TargetPriorityHighlightStart(useStartDelay: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `useStartDelay` | `bool` | default `false` |

### TargetToggle

```lua
TargetToggle()
```

`HasRestrictions`

### TargetUnit

```lua
TargetUnit(name: cstring, exactMatch: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` | default `""` |
| `exactMatch` | `bool` | default `false` |
