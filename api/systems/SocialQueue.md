# SocialQueue

Namespace `C_SocialQueue` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/socialqueuedocumentation.lua` (FileDataID 4637251)

## Functions

### GetAllGroups

```lua
C_SocialQueue.GetAllGroups(allowNonJoinable: bool, allowNonQueuedGroups: bool) -> groupGUIDs: WOWGUID[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `allowNonJoinable` | `bool` | default `false` |
| `allowNonQueuedGroups` | `bool` | default `false` |

### GetConfig

```lua
C_SocialQueue.GetConfig() -> config: SocialQueueConfig
```

`MayReturnNothing`

### GetGroupForPlayer

```lua
C_SocialQueue.GetGroupForPlayer(playerGUID: WOWGUID) -> groupGUID: WOWGUID, isSoloQueueParty: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGroupInfo

```lua
C_SocialQueue.GetGroupInfo(groupGUID: WOWGUID) -> canJoin: bool, numQueues: number, needTank: bool, needHealer: bool, needDamage: bool, isSoloQueueParty: bool, questSessionActive: bool, leaderGUID: WOWGUID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGroupMembers

```lua
C_SocialQueue.GetGroupMembers(groupGUID: WOWGUID) -> groupMembers: SocialQueuePlayerInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGroupQueues

```lua
C_SocialQueue.GetGroupQueues(groupGUID: WOWGUID) -> queues: SocialQueueGroupQueueInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### RequestToJoin

```lua
C_SocialQueue.RequestToJoin(groupGUID: WOWGUID, applyAsTank: bool, applyAsHealer: bool, applyAsDamage: bool) -> requestSuccessful: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `groupGUID` | `WOWGUID` |  |
| `applyAsTank` | `bool` | default `false` |
| `applyAsHealer` | `bool` | default `false` |
| `applyAsDamage` | `bool` | default `false` |

### SignalToastDisplayed

```lua
C_SocialQueue.SignalToastDisplayed(groupGUID: WOWGUID, priority: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SOCIAL_QUEUE_CONFIG_UPDATED

```lua
SOCIAL_QUEUE_CONFIG_UPDATED()
```

`SynchronousEvent`

### SOCIAL_QUEUE_UPDATE

```lua
SOCIAL_QUEUE_UPDATE(groupGUID: WOWGUID, numAddedItems: number?)
```

`SynchronousEvent`

## Types

### SocialQueueConfig

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `TOASTS_DISABLED` | `bool` |  |
| `TOAST_DURATION` | `number` |  |
| `DELAY_DURATION` | `number` |  |
| `QUEUE_MULTIPLIER` | `number` |  |
| `PLAYER_MULTIPLIER` | `number` |  |
| `PLAYER_FRIEND_VALUE` | `number` |  |
| `PLAYER_GUILD_VALUE` | `number` |  |
| `THROTTLE_INITIAL_THRESHOLD` | `number` |  |
| `THROTTLE_DECAY_TIME` | `number` |  |
| `THROTTLE_PRIORITY_SPIKE` | `number` |  |
| `THROTTLE_MIN_THRESHOLD` | `number` |  |
| `THROTTLE_PVP_PRIORITY_NORMAL` | `number` |  |
| `THROTTLE_PVP_PRIORITY_LOW` | `number` |  |
| `THROTTLE_PVP_HONOR_THRESHOLD` | `number` |  |
| `THROTTLE_LFGLIST_PRIORITY_DEFAULT` | `number` |  |
| `THROTTLE_LFGLIST_PRIORITY_ABOVE` | `number` |  |
| `THROTTLE_LFGLIST_PRIORITY_BELOW` | `number` |  |
| `THROTTLE_LFGLIST_ILVL_SCALING_ABOVE` | `number` |  |
| `THROTTLE_LFGLIST_ILVL_SCALING_BELOW` | `number` |  |
| `THROTTLE_RF_PRIORITY_ABOVE` | `number` |  |
| `THROTTLE_RF_ILVL_SCALING_ABOVE` | `number` |  |
| `THROTTLE_DF_MAX_ITEM_LEVEL` | `number` |  |
| `THROTTLE_DF_BEST_PRIORITY` | `number` |  |

### SocialQueueGroupInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `canJoin` | `bool` |  |
| `numQueues` | `number` |  |
| `needTank` | `bool` |  |
| `needHealer` | `bool` |  |
| `needDamage` | `bool` |  |
| `isSoloQueueParty` | `bool` |  |
| `questSessionActive` | `bool` |  |
| `leaderGUID` | `WOWGUID` |  |

### SocialQueueGroupQueueInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `clientID` | `number` |  |
| `eligible` | `bool` |  |
| `needTank` | `bool` |  |
| `needHealer` | `bool` |  |
| `needDamage` | `bool` |  |
| `isAutoAccept` | `bool` |  |
| `queueData` | `QueueSpecificInfo` |  |

### SocialQueuePlayerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `guid` | `WOWGUID` |  |
| `clubId` | `ClubId?` |  |
