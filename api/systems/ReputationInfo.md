# ReputationInfo

Namespace `C_Reputation` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/reputationinfodocumentation.lua` (FileDataID 4637187)

## Functions

### AreLegacyReputationsShown

```lua
C_Reputation.AreLegacyReputationsShown() -> areLegacyReputationsShown: bool
```

### CollapseAllFactionHeaders

```lua
C_Reputation.CollapseAllFactionHeaders()
```

### CollapseFactionHeader

```lua
C_Reputation.CollapseFactionHeader(factionSortIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### ExpandAllFactionHeaders

```lua
C_Reputation.ExpandAllFactionHeaders()
```

### ExpandFactionHeader

```lua
C_Reputation.ExpandFactionHeader(factionSortIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetFactionDataByID

```lua
C_Reputation.GetFactionDataByID(factionID: number) -> factionData: FactionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetFactionDataByIndex

```lua
C_Reputation.GetFactionDataByIndex(factionSortIndex: luaIndex) -> factionData: FactionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetFactionParagonInfo

```lua
C_Reputation.GetFactionParagonInfo(factionID: number) -> currentValue: number, threshold: number, rewardQuestID: number, hasRewardPending: bool, tooLowLevelForParagon: bool, paragonStorageLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGuildFactionData

```lua
C_Reputation.GetGuildFactionData() -> guildFactionData: FactionData?
```

### GetGuildRepExpirationTime

```lua
C_Reputation.GetGuildRepExpirationTime() -> expirationTime: number?
```

### GetNumFactions

```lua
C_Reputation.GetNumFactions() -> numFactions: number
```

### GetReputationSortType

```lua
C_Reputation.GetReputationSortType() -> sortType: ReputationSortType
```

### GetSelectedFaction

```lua
C_Reputation.GetSelectedFaction() -> selectedFactionSortIndex: luaIndex
```

### GetWatchedFactionData

```lua
C_Reputation.GetWatchedFactionData() -> watchedFactionData: FactionData?
```

### IsAccountWideReputation

```lua
C_Reputation.IsAccountWideReputation(factionID: number) -> isAccountWide: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFactionActive

```lua
C_Reputation.IsFactionActive(factionSortIndex: luaIndex) -> isActive: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFactionParagon

```lua
C_Reputation.IsFactionParagon(factionID: number) -> factionIsParagon: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFactionParagonForCurrentPlayer

```lua
C_Reputation.IsFactionParagonForCurrentPlayer(factionID: number) -> currentPlayerHasParagon: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMajorFaction

```lua
C_Reputation.IsMajorFaction(factionID: number) -> isMajorFaction: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestFactionParagonPreloadRewardData

```lua
C_Reputation.RequestFactionParagonPreloadRewardData(factionID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFactionActive

```lua
C_Reputation.SetFactionActive(factionSortIndex: luaIndex, setActive: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetLegacyReputationsShown

```lua
C_Reputation.SetLegacyReputationsShown(showLegacyReputations: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetReputationSortType

```lua
C_Reputation.SetReputationSortType(sortType: ReputationSortType)
```

`SecretArguments=AllowedWhenUntainted`

### SetSelectedFaction

```lua
C_Reputation.SetSelectedFaction(factionSortIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### SetWatchedFactionByID

```lua
C_Reputation.SetWatchedFactionByID(factionID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetWatchedFactionByIndex

```lua
C_Reputation.SetWatchedFactionByIndex(factionSortIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### ToggleFactionAtWar

```lua
C_Reputation.ToggleFactionAtWar(factionSortIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### FACTION_STANDING_CHANGED

```lua
FACTION_STANDING_CHANGED(factionID: number, updatedStanding: number)
```

`SynchronousEvent`

## Types

### ReputationSortType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ReputationSortType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ReputationSortType` | = 0 |
| `Account` | `ReputationSortType` | = 1 |
| `Character` | `ReputationSortType` | = 2 |

### FactionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `factionID` | `number` |  |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `reaction` | `luaIndex` |  |
| `currentReactionThreshold` | `number` |  |
| `nextReactionThreshold` | `number` |  |
| `currentStanding` | `number` |  |
| `atWarWith` | `bool` |  |
| `canToggleAtWar` | `bool` |  |
| `isChild` | `bool` |  |
| `isHeader` | `bool` |  |
| `isHeaderWithRep` | `bool` |  |
| `isCollapsed` | `bool` |  |
| `isWatched` | `bool` |  |
| `hasBonusRepGain` | `bool` |  |
| `canSetInactive` | `bool` |  |
| `isAccountWide` | `bool` |  |
