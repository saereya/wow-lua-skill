# LegendaryCraftingTypes

source `interface/addons/blizzard_apidocumentationgenerated/legendarycraftingtypesdocumentation.lua` (FileDataID 4637121)

## Types

### RuneforgePowerFilter

*Enumeration* · 4 values, 0..3

Access values as `Enum.RuneforgePowerFilter.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `All` | `RuneforgePowerFilter` | = 0 |
| `Relevant` | `RuneforgePowerFilter` | = 1 |
| `Available` | `RuneforgePowerFilter` | = 2 |
| `Unavailable` | `RuneforgePowerFilter` | = 3 |

### RuneforgePowerState

*Enumeration* · 3 values, 0..2

Access values as `Enum.RuneforgePowerState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `RuneforgePowerState` | = 0 |
| `Unavailable` | `RuneforgePowerState` | = 1 |
| `Invalid` | `RuneforgePowerState` | = 2 |

### CurrencyCost

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyID` | `number` |  |
| `amount` | `number` |  |

### RuneforgeItemPreviewInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemGUID` | `WOWGUID` |  |
| `itemLevel` | `number` |  |
| `itemName` | `string` |  |

### RuneforgeLegendaryComponentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `powerID` | `number` |  |
| `modifiers` | `number[]` |  |

### RuneforgeLegendaryCraftDescription

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `baseItem` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `runeforgePowerID` | `number` |  |
| `modifiers` | `number[]` |  |

### RuneforgePower

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `runeforgePowerID` | `number` |  |
| `state` | `RuneforgePowerState` |  |
| `name` | `cstring` |  |
| `descriptionSpellID` | `number` |  |
| `description` | `string` |  |
| `source` | `cstring?` |  |
| `iconFileID` | `fileID` |  |
| `specName` | `cstring?` |  |
| `matchesSpec` | `bool` |  |
| `matchesCovenant` | `bool` |  |
| `covenantID` | `number?` |  |
| `slots` | `cstring[]` |  |
