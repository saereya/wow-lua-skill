# LootJournal

Namespace `C_LootJournal` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lootjournaldocumentation.lua` (FileDataID 4637137)

## Functions

### GetItemSetItems

```lua
C_LootJournal.GetItemSetItems(setID: number) -> items: LootJournalItemInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemSets

```lua
C_LootJournal.GetItemSets(classID: number?, specID: number?) -> itemSets: LootJournalItemSetInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### LOOT_JOURNAL_ITEM_UPDATE

```lua
LOOT_JOURNAL_ITEM_UPDATE()
```

`UniqueEvent`

## Types

### LootJournalItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `icon` | `fileID` |  |
| `invType` | `luaIndex` |  |

### LootJournalItemSetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `setID` | `number` |  |
| `itemLevel` | `number` |  |
| `name` | `cstring` |  |
