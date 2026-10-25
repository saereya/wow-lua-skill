# HouseExteriorConstants

source `interface/addons/blizzard_apidocumentationgenerated/houseexteriorconstantsdocumentation.lua` (FileDataID 7318842)

## Types

### HouseExteriorSizeOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `size` | `HousingFixtureSize` |  |
| `name` | `cstring` |  |
| `isLocked` | `bool` |  |

### HouseExteriorSizeOptionsInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `selectedSize` | `HousingFixtureSize` |  |
| `options` | `HouseExteriorSizeOption[]` |  |

### HouseExteriorTypeOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `houseExteriorTypeID` | `number` |  |
| `name` | `cstring` |  |
| `isLocked` | `bool` |  |
| `isInvalid` | `bool` |  |
| `reasonString` | `cstring` |  |

### HouseExteriorTypeOptionsInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `selectedExteriorType` | `number` |  |
| `options` | `HouseExteriorTypeOption[]` |  |

### HousingCoreFixtureInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `selectedVariantFixtureID` | `number` | For fixtures that are variants, the id of specific selected variant; If fixture has no variants, will be the same id as selectedStyleFixtureID |
| `selectedStyleFixtureID` | `number` | For fixtures that are variants, the id of their specific base style fixture; If fixture has no variants, will be the same id as selectedVariantFixtureID |
| `currentStyleVariantOptions` | `HousingFixtureOption[]` | Fixtures that are variants of the same style as the selected (meaning they all share the same hooks); Includes the currently selected fixture |
| `styleOptions` | `HousingFixtureOption[]` | Fixtures that are different styles for this type and size of fixture (swapping will clear all hooks); Includes the currently selected fixture |

### HousingFixtureOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `fixtureID` | `number` |  |
| `name` | `cstring` |  |
| `typeID` | `number` |  |
| `typeName` | `cstring` |  |
| `isLocked` | `bool` |  |
| `isInvalid` | `bool` |  |
| `reasonString` | `cstring` |  |
| `colorID` | `number` |  |

### HousingFixturePointInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ownerHash` | `number` |  |
| `selectedFixtureID` | `number?` |  |
| `fixtureOptions` | `HousingFixtureOption[]` |  |
| `canSelectionBeRemoved` | `bool` |  |
