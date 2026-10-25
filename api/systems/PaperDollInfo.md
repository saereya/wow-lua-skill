# PaperDollInfo

Namespace `C_PaperDollInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/paperdollinfodocumentation.lua` (FileDataID 4637165)

## Functions

### AmmoNeeded

```lua
C_PaperDollInfo.AmmoNeeded() -> ammoNeeded: bool
```

### CanAutoEquipCursorItem

```lua
C_PaperDollInfo.CanAutoEquipCursorItem() -> canAutoEquip: bool
```

### CancelTemporaryEnchantment

```lua
C_PaperDollInfo.CancelTemporaryEnchantment(slot: LuaInventorySlot)
```

Cancels active temporary enchantments on inventory slot items.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CursorCanGoInSlot

```lua
C_PaperDollInfo.CursorCanGoInSlot(slotIndex: luaIndex) -> canOccupySlot: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetArmorEffectiveness

```lua
C_PaperDollInfo.GetArmorEffectiveness(armor: number, attackerLevel: number) -> effectiveness: number
```

`SecretArguments=AllowedWhenUntainted`

### GetArmorEffectivenessAgainstTarget

```lua
C_PaperDollInfo.GetArmorEffectivenessAgainstTarget(armor: number) -> effectiveness: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetInspectAzeriteItemEmpoweredChoices

```lua
C_PaperDollInfo.GetInspectAzeriteItemEmpoweredChoices(unit: UnitToken, equipmentSlotIndex: luaIndex) -> azeritePowerIDs: number[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInspectGuildInfo

```lua
C_PaperDollInfo.GetInspectGuildInfo(unitString: string) -> achievementPoints: number, numMembers: number, guildName: string, realmName: string
```

`SecretArguments=AllowedWhenUntainted`

### GetInspectItemLevel

```lua
C_PaperDollInfo.GetInspectItemLevel(unit: UnitToken) -> equippedItemLevel: number
```

`SecretArguments=AllowedWhenUntainted`

### GetInspectRatedBGBlitzData

```lua
C_PaperDollInfo.GetInspectRatedBGBlitzData() -> ratedBGBlitzData: InspectPVPData
```

### GetInspectRatedBGData

```lua
C_PaperDollInfo.GetInspectRatedBGData() -> ratedBGData: InspectRatedBGData
```

### GetInspectRatedSoloShuffleData

```lua
C_PaperDollInfo.GetInspectRatedSoloShuffleData() -> ratedSoloShuffleData: InspectPVPData
```

### GetInventorySlotInfo

```lua
C_PaperDollInfo.GetInventorySlotInfo(slotName: cstring) -> invSlot: number, slotTexture: fileID, checkRelic: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInventorySlotInfoForInvSlot

```lua
C_PaperDollInfo.GetInventorySlotInfoForInvSlot(invSlotValue: number) -> invSlot: number, slotTexture: fileID, checkRelic: bool, slotName: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `invSlotValue` | `number` | This is the Lua version of the INVSLOT enum, not a luaIndex |

### GetMinItemLevel

```lua
C_PaperDollInfo.GetMinItemLevel() -> minItemLevel: number?
```

### GetStaggerPercentage

```lua
C_PaperDollInfo.GetStaggerPercentage(unit: UnitToken) -> stagger: number, staggerAgainstTarget: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetTemporaryEnchantmentInfo

```lua
C_PaperDollInfo.GetTemporaryEnchantmentInfo(slot: LuaInventorySlot) -> enchantInfo: TemporaryItemEnchantInfo
```

Queries information about active temporary enchants on inventory slot items.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `slot` | `LuaInventorySlot` | An appropriate INVSLOT_ constant. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `enchantInfo` | `TemporaryItemEnchantInfo` | Returns nothing if no temporary enchantment is active for this slot. |

### IsInventorySlotEnabled

```lua
C_PaperDollInfo.IsInventorySlotEnabled(slotName: stringView) -> isEnabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsRangedSlotShown

```lua
C_PaperDollInfo.IsRangedSlotShown() -> isShown: bool
```

### OffhandHasShield

```lua
C_PaperDollInfo.OffhandHasShield() -> offhandHasShield: bool
```

### OffhandHasWeapon

```lua
C_PaperDollInfo.OffhandHasWeapon() -> offhandHasWeapon: bool
```

## Events

### AVOIDANCE_UPDATE

```lua
AVOIDANCE_UPDATE()
```

`SynchronousEvent`

### CHARACTER_POINTS_CHANGED

```lua
CHARACTER_POINTS_CHANGED(change: number)
```

`SynchronousEvent`

### CHARACTER_UPGRADE_SPELL_TIER_SET

```lua
CHARACTER_UPGRADE_SPELL_TIER_SET(tierIndex: number)
```

`SynchronousEvent`

### COMBAT_RATING_UPDATE

```lua
COMBAT_RATING_UPDATE()
```

`SynchronousEvent`

### DISABLE_XP_GAIN

```lua
DISABLE_XP_GAIN()
```

`SynchronousEvent`

### ENABLE_XP_GAIN

```lua
ENABLE_XP_GAIN()
```

`SynchronousEvent`

### EQUIP_BIND_CONFIRM

```lua
EQUIP_BIND_CONFIRM(slot: number, itemLocation: ItemLocation)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `slot` | `number` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### INSPECT_HONOR_UPDATE

```lua
INSPECT_HONOR_UPDATE()
```

`SynchronousEvent`

### INSPECT_READY

```lua
INSPECT_READY(inspecteeGUID: WOWGUID)
```

`SynchronousEvent`

### LIFESTEAL_UPDATE

```lua
LIFESTEAL_UPDATE()
```

`SynchronousEvent`

### MASTERY_UPDATE

```lua
MASTERY_UPDATE()
```

`SynchronousEvent`

### PET_STATS_UPDATE

```lua
PET_STATS_UPDATE()
```

`SynchronousEvent`

### PLAYER_AVG_ITEM_LEVEL_UPDATE

```lua
PLAYER_AVG_ITEM_LEVEL_UPDATE()
```

`SynchronousEvent`

### PLAYER_EQUIPMENT_CHANGED

```lua
PLAYER_EQUIPMENT_CHANGED(equipmentSlot: number, hasCurrent: bool)
```

`SynchronousEvent`

### PROFESSION_EQUIPMENT_CHANGED

```lua
PROFESSION_EQUIPMENT_CHANGED(skillLineID: number, isTool: bool)
```

`SynchronousEvent`

### PVP_POWER_UPDATE

```lua
PVP_POWER_UPDATE()
```

`SynchronousEvent`

### SPEED_UPDATE

```lua
SPEED_UPDATE()
```

`SynchronousEvent`

### SPELL_POWER_CHANGED

```lua
SPELL_POWER_CHANGED()
```

`SynchronousEvent`

### STURDINESS_UPDATE

```lua
STURDINESS_UPDATE()
```

`SynchronousEvent`

### UPDATE_FACTION

```lua
UPDATE_FACTION()
```

`SynchronousEvent`

### UPDATE_INVENTORY_ALERTS

```lua
UPDATE_INVENTORY_ALERTS()
```

`SynchronousEvent`

### UPDATE_INVENTORY_DURABILITY

```lua
UPDATE_INVENTORY_DURABILITY()
```

`SynchronousEvent`

### WEAPON_SLOT_CHANGED

```lua
WEAPON_SLOT_CHANGED()
```

`UniqueEvent`

## Types

### InspectGuildInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `achievementPoints` | `number` |  |
| `numMembers` | `number` |  |
| `guildName` | `string` |  |
| `realmName` | `string` |  |

### InspectPVPData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rating` | `number` |  |
| `gamesWon` | `number` |  |
| `gamesPlayed` | `number` |  |
| `roundsWon` | `number` |  |
| `roundsPlayed` | `number` |  |

### InspectRatedBGData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `rating` | `number` |  |
| `played` | `number` |  |
| `won` | `number` |  |

### TemporaryItemEnchantInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `enchantID` | `number` |  |
| `remainingTimeMs` | `number` |  |
| `chargesRemaining` | `number` |  |
| `hasExpirationTime` | `bool` |  |
