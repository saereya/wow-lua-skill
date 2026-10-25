# LegendaryCrafting

Namespace `C_LegendaryCrafting` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/legendarycraftingdocumentation.lua` (FileDataID 4637129)

## Functions

### CloseRuneforgeInteraction

```lua
C_LegendaryCrafting.CloseRuneforgeInteraction()
```

### CraftRuneforgeLegendary

```lua
C_LegendaryCrafting.CraftRuneforgeLegendary(description: RuneforgeLegendaryCraftDescription)
```

`SecretArguments=AllowedWhenUntainted`

### GetRuneforgeItemPreviewInfo

```lua
C_LegendaryCrafting.GetRuneforgeItemPreviewInfo(baseItem: ItemLocation, runeforgePowerID: number?, modifiers: number[]?) -> info: RuneforgeItemPreviewInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `runeforgePowerID` | `number?` |  |
| `modifiers` | `number[]?` |  |

### GetRuneforgeLegendaryComponentInfo

```lua
C_LegendaryCrafting.GetRuneforgeLegendaryComponentInfo(runeforgeLegendary: ItemLocation) -> componentInfo: RuneforgeLegendaryComponentInfo
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `runeforgeLegendary` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetRuneforgeLegendaryCost

```lua
C_LegendaryCrafting.GetRuneforgeLegendaryCost(baseItem: ItemLocation) -> cost: CurrencyCost[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetRuneforgeLegendaryCraftSpellID

```lua
C_LegendaryCrafting.GetRuneforgeLegendaryCraftSpellID() -> spellID: number
```

### GetRuneforgeLegendaryCurrencies

```lua
C_LegendaryCrafting.GetRuneforgeLegendaryCurrencies() -> currencies: number[]
```

### GetRuneforgeLegendaryUpgradeCost

```lua
C_LegendaryCrafting.GetRuneforgeLegendaryUpgradeCost(runeforgeLegendary: ItemLocation, upgradeItem: ItemLocation) -> cost: CurrencyCost[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `runeforgeLegendary` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `upgradeItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetRuneforgeModifierInfo

```lua
C_LegendaryCrafting.GetRuneforgeModifierInfo(baseItem: ItemLocation, powerID: number?, addedModifierIndex: luaIndex, modifiers: number[]) -> name: string, description: string[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `powerID` | `number?` |  |
| `addedModifierIndex` | `luaIndex` |  |
| `modifiers` | `number[]` |  |

### GetRuneforgeModifiers

```lua
C_LegendaryCrafting.GetRuneforgeModifiers() -> modifiedReagentItemIDs: number[]
```

### GetRuneforgePowerInfo

```lua
C_LegendaryCrafting.GetRuneforgePowerInfo(runeforgePowerID: number) -> power: RuneforgePower
```

`SecretArguments=AllowedWhenUntainted`

### GetRuneforgePowers

```lua
C_LegendaryCrafting.GetRuneforgePowers(baseItem: ItemLocation?, filter: RuneforgePowerFilter?) -> primaryRuneforgePowerIDs: number[], otherRuneforgePowerIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation?` | `Mixin=ItemLocationMixin` |
| `filter` | `RuneforgePowerFilter?` |  |

### GetRuneforgePowersByClassSpecAndCovenant

```lua
C_LegendaryCrafting.GetRuneforgePowersByClassSpecAndCovenant(classID: number?, specID: number?, covenantID: number?, filter: RuneforgePowerFilter?) -> runeforgePowerIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetRuneforgePowerSlots

```lua
C_LegendaryCrafting.GetRuneforgePowerSlots(runeforgePowerID: number) -> slotNames: cstring[]
```

`SecretArguments=AllowedWhenUntainted`

### IsRuneforgeLegendary

```lua
C_LegendaryCrafting.IsRuneforgeLegendary(item: ItemLocation) -> isRuneforgeLegendary: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsRuneforgeLegendaryMaxLevel

```lua
C_LegendaryCrafting.IsRuneforgeLegendaryMaxLevel(runeforgeLegendary: ItemLocation) -> isMaxLevel: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `runeforgeLegendary` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsUpgradeItemValidForRuneforgeLegendary

```lua
C_LegendaryCrafting.IsUpgradeItemValidForRuneforgeLegendary(runeforgeLegendary: ItemLocation, upgradeItem: ItemLocation) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `runeforgeLegendary` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `upgradeItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### IsValidRuneforgeBaseItem

```lua
C_LegendaryCrafting.IsValidRuneforgeBaseItem(baseItem: ItemLocation) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### MakeRuneforgeCraftDescription

```lua
C_LegendaryCrafting.MakeRuneforgeCraftDescription(baseItem: ItemLocation, runeforgePowerID: number, modifiers: number[]) -> description: RuneforgeLegendaryCraftDescription
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `runeforgePowerID` | `number` |  |
| `modifiers` | `number[]` |  |

### UpgradeRuneforgeLegendary

```lua
C_LegendaryCrafting.UpgradeRuneforgeLegendary(runeforgeLegendary: ItemLocation, upgradeItem: ItemLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `runeforgeLegendary` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `upgradeItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |

## Events

### NEW_RUNEFORGE_POWER_ADDED

```lua
NEW_RUNEFORGE_POWER_ADDED(powerID: number)
```

`SynchronousEvent`

### RUNEFORGE_LEGENDARY_CRAFTING_CLOSED

```lua
RUNEFORGE_LEGENDARY_CRAFTING_CLOSED()
```

`SynchronousEvent`

### RUNEFORGE_LEGENDARY_CRAFTING_OPENED

```lua
RUNEFORGE_LEGENDARY_CRAFTING_OPENED(isUpgrade: bool)
```

`SynchronousEvent`

### RUNEFORGE_POWER_INFO_UPDATED

```lua
RUNEFORGE_POWER_INFO_UPDATED(powerID: number)
```

`SynchronousEvent`
