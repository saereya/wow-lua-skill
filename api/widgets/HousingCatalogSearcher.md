# HousingCatalogSearcher

Widget methods (`HousingCatalogSearcherAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingcatalogsearcherapidocumentation.lua` (FileDataID 7153761)

## Methods

### GetAllSearchItems

```lua
HousingCatalogSearcher:GetAllSearchItems() -> matchingEntryVariantIDs: HousingCatalogEntryVariantID[]
```

Returns all catalog entries being searched (note these are NOT search results, this is the source collection of what's being searched)

### GetCatalogSearchResults

```lua
HousingCatalogSearcher:GetCatalogSearchResults() -> matchingEntryVariantIDs: HousingCatalogEntryVariantID[]
```

Returns the most recent search result entries

### GetEditorModeContext

```lua
HousingCatalogSearcher:GetEditorModeContext() -> editorModeContext: HouseEditorMode?
```

### GetFilteredCategoryID

```lua
HousingCatalogSearcher:GetFilteredCategoryID() -> categoryID: number?
```

### GetFilteredSubcategoryID

```lua
HousingCatalogSearcher:GetFilteredSubcategoryID() -> subcategoryID: number?
```

### GetFilterTagStatus

```lua
HousingCatalogSearcher:GetFilterTagStatus(groupID: number, tagID: number) -> active: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetNumSearchItems

```lua
HousingCatalogSearcher:GetNumSearchItems() -> numSearchItems: number
```

Returns the total number of entries being searched through

### GetSearchCount

```lua
HousingCatalogSearcher:GetSearchCount() -> searchCount: number
```

Returns the total number of owned instances across all most recent search result entries

### GetSearchText

```lua
HousingCatalogSearcher:GetSearchText() -> searchText: string?
```

### GetSortType

```lua
HousingCatalogSearcher:GetSortType() -> sortType: HousingCatalogSortType
```

### IsAllowedIndoorsActive

```lua
HousingCatalogSearcher:IsAllowedIndoorsActive() -> isActive: bool
```

### IsAllowedOutdoorsActive

```lua
HousingCatalogSearcher:IsAllowedOutdoorsActive() -> isActive: bool
```

### IsBaseVariantOnlyActive

```lua
HousingCatalogSearcher:IsBaseVariantOnlyActive() -> isActive: bool
```

### IsCollectedActive

```lua
HousingCatalogSearcher:IsCollectedActive() -> isActive: bool
```

### IsCustomizableOnlyActive

```lua
HousingCatalogSearcher:IsCustomizableOnlyActive() -> isActive: bool
```

### IsFirstAcquisitionBonusOnlyActive

```lua
HousingCatalogSearcher:IsFirstAcquisitionBonusOnlyActive() -> isActive: bool
```

### IsSearchInProgress

```lua
HousingCatalogSearcher:IsSearchInProgress() -> isSearchInProgress: bool
```

### IsStoredOnlyActive

```lua
HousingCatalogSearcher:IsStoredOnlyActive() -> isActive: bool
```

### IsUncollectedActive

```lua
HousingCatalogSearcher:IsUncollectedActive() -> isActive: bool
```

### RunSearch

```lua
HousingCatalogSearcher:RunSearch()
```

Run search with all current param values

### SetAllInFilterTagGroup

```lua
HousingCatalogSearcher:SetAllInFilterTagGroup(groupID: number, active: bool)
```

Set the toggle state of all filter tags within a specific group; If active, only entries that match Any of the tags in the group will be included in search results

`SecretArguments=AllowedWhenUntainted`

### SetAllowedIndoors

```lua
HousingCatalogSearcher:SetAllowedIndoors(isActive: bool)
```

Search parameter; If true, entries that can be placed in house interiors will be included in the search; Note many decor objects can be placed both indoors and outdoors, so having only this toggled on may still include decor that can also be placed outdoors

`SecretArguments=AllowedWhenUntainted`

### SetAllowedOutdoors

```lua
HousingCatalogSearcher:SetAllowedOutdoors(isActive: bool)
```

Search parameter; If true, entries that can be placed outside in plots will be included in the search; Note many decor objects can be placed both indoors and outdoors, so having only this toggled on may still include decor that can also be placed indoors

`SecretArguments=AllowedWhenUntainted`

### SetAutoUpdateOnParamChanges

```lua
HousingCatalogSearcher:SetAutoUpdateOnParamChanges(autoUpdateActive: bool)
```

If true, searcher automatically updates results whenever search param values are changed

`SecretArguments=AllowedWhenUntainted`

### SetBaseVariantOnly

```lua
HousingCatalogSearcher:SetBaseVariantOnly(isActive: bool)
```

Search parameter; If true, only the base variant of each decor entry will be included

`SecretArguments=AllowedWhenUntainted`

### SetCollected

```lua
HousingCatalogSearcher:SetCollected(isActive: bool)
```

Search parameter; If true, includes all owned entries, including those that are in storage OR placed in an owned house or plot; See IsStoredOnlyActive for a more exclusive toggle

`SecretArguments=AllowedWhenUntainted`

### SetCustomizableOnly

```lua
HousingCatalogSearcher:SetCustomizableOnly(isActive: bool)
```

Search parameter; If true, catalog entries that cannot be customized (ie dyed) will be excluded from the search

`SecretArguments=AllowedWhenUntainted`

### SetEditorModeContext

```lua
HousingCatalogSearcher:SetEditorModeContext(editorModeContext: HouseEditorMode?)
```

Search parameter; If set, limits search results to only entries that are used/valid in the specified editor mode

`SecretArguments=AllowedWhenUntainted`

### SetFilteredCategoryID

```lua
HousingCatalogSearcher:SetFilteredCategoryID(categoryID: number?)
```

Search parameter; If set, limits search results to only those within the specified category

`SecretArguments=AllowedWhenUntainted`

### SetFilteredSubcategoryID

```lua
HousingCatalogSearcher:SetFilteredSubcategoryID(subcategoryID: number?)
```

Search parameter; If set, limits search results to only those within the specified subcategory

`SecretArguments=AllowedWhenUntainted`

### SetFilterTagStatus

```lua
HousingCatalogSearcher:SetFilterTagStatus(groupID: number, tagID: number, active: bool)
```

Set the toggle state of a single filter tag within a specific group

`SecretArguments=AllowedWhenUntainted`

### SetFirstAcquisitionBonusOnly

```lua
HousingCatalogSearcher:SetFirstAcquisitionBonusOnly(isActive: bool)
```

Search parameter; If true, excludes any entries that do not reward house xp when acquired for the first time

`SecretArguments=AllowedWhenUntainted`

### SetResultsUpdatedCallback

```lua
HousingCatalogSearcher:SetResultsUpdatedCallback(callback: HousingCatalogSearchResultsUpdatedCallback)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearchText

```lua
HousingCatalogSearcher:SetSearchText(searchText: string?)
```

Search parameter; If set, multiple text fields are checked for instances of the text, including name, category, subcategory, and data tags

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `searchText` | `string?` | Supports advanced search tokens ('"' '-' and '\|'), case and accent insensitive; Set nil to clear out the search text |

### SetSortType

```lua
HousingCatalogSearcher:SetSortType(sortType: HousingCatalogSortType)
```

`SecretArguments=AllowedWhenUntainted`

### SetStoredOnly

```lua
HousingCatalogSearcher:SetStoredOnly(isActive: bool)
```

Search parameter; If true, only entries that you have instances of available in storage will be included; This does not include entries that you own but have all been placed in a house; See IsCollectedActive for param that includes placed entries

`SecretArguments=AllowedWhenUntainted`

### SetUncollected

```lua
HousingCatalogSearcher:SetUncollected(isActive: bool)
```

Search parameter; If true, includes entries that are not owned, meaning not available in storage nor placed in any owned houses or plots

`SecretArguments=AllowedWhenUntainted`

### ToggleAllowedIndoors

```lua
HousingCatalogSearcher:ToggleAllowedIndoors()
```

### ToggleAllowedOutdoors

```lua
HousingCatalogSearcher:ToggleAllowedOutdoors()
```

### ToggleBaseVariantOnly

```lua
HousingCatalogSearcher:ToggleBaseVariantOnly()
```

### ToggleCollected

```lua
HousingCatalogSearcher:ToggleCollected()
```

### ToggleCustomizableOnly

```lua
HousingCatalogSearcher:ToggleCustomizableOnly()
```

### ToggleFilterTag

```lua
HousingCatalogSearcher:ToggleFilterTag(groupID: number, tagID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ToggleFirstAcquisitionBonusOnly

```lua
HousingCatalogSearcher:ToggleFirstAcquisitionBonusOnly()
```

### ToggleStoredOnly

```lua
HousingCatalogSearcher:ToggleStoredOnly()
```

### ToggleUncollected

```lua
HousingCatalogSearcher:ToggleUncollected()
```

## Types

### HousingCatalogSearchResultsUpdatedCallback

*CallbackType*
