# PlayerInteractionManager

Namespace `C_PlayerInteractionManager` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playerinteractionmanagerdocumentation.lua` (FileDataID 4686648)

## Functions

### ClearInteraction

```lua
C_PlayerInteractionManager.ClearInteraction(type: PlayerInteractionType?)
```

`SecretArguments=AllowedWhenUntainted`

### ConfirmationInteraction

```lua
C_PlayerInteractionManager.ConfirmationInteraction(type: PlayerInteractionType?)
```

`SecretArguments=AllowedWhenUntainted`

### InteractUnit

```lua
C_PlayerInteractionManager.InteractUnit(unit: string, exactMatch: bool, looseTargeting: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unit` | `string` |  |
| `exactMatch` | `bool` | default `false` |
| `looseTargeting` | `bool` | default `true` |

### IsInteractingWithNpcOfType

```lua
C_PlayerInteractionManager.IsInteractingWithNpcOfType(type: PlayerInteractionType) -> interacting: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsReplacingUnit

```lua
C_PlayerInteractionManager.IsReplacingUnit() -> replacing: bool
```

### IsValidNPCInteraction

```lua
C_PlayerInteractionManager.IsValidNPCInteraction(type: PlayerInteractionType) -> isValidInteraction: bool
```

`SecretArguments=AllowedWhenUntainted`

### ReopenInteraction

```lua
C_PlayerInteractionManager.ReopenInteraction()
```

`HasRestrictions`

### ShardTransferConfirm

```lua
C_PlayerInteractionManager.ShardTransferConfirm()
```

## Events

### PLAYER_INTERACTION_MANAGER_FRAME_HIDE

```lua
PLAYER_INTERACTION_MANAGER_FRAME_HIDE(type: PlayerInteractionType)
```

`SynchronousEvent`

### PLAYER_INTERACTION_MANAGER_FRAME_SHOW

```lua
PLAYER_INTERACTION_MANAGER_FRAME_SHOW(type: PlayerInteractionType)
```

`SynchronousEvent`
