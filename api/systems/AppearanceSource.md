# AppearanceSource

source `interface/addons/blizzard_apidocumentationgenerated/appearancesourcedocumentation.lua` (FileDataID 4637010)

## Types

### AppearanceSourceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `visualID` | `number` |  |
| `sourceID` | `number` |  |
| `isCollected` | `bool` |  |
| `itemID` | `number` |  |
| `itemModID` | `number` |  |
| `invType` | `luaIndex` | default `0` |
| `categoryID` | `TransmogCollectionType` | default `"None"` |
| `playerCanCollect` | `bool` |  |
| `isValidSourceForPlayer` | `bool` |  |
| `canDisplayOnPlayer` | `bool` |  |
| `inventorySlot` | `number?` |  |
| `sourceType` | `luaIndex?` |  |
| `name` | `string?` |  |
| `quality` | `number?` |  |
| `useError` | `string?` |  |
| `useErrorType` | `TransmogUseErrorType?` |  |
| `meetsTransmogPlayerCondition` | `bool?` |  |
| `isHideVisual` | `bool?` |  |
| `isValidForEquippedItem` | `bool?` |  |
