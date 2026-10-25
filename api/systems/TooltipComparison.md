# TooltipComparison

Namespace `C_TooltipComparison` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/tooltipcomparisondocumentation.lua` (FileDataID 4763881)

## Functions

### CompareItem

```lua
C_TooltipComparison.CompareItem(comparisonItem: TooltipComparisonItem, tooltip: Tooltip, anchorFrame: SimpleFrame?)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### GetItemComparisonDelta

```lua
C_TooltipComparison.GetItemComparisonDelta(comparisonItem: TooltipComparisonItem, equippedItem: TooltipComparisonItem, pairedItem: TooltipComparisonItem?, addPairedStats: bool?) -> lines: string[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `comparisonItem` | `TooltipComparisonItem` |  |
| `equippedItem` | `TooltipComparisonItem` |  |
| `pairedItem` | `TooltipComparisonItem?` |  |
| `addPairedStats` | `bool?` | Whether the paired item's stats are added or subtracted |

### GetItemComparisonInfo

```lua
C_TooltipComparison.GetItemComparisonInfo(comparisonItem: TooltipComparisonItem) -> info: TooltipItemComparisonInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

## Events

### TOOLTIP_SHOW_ITEM_COMPARISON

```lua
TOOLTIP_SHOW_ITEM_COMPARISON(comparisonItem: TooltipComparisonItem, tooltip: Tooltip, anchorFrame: SimpleFrame?)
```

`CallbackEvent`

## Types

### TooltipComparisonMethod

*Enumeration* · 4 values, 0..3

Access values as `Enum.TooltipComparisonMethod.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Single` | `TooltipComparisonMethod` | = 0 |
| `WithBothHands` | `TooltipComparisonMethod` | = 1 |
| `WithBagMainHandItem` | `TooltipComparisonMethod` | = 2 |
| `WithBagOffHandItem` | `TooltipComparisonMethod` | = 3 |

### TooltipItemComparisonInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `method` | `TooltipComparisonMethod` | default `"Single"` |
| `item` | `TooltipComparisonItem` |  |
| `additionalItems` | `TooltipComparisonItem[]` |  |
