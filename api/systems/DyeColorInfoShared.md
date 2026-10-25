# DyeColorInfoShared

source `interface/addons/blizzard_apidocumentationgenerated/dyecolorinfoshareddocumentation.lua` (FileDataID 6637347)

## Types

### DyeColorCategoryDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `cstring` |  |

### DyeColorDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `dyeColorCategoryID` | `number` |  |
| `name` | `cstring` |  |
| `sortOrder` | `number` |  |
| `swatchColorStart` | `colorRGB` | `Mixin=ColorMixin` |
| `swatchColorEnd` | `colorRGB` | `Mixin=ColorMixin` |
| `itemID` | `number?` | The consumable item used to apply this Dye Color; May be nil if dye color does not have an associated item |
| `numOwned` | `number` | The number of this dye's consumable item owned by the player; Includes both held and banked items; Will be 0 if dye has no associated item |
