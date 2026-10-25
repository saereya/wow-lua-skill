# HousingCatalogConstants

source `interface/addons/blizzard_apidocumentationgenerated/housingcatalogconstantsdocumentation.lua` (FileDataID 6907393)

## Types

### HousingCatalogEntryModelScenePresets

*Enumeration* · 10 values, 1317..1452

Access values as `Enum.HousingCatalogEntryModelScenePresets.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DecorDefault` | `HousingCatalogEntryModelScenePresets` | = 1317 |
| `DecorTiny` | `HousingCatalogEntryModelScenePresets` | = 1333 |
| `DecorSmall` | `HousingCatalogEntryModelScenePresets` | = 1334 |
| `DecorMedium` | `HousingCatalogEntryModelScenePresets` | = 1335 |
| `DecorLarge` | `HousingCatalogEntryModelScenePresets` | = 1336 |
| `DecorHuge` | `HousingCatalogEntryModelScenePresets` | = 1337 |
| `DecorCeiling` | `HousingCatalogEntryModelScenePresets` | = 1338 |
| `DecorWall` | `HousingCatalogEntryModelScenePresets` | = 1339 |
| `DecorFlat` | `HousingCatalogEntryModelScenePresets` | = 1318 |
| `DecorHorizontalSurface` | `HousingCatalogEntryModelScenePresets` | = 1452 |

### HousingCatalogEntrySize

*Enumeration* · 6 values, 0..69

Access values as `Enum.HousingCatalogEntrySize.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingCatalogEntrySize` | = 0 |
| `Tiny` | `HousingCatalogEntrySize` | = 65 |
| `Small` | `HousingCatalogEntrySize` | = 66 |
| `Medium` | `HousingCatalogEntrySize` | = 67 |
| `Large` | `HousingCatalogEntrySize` | = 68 |
| `Huge` | `HousingCatalogEntrySize` | = 69 |

### HousingCatalogEntryType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingCatalogEntryType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `HousingCatalogEntryType` | = 0 |
| `Decor` | `HousingCatalogEntryType` | = 1 |
| `Room` | `HousingCatalogEntryType` | = 2 |

### HousingCatalogSortType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingCatalogSortType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DateAdded` | `HousingCatalogSortType` | = 0 |
| `Alphabetical` | `HousingCatalogSortType` | = 1 |

### HousingCatalogConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `HOUSING_CATALOG_FEATURED_CATEGORY_ID` | `number` | = `17` |
| `HOUSING_CATALOG_ALL_CATEGORY_ID` | `number` | = `18` |
| `HOUSING_CATALOG_DECOR_MODELSCENEID_DEFAULT` | `number` | = `1317` |

### HousingCatalogEntryID

*Structure*

Identifier for base entries in the catalog

Fields:

| Name | Type | Notes |
|---|---|---|
| `recordID` | `number` |  |
| `entryType` | `HousingCatalogEntryType` |  |

### HousingCatalogEntryVariantID

*Structure*

Compound Identifier for entry variant stacks in the catalog

Fields:

| Name | Type | Notes |
|---|---|---|
| `recordID` | `number` |  |
| `entryType` | `HousingCatalogEntryType` |  |
| `variantIdentifier` | `number` | Hashed value used to identify and differentiate stacks that are the same type and record, but have some variant-specific difference (e.g. dye colors) |

### HousingCatalogFilterTagGroupInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `groupID` | `number` |  |
| `groupName` | `cstring` |  |
| `tags` | `HousingCatalogFilterTagInfo[]` |  |

### HousingCatalogFilterTagInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tagID` | `number` |  |
| `tagName` | `string` |  |
| `orderIndex` | `number` |  |
| `anyAssociatedEntries` | `bool` |  |
