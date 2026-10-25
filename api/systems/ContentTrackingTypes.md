# ContentTrackingTypes

source `interface/addons/blizzard_apidocumentationgenerated/contenttrackingtypesdocumentation.lua` (FileDataID 5126424)

## Types

### ContentTrackingError

*Enumeration* · 3 values, 0..2

Access values as `Enum.ContentTrackingError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Untrackable` | `ContentTrackingError` | = 0 |
| `MaxTracked` | `ContentTrackingError` | = 1 |
| `AlreadyTracked` | `ContentTrackingError` | = 2 |

### ContentTrackingResult

*Enumeration* · 3 values, 0..2

Access values as `Enum.ContentTrackingResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `ContentTrackingResult` | = 0 |
| `DataPending` | `ContentTrackingResult` | = 1 |
| `Failure` | `ContentTrackingResult` | = 2 |

### ContentTrackingStopType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ContentTrackingStopType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalidated` | `ContentTrackingStopType` | = 0 |
| `Collected` | `ContentTrackingStopType` | = 1 |
| `Manual` | `ContentTrackingStopType` | = 2 |

### ContentTrackingTargetType

*Enumeration* · 5 values, 0..4

Access values as `Enum.ContentTrackingTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `JournalEncounter` | `ContentTrackingTargetType` | = 0 |
| `Vendor` | `ContentTrackingTargetType` | = 1 |
| `Achievement` | `ContentTrackingTargetType` | = 2 |
| `Profession` | `ContentTrackingTargetType` | = 3 |
| `Quest` | `ContentTrackingTargetType` | = 4 |

### ContentTrackingType

*Enumeration* · 4 values, 0..3

Access values as `Enum.ContentTrackingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Appearance` | `ContentTrackingType` | = 0 |
| `Mount` | `ContentTrackingType` | = 1 |
| `Achievement` | `ContentTrackingType` | = 2 |
| `Decor` | `ContentTrackingType` | = 3 |

### ContentTrackingConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `MaxTrackedCollectableSources` | `number` | = `15` |
| `MaxTrackedAchievements` | `number` | = `10` |

### ContentTrackingMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `number` |  |
| `trackableType` | `ContentTrackingType` |  |
| `trackableID` | `number` |  |
| `targetType` | `ContentTrackingTargetType` |  |
| `targetID` | `number` |  |
| `waypointText` | `string` |  |

### EncounterTrackingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterName` | `cstring` |  |
| `journalEncounterID` | `number?` |  |
| `journalInstanceID` | `number?` |  |
| `instanceName` | `cstring` |  |
| `subText` | `cstring?` |  |
| `difficultyID` | `number?` |  |
| `lfgDungeonID` | `number?` |  |
| `groupFinderActivityID` | `number?` |  |

### VendorTrackingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `creatureName` | `cstring` |  |
| `zoneName` | `string?` |  |
| `currencyType` | `number?` |  |
| `cost` | `BigUInteger?` |  |
