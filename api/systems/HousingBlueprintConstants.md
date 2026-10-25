# HousingBlueprintConstants

source `interface/addons/blizzard_apidocumentationgenerated/housingblueprintconstantsdocumentation.lua` (FileDataID 7950561)

## Types

### HousingBlueprintContentType

*Enumeration* · 7 values, 0..6

Access values as `Enum.HousingBlueprintContentType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingBlueprintContentType` | = 0 |
| `HouseType` | `HousingBlueprintContentType` | = 1 |
| `Room` | `HousingBlueprintContentType` | = 2 |
| `Decor` | `HousingBlueprintContentType` | = 3 |
| `Dye` | `HousingBlueprintContentType` | = 4 |
| `Fixture` | `HousingBlueprintContentType` | = 5 |
| `Other` | `HousingBlueprintContentType` | = 6 |

### HousingBlueprintUnmetRequirementFlags

*Enumeration* · 8 values, 1..128

Access values as `Enum.HousingBlueprintUnmetRequirementFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InsufficientBudget` | `HousingBlueprintUnmetRequirementFlags` | = 1 |
| `MissingRoom` | `HousingBlueprintUnmetRequirementFlags` | = 2 |
| `MissingFixture` | `HousingBlueprintUnmetRequirementFlags` | = 4 |
| `MissingDecor` | `HousingBlueprintUnmetRequirementFlags` | = 8 |
| `MissingDye` | `HousingBlueprintUnmetRequirementFlags` | = 16 |
| `MismatchedExteriorFaction` | `HousingBlueprintUnmetRequirementFlags` | = 32 |
| `HouseTypeLocked` | `HousingBlueprintUnmetRequirementFlags` | = 64 |
| `HouseSizeLocked` | `HousingBlueprintUnmetRequirementFlags` | = 128 |

### HousingBlueprintBudgetEntry

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `budgetType` | `HousingBudgetType` |  |
| `cost` | `number` |  |
| `max` | `number?` | Will be nil if there is no target house or information for it is unavailable |
| `current` | `number?` | Will be nil if there is no target house or information for it is unavailable |

### HousingBlueprintBudgetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `exteriorBudgets` | `table<HousingBudgetType, HousingBlueprintBudgetEntry>` | Map of budget type to budget entry |
| `interiorBudgets` | `table<HousingBudgetType, HousingBlueprintBudgetEntry>` | Map of budget type to budget entry |

### HousingBlueprintCollection

*Structure*

List of Blueprints, separated into like groups

Fields:

| Name | Type | Notes |
|---|---|---|
| `groups` | `HousingBlueprintGroup[]` |  |

### HousingBlueprintContentEntry

*Structure*

A single specific object that makes up a Blueprint's contents

Fields:

| Name | Type | Notes |
|---|---|---|
| `contentType` | `HousingBlueprintContentType` |  |
| `recordID` | `number` |  |
| `name` | `string` |  |
| `total` | `number` | default `0`; Total instances of the object contained within or required by the Blueprint |
| `numMissing` | `number` | default `0`; The number of instances of this item that the player doesn't own, or have unlocked, or have available for use (depending on the type of content) |
| `invalid` | `bool` | default `false`; True for content that isn't valid for use whether it's owned or not, for example exterior types of the opposite faction than the house's neighborhood |
| `tooltip` | `string?` |  |

### HousingBlueprintContentGroup

*Structure*

Group of entries of one specific type of object within a Blueprint

Fields:

| Name | Type | Notes |
|---|---|---|
| `contentType` | `HousingBlueprintContentType` |  |
| `entries` | `HousingBlueprintContentEntry[]` |  |

### HousingBlueprintContentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `shareCode` | `string` |  |
| `targetHouseGUID` | `WOWGUID?` |  |
| `budgetInfo` | `HousingBlueprintBudgetInfo` |  |
| `contentGroups` | `HousingBlueprintContentGroup[]` |  |
| `unmetRequirementFlags` | `HousingBlueprintUnmetRequirementFlags` |  |
| `blockingRequirementFlags` | `HousingBlueprintUnmetRequirementFlags` |  |

### HousingBlueprintGroup

*Structure*

Group of Blueprints of the same or similar types

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `entries` | `HousingBlueprintInfo[]` |  |

### HousingBlueprintInfo

*Structure*

List of entries of one specific type of object within a Blueprint

Fields:

| Name | Type | Notes |
|---|---|---|
| `blueprintID` | `BigUInteger` |  |
| `shareCode` | `string` |  |
| `name` | `string` |  |
| `blueprintType` | `HousingBlueprintType` |  |
| `creationTime` | `time_t` |  |
| `isAutoSave` | `bool` | True if this blueprint is an automatically saved backup, rather than a manually player-saved blueprint |
