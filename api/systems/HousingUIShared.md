# HousingUIShared

source `interface/addons/blizzard_apidocumentationgenerated/housinguishareddocumentation.lua` (FileDataID 6240408)

## Types

### HouseLevelRewardType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HouseLevelRewardType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Value` | `HouseLevelRewardType` | = 0 |
| `Object` | `HouseLevelRewardType` | = 1 |

### HouseLevelRewardValueType

*Enumeration* · 4 values, 0..3

Access values as `Enum.HouseLevelRewardValueType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ExteriorDecor` | `HouseLevelRewardValueType` | = 0 |
| `InteriorDecor` | `HouseLevelRewardValueType` | = 1 |
| `Rooms` | `HouseLevelRewardValueType` | = 2 |
| `Fixtures` | `HouseLevelRewardValueType` | = 3 |

### HouseVisitType

*Enumeration* · 4 values, 0..3

Access values as `Enum.HouseVisitType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unknown` | `HouseVisitType` | = 0 |
| `Friend` | `HouseVisitType` | = 1 |
| `Guild` | `HouseVisitType` | = 2 |
| `Party` | `HouseVisitType` | = 3 |

### HouseInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `plotID` | `number` |  |
| `houseName` | `string?` |  |
| `ownerName` | `string?` |  |
| `plotCost` | `number?` |  |
| `neighborhoodName` | `string?` |  |
| `moveOutTime` | `time_t?` |  |
| `plotReserved` | `bool?` |  |
| `neighborhoodGUID` | `WOWGUID?` |  |
| `houseGUID` | `WOWGUID?` |  |

### HouseLevelFavor

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `houseGUID` | `WOWGUID?` |  |
| `houseLevel` | `number` |  |
| `houseFavor` | `number` |  |

### HouseLevelInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `level` | `number` | This specific house's current level, determined/increasesd by earning house xp |
| `interiorDecorPlacementBudget` | `number` | Current max decor placement budget for inside the house; Can be increased via house level |
| `exteriorDecorPlacementBudget` | `number` | Current max decor placement budget for the house exterior/in the house's plot; Can be increased via house level |
| `roomPlacementBudget` | `number` | Current max room placement budget for the house; Can be increased via house level |
| `exteriorFixtureBudget` | `number` |  |

### HouseLevelReward

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `HouseLevelRewardType` |  |
| `asset` | `ModelAsset?` |  |
| `iconTexture` | `FileAsset?` |  |
| `iconAtlas` | `textureAtlas?` |  |
| `objectName` | `string?` |  |
| `tooltipText` | `string?` |  |
| `valueType` | `HouseLevelRewardValueType?` |  |
| `oldValue` | `number?` |  |
| `newValue` | `number?` |  |

### HouseOwnerCharacterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `characterName` | `string` |  |
| `classID` | `number` |  |
| `error` | `HouseOwnerError` |  |
| `playerGUID` | `WOWGUID` |  |

### HouseholdMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `characterName` | `string` |  |
| `classID` | `number` |  |

### NeighborhoodInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `neighborhoodType` | `NeighborhoodType` |  |
| `neighborhoodOwnerType` | `NeighborhoodOwnerType` | default `"None"` |
| `neighborhoodName` | `string` |  |
| `neighborhoodGUID` | `WOWGUID` |  |
| `ownerGUID` | `WOWGUID` |  |
| `suggestionReason` | `HouseFinderSuggestionReason?` |  |
| `ownerName` | `string?` |  |
| `locationName` | `string?` |  |

### NeighborhoodPlotMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `mapPosition` | `vector2` | `Mixin=Vector2DMixin` |
| `plotDataID` | `number` |  |
| `plotID` | `number` |  |
| `ownerType` | `HousingPlotOwnerType` | default `"None"` |
| `plotCost` | `number?` |  |
| `ownerName` | `string?` |  |

### NeighborhoodRosterMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playerGUID` | `WOWGUID` |  |
| `residentName` | `string` |  |
| `residentType` | `ResidentType` |  |
| `isOnline` | `bool` |  |
| `plotID` | `number` |  |
| `subdivision` | `number?` |  |

### NeighborhoodRosterMemberUpdateInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `playerGUID` | `WOWGUID` |  |
| `residentType` | `ResidentType` |  |
| `isOnline` | `bool` |  |
