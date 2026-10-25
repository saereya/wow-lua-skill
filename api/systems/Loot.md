# Loot

Namespace `C_Loot` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lootdocumentation.lua` (FileDataID 4637128)

## Functions

### GetLootRollDuration

```lua
C_Loot.GetLootRollDuration(rollID: number) -> duration: number?
```

`SecretArguments=AllowedWhenUntainted`

### IsLegacyLootModeEnabled

```lua
C_Loot.IsLegacyLootModeEnabled() -> isLegacyLootModeEnabled: bool
```

## Events

### AZERITE_EMPOWERED_ITEM_LOOTED

```lua
AZERITE_EMPOWERED_ITEM_LOOTED(itemLink: cstring)
```

`SynchronousEvent`

### BONUS_ROLL_ACTIVATE

```lua
BONUS_ROLL_ACTIVATE()
```

`SynchronousEvent`

### BONUS_ROLL_DEACTIVATE

```lua
BONUS_ROLL_DEACTIVATE()
```

`SynchronousEvent`

### BONUS_ROLL_FAILED

```lua
BONUS_ROLL_FAILED()
```

`SynchronousEvent`

### BONUS_ROLL_RESULT

```lua
BONUS_ROLL_RESULT(typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, currencyID: number?, isSecondaryResult: bool, corrupted: bool)
```

`SynchronousEvent`

### BONUS_ROLL_STARTED

```lua
BONUS_ROLL_STARTED()
```

`SynchronousEvent`

### CANCEL_ALL_LOOT_ROLLS

```lua
CANCEL_ALL_LOOT_ROLLS()
```

`SynchronousEvent`

### CANCEL_LOOT_ROLL

```lua
CANCEL_LOOT_ROLL(rollID: number)
```

`SynchronousEvent`

### CONFIRM_DISENCHANT_ROLL

```lua
CONFIRM_DISENCHANT_ROLL(rollID: number, rollType: number)
```

`SynchronousEvent`

### CONFIRM_LOOT_ROLL

```lua
CONFIRM_LOOT_ROLL(rollID: number, rollType: number, confirmReason: cstring)
```

`SynchronousEvent`

### ENCOUNTER_LOOT_RECEIVED

```lua
ENCOUNTER_LOOT_RECEIVED(encounterID: number, itemID: number, itemLink: cstring, quantity: number, itemName: cstring, fileName: cstring)
```

`SynchronousEvent`

### GARRISON_MISSION_BONUS_ROLL_LOOT

```lua
GARRISON_MISSION_BONUS_ROLL_LOOT(itemID: number, quantity: number)
```

`SynchronousEvent`

### ITEM_PUSH

```lua
ITEM_PUSH(bagSlot: luaIndex, iconFileID: number)
```

`SynchronousEvent`

### LEGACY_LOOT_RULES_CHANGED

```lua
LEGACY_LOOT_RULES_CHANGED(isLegacyLootModeEnabled: bool)
```

`SynchronousEvent`

### LOOT_BIND_CONFIRM

```lua
LOOT_BIND_CONFIRM(lootSlot: luaIndex)
```

`SynchronousEvent`

### LOOT_CLOSED

```lua
LOOT_CLOSED()
```

`SynchronousEvent`

### LOOT_ITEM_AVAILABLE

```lua
LOOT_ITEM_AVAILABLE(itemTooltip: cstring, lootHandle: number)
```

`SynchronousEvent`

### LOOT_ITEM_ROLL_WON

```lua
LOOT_ITEM_ROLL_WON(itemLink: cstring, rollQuantity: number, rollType: number, roll: number, upgraded: bool)
```

`SynchronousEvent`

### LOOT_OPENED

```lua
LOOT_OPENED(autoLoot: bool, isFromItem: bool)
```

`SynchronousEvent`

### LOOT_READY

```lua
LOOT_READY(autoloot: bool)
```

`SynchronousEvent`

### LOOT_ROLLS_COMPLETE

```lua
LOOT_ROLLS_COMPLETE(lootHandle: number)
```

`SynchronousEvent`

### LOOT_SLOT_CHANGED

```lua
LOOT_SLOT_CHANGED(lootSlot: luaIndex)
```

`SynchronousEvent`

### LOOT_SLOT_CLEARED

```lua
LOOT_SLOT_CLEARED(lootSlot: luaIndex)
```

`SynchronousEvent`

### MAIN_SPEC_NEED_ROLL

```lua
MAIN_SPEC_NEED_ROLL(rollID: number, roll: number, isWinning: bool)
```

`SynchronousEvent`

### OPEN_MASTER_LOOT_LIST

```lua
OPEN_MASTER_LOOT_LIST()
```

`SynchronousEvent`

### PET_BATTLE_LOOT_RECEIVED

```lua
PET_BATTLE_LOOT_RECEIVED(typeIdentifier: cstring, itemLink: cstring, quantity: number)
```

`SynchronousEvent`

### PLAYER_LOOT_SPEC_UPDATED

```lua
PLAYER_LOOT_SPEC_UPDATED()
```

`SynchronousEvent`

### QUEST_CURRENCY_LOOT_RECEIVED

```lua
QUEST_CURRENCY_LOOT_RECEIVED(questID: number, currencyId: number, quantity: number)
```

`SynchronousEvent`

### QUEST_LOOT_RECEIVED

```lua
QUEST_LOOT_RECEIVED(questID: number, itemLink: cstring, quantity: number)
```

`SynchronousEvent`

### SHOW_LOOT_TOAST

```lua
SHOW_LOOT_TOAST(typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, toastMethod: number, lessAwesome: bool, upgraded: bool, corrupted: bool)
```

`SynchronousEvent`

### SHOW_LOOT_TOAST_LEGENDARY_LOOTED

```lua
SHOW_LOOT_TOAST_LEGENDARY_LOOTED(itemLink: cstring)
```

`SynchronousEvent`

### SHOW_LOOT_TOAST_UPGRADE

```lua
SHOW_LOOT_TOAST_UPGRADE(itemLink: cstring, quantity: number, specID: number, sex: number, baseQuality: number, personalLootToast: bool, lessAwesome: bool)
```

`SynchronousEvent`

### SHOW_PVP_FACTION_LOOT_TOAST

```lua
SHOW_PVP_FACTION_LOOT_TOAST(typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, lessAwesome: bool)
```

`SynchronousEvent`

### SHOW_RATED_PVP_REWARD_TOAST

```lua
SHOW_RATED_PVP_REWARD_TOAST(typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, lessAwesome: bool)
```

`SynchronousEvent`

### START_LOOT_ROLL

```lua
START_LOOT_ROLL(rollID: number, rollTime: number, lootHandle: number?)
```

`SynchronousEvent`

### TRIAL_CAP_REACHED_MONEY

```lua
TRIAL_CAP_REACHED_MONEY()
```

`SynchronousEvent`

### UPDATE_MASTER_LOOT_LIST

```lua
UPDATE_MASTER_LOOT_LIST()
```

`SynchronousEvent`
