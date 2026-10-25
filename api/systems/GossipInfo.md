# GossipInfo

Namespace `C_GossipInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gossipinfodocumentation.lua` (FileDataID 4637095)

## Functions

### CloseGossip

```lua
C_GossipInfo.CloseGossip()
```

### ForceGossip

```lua
C_GossipInfo.ForceGossip() -> forceGossip: bool
```

### GetActiveQuests

```lua
C_GossipInfo.GetActiveQuests() -> info: GossipQuestUIInfo[]
```

### GetAvailableQuests

```lua
C_GossipInfo.GetAvailableQuests() -> info: GossipQuestUIInfo[]
```

### GetCompletedOptionDescriptionString

```lua
C_GossipInfo.GetCompletedOptionDescriptionString() -> description: string?
```

### GetCustomGossipDescriptionString

```lua
C_GossipInfo.GetCustomGossipDescriptionString() -> description: string?
```

### GetFriendshipReputation

```lua
C_GossipInfo.GetFriendshipReputation(friendshipFactionID: number) -> reputationInfo: FriendshipReputationInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFriendshipReputationRanks

```lua
C_GossipInfo.GetFriendshipReputationRanks(friendshipFactionID: number) -> rankInfo: FriendshipReputationRankInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetNumActiveQuests

```lua
C_GossipInfo.GetNumActiveQuests() -> numQuests: number
```

### GetNumAvailableQuests

```lua
C_GossipInfo.GetNumAvailableQuests() -> numQuests: number
```

### GetOptions

```lua
C_GossipInfo.GetOptions() -> info: GossipOptionUIInfo[]
```

### GetOptionUIWidgetSetsAndTypesByOptionID

```lua
C_GossipInfo.GetOptionUIWidgetSetsAndTypesByOptionID(gossipOptionID: number) -> gossipOptionUIWidgetSetsAndTypes: GossipOptionUIWidgetSetAndType[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetPoiForUiMapID

```lua
C_GossipInfo.GetPoiForUiMapID(uiMapID: number) -> gossipPoiID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetPoiInfo

```lua
C_GossipInfo.GetPoiInfo(uiMapID: number, gossipPoiID: number) -> gossipPoiInfo: GossipPoiInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetText

```lua
C_GossipInfo.GetText() -> gossipText: cstring
```

### RefreshOptions

```lua
C_GossipInfo.RefreshOptions()
```

### SelectActiveQuest

```lua
C_GossipInfo.SelectActiveQuest(optionID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SelectAvailableQuest

```lua
C_GossipInfo.SelectAvailableQuest(optionID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SelectOption

```lua
C_GossipInfo.SelectOption(optionID: number, text: cstring?, confirmed: bool?)
```

`SecretArguments=AllowedWhenUntainted`

### SelectOptionByIndex

```lua
C_GossipInfo.SelectOptionByIndex(optionID: number, text: cstring?, confirmed: bool?)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### DYNAMIC_GOSSIP_POI_UPDATED

```lua
DYNAMIC_GOSSIP_POI_UPDATED()
```

`UniqueEvent`

### GOSSIP_CLOSED

```lua
GOSSIP_CLOSED(interactionIsContinuing: bool)
```

`SynchronousEvent`

### GOSSIP_CONFIRM

```lua
GOSSIP_CONFIRM(gossipID: number, text: string, cost: WOWMONEY)
```

`SynchronousEvent`

### GOSSIP_CONFIRM_CANCEL

```lua
GOSSIP_CONFIRM_CANCEL()
```

`SynchronousEvent`

### GOSSIP_ENTER_CODE

```lua
GOSSIP_ENTER_CODE(gossipID: number)
```

`SynchronousEvent`

### GOSSIP_OPTIONS_REFRESHED

```lua
GOSSIP_OPTIONS_REFRESHED()
```

`SynchronousEvent`

### GOSSIP_SHOW

```lua
GOSSIP_SHOW(uiTextureKit: textureKit?)
```

`SynchronousEvent`

## Types

### GossipOptionRewardType

*Enumeration* · 2 values, 0..1

Access values as `Enum.GossipOptionRewardType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `GossipOptionRewardType` | = 0 |
| `Currency` | `GossipOptionRewardType` | = 1 |

### GossipOptionStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.GossipOptionStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `GossipOptionStatus` | = 0 |
| `Unavailable` | `GossipOptionStatus` | = 1 |
| `Locked` | `GossipOptionStatus` | = 2 |
| `AlreadyComplete` | `GossipOptionStatus` | = 3 |

### GossipOptionUIWidgetSetTypes

*Enumeration* · 2 values, 0..1

Access values as `Enum.GossipOptionUIWidgetSetTypes.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Modifiers` | `GossipOptionUIWidgetSetTypes` | = 0 |
| `Background` | `GossipOptionUIWidgetSetTypes` | = 1 |

### FriendshipReputationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `friendshipFactionID` | `number` |  |
| `standing` | `number` |  |
| `maxRep` | `number` |  |
| `name` | `string?` |  |
| `text` | `string` |  |
| `texture` | `number` |  |
| `reaction` | `string` |  |
| `reactionThreshold` | `number` |  |
| `nextThreshold` | `number?` |  |
| `reversedColor` | `bool` |  |
| `overrideColor` | `number?` |  |

### FriendshipReputationRankInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currentLevel` | `number` |  |
| `maxLevel` | `number` |  |

### GossipOptionRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `quantity` | `number` |  |
| `rewardType` | `GossipOptionRewardType` |  |
| `context` | `ItemCreationContext` |  |

### GossipOptionUIInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `gossipOptionID` | `number?` |  |
| `name` | `string` |  |
| `icon` | `fileID` |  |
| `rewards` | `GossipOptionRewardInfo[]` |  |
| `status` | `GossipOptionStatus` |  |
| `spellID` | `number?` |  |
| `flags` | `number` |  |
| `overrideIconID` | `fileID?` |  |
| `selectOptionWhenOnlyOption` | `bool` |  |
| `orderIndex` | `number` |  |
| `failureDescription` | `string?` |  |

### GossipOptionUIWidgetSetAndType

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `widgetType` | `number` |  |
| `uiWidgetSetID` | `number` |  |

### GossipPoiInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `textureIndex` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `inBattleMap` | `bool` |  |

### GossipQuestUIInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `questLevel` | `number` |  |
| `isTrivial` | `bool` |  |
| `frequency` | `number?` |  |
| `repeatable` | `bool?` |  |
| `isComplete` | `bool?` |  |
| `isLegendary` | `bool` |  |
| `isIgnored` | `bool` |  |
| `questID` | `number` |  |
| `isImportant` | `bool` |  |
| `isMeta` | `bool` |  |
| `questInfoID` | `number` |  |
