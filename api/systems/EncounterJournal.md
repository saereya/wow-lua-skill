# EncounterJournal

Namespace `C_EncounterJournal` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encounterjournaldocumentation.lua` (FileDataID 4637091)

## Functions

### GetBaseDifficultyID

```lua
C_EncounterJournal.GetBaseDifficultyID(difficultyID: number) -> baseDifficultyID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetDungeonEntrancesForMap

```lua
C_EncounterJournal.GetDungeonEntrancesForMap(uiMapID: number) -> dungeonEntrances: DungeonEntranceMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetEncounterJournalLink

```lua
C_EncounterJournal.GetEncounterJournalLink(linkType: JournalLinkTypes, ID: number, displayText: string, difficultyID: number) -> link: string
```

`SecretArguments=AllowedWhenUntainted`

### GetEncountersOnMap

```lua
C_EncounterJournal.GetEncountersOnMap(uiMapID: number) -> encounters: EncounterJournalMapEncounterInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetInstanceForGameMap

```lua
C_EncounterJournal.GetInstanceForGameMap(mapID: number) -> journalInstanceID: number?
```

GameMap as opposed to UIMap since we use a mapID not a uiMapID.

`SecretArguments=AllowedWhenUntainted`

### GetLootInfo

```lua
C_EncounterJournal.GetLootInfo(id: number) -> itemInfo: EncounterJournalItemInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetLootInfoByIndex

```lua
C_EncounterJournal.GetLootInfoByIndex(index: luaIndex, encounterIndex: luaIndex?) -> itemInfo: EncounterJournalItemInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSectionIconFlags

```lua
C_EncounterJournal.GetSectionIconFlags(sectionID: number) -> iconFlags: number[]?
```

Represents the icon indices for this EJ section.  An icon index can be used to arrive at texture coordinates for specific encounter types, e.g.: EncounterJournal_SetFlagIcon

`SecretArguments=AllowedWhenUntainted`

### GetSectionInfo

```lua
C_EncounterJournal.GetSectionInfo(sectionID: number) -> info: EncounterJournalSectionInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSlotFilter

```lua
C_EncounterJournal.GetSlotFilter() -> filter: ItemSlotFilterType
```

### InitalizeSelectedTier

```lua
C_EncounterJournal.InitalizeSelectedTier()
```

### InstanceHasDifficultyID

```lua
C_EncounterJournal.InstanceHasDifficultyID(difficultyID: number) -> hasDifficultyID: bool
```

`SecretArguments=AllowedWhenUntainted`

### InstanceHasLoot

```lua
C_EncounterJournal.InstanceHasLoot(instanceID: number?) -> hasLoot: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsEncounterComplete

```lua
C_EncounterJournal.IsEncounterComplete(journalEncounterID: number) -> isEncounterComplete: bool
```

`SecretArguments=AllowedWhenUntainted`

### OnClose

```lua
C_EncounterJournal.OnClose()
```

`HasRestrictions`

### OnOpen

```lua
C_EncounterJournal.OnOpen()
```

`HasRestrictions`

### ResetSlotFilter

```lua
C_EncounterJournal.ResetSlotFilter()
```

### SetPreviewMythicPlusLevel

```lua
C_EncounterJournal.SetPreviewMythicPlusLevel(level: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPreviewPvpTier

```lua
C_EncounterJournal.SetPreviewPvpTier(tier: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSlotFilter

```lua
C_EncounterJournal.SetSlotFilter(filterSlot: ItemSlotFilterType)
```

`SecretArguments=AllowedWhenUntainted`

### SetTab

```lua
C_EncounterJournal.SetTab(tabIdx: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### StartArathiRPE

```lua
C_EncounterJournal.StartArathiRPE()
```

## Events

### EJ_DIFFICULTY_UPDATE

```lua
EJ_DIFFICULTY_UPDATE(difficultyID: number)
```

`SynchronousEvent`

### EJ_LOOT_DATA_RECIEVED

```lua
EJ_LOOT_DATA_RECIEVED(itemID: number?)
```

`SynchronousEvent` `UniqueEvent`

### SHOW_JOURNEYS_UI

```lua
SHOW_JOURNEYS_UI(factionID: number)
```

Signaled when the UI needs to display the journeys dashboard at a specific faction.

`SynchronousEvent`

## Types

### ItemSlotFilterType

*Enumeration* · 16 values, 0..15

Access values as `Enum.ItemSlotFilterType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Head` | `ItemSlotFilterType` | = 0 |
| `Neck` | `ItemSlotFilterType` | = 1 |
| `Shoulder` | `ItemSlotFilterType` | = 2 |
| `Cloak` | `ItemSlotFilterType` | = 3 |
| `Chest` | `ItemSlotFilterType` | = 4 |
| `Wrist` | `ItemSlotFilterType` | = 5 |
| `Hand` | `ItemSlotFilterType` | = 6 |
| `Waist` | `ItemSlotFilterType` | = 7 |
| `Legs` | `ItemSlotFilterType` | = 8 |
| `Feet` | `ItemSlotFilterType` | = 9 |
| `MainHand` | `ItemSlotFilterType` | = 10 |
| `OffHand` | `ItemSlotFilterType` | = 11 |
| `Finger` | `ItemSlotFilterType` | = 12 |
| `Trinket` | `ItemSlotFilterType` | = 13 |
| `Other` | `ItemSlotFilterType` | = 14 |
| `NoFilter` | `ItemSlotFilterType` | = 15 |

### DungeonEntranceMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `atlasName` | `string` |  |
| `journalInstanceID` | `number` |  |

### EncounterJournalItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `encounterID` | `number?` |  |
| `name` | `string?` |  |
| `itemQuality` | `string?` |  |
| `filterType` | `ItemSlotFilterType?` |  |
| `icon` | `fileID?` |  |
| `slot` | `string?` |  |
| `armorType` | `string?` |  |
| `link` | `string?` |  |
| `handError` | `bool?` |  |
| `weaponTypeError` | `bool?` |  |
| `displayAsPerPlayerLoot` | `bool?` |  |
| `displayAsVeryRare` | `bool?` |  |
| `displayAsExtremelyRare` | `bool?` |  |
| `displaySeasonID` | `number?` |  |

### EncounterJournalMapEncounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterID` | `number` |  |
| `mapX` | `number` |  |
| `mapY` | `number` |  |

### EncounterJournalSectionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `title` | `cstring` |  |
| `description` | `string?` |  |
| `headerType` | `number` |  |
| `abilityIcon` | `fileID` |  |
| `creatureDisplayID` | `number` |  |
| `uiModelSceneID` | `number` |  |
| `siblingSectionID` | `number?` |  |
| `firstChildSectionID` | `number?` |  |
| `filteredByDifficulty` | `bool` |  |
| `link` | `string` |  |
| `startsOpen` | `bool` |  |
