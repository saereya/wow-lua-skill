# TransmogrifyCollection

Namespace `C_TransmogCollection` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/transmogitemsdocumentation.lua` (FileDataID 4637273)

## Functions

### AccountCanCollectSource

```lua
C_TransmogCollection.AccountCanCollectSource(sourceID: number) -> hasItemData: bool, canCollect: bool
```

`SecretArguments=AllowedWhenUntainted`

### AreAllCollectionTypeFiltersChecked

```lua
C_TransmogCollection.AreAllCollectionTypeFiltersChecked() -> areAllCollectionTypeFiltersChecked: bool
```

### AreAllSourceTypeFiltersChecked

```lua
C_TransmogCollection.AreAllSourceTypeFiltersChecked() -> areAllSourceTypeFiltersChecked: bool
```

### CanAppearanceHaveIllusion

```lua
C_TransmogCollection.CanAppearanceHaveIllusion(appearanceID: number) -> canHaveIllusion: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClearNewAppearance

```lua
C_TransmogCollection.ClearNewAppearance(visualID: number)
```

`SecretArguments=AllowedWhenUntainted`

### ClearSearch

```lua
C_TransmogCollection.ClearSearch(searchType: TransmogSearchType) -> completed: bool
```

`SecretArguments=AllowedWhenUntainted`

### DeleteCustomSet

```lua
C_TransmogCollection.DeleteCustomSet(customSetID: number)
```

`SecretArguments=AllowedWhenUntainted`

### EndSearch

```lua
C_TransmogCollection.EndSearch()
```

### GetAllAppearanceSources

```lua
C_TransmogCollection.GetAllAppearanceSources(itemAppearanceID: number) -> itemModifiedAppearanceIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAllFactionsShown

```lua
C_TransmogCollection.GetAllFactionsShown() -> shown: bool
```

### GetAllRacesShown

```lua
C_TransmogCollection.GetAllRacesShown() -> shown: bool
```

### GetAppearanceCameraID

```lua
C_TransmogCollection.GetAppearanceCameraID(itemAppearanceID: number, variation: TransmogCameraVariation?) -> cameraID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAppearanceCameraIDBySource

```lua
C_TransmogCollection.GetAppearanceCameraIDBySource(itemModifiedAppearanceID: number, variation: TransmogCameraVariation?) -> cameraID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAppearanceInfoBySource

```lua
C_TransmogCollection.GetAppearanceInfoBySource(itemModifiedAppearanceID: number) -> info: TransmogAppearanceInfoBySourceData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAppearanceSourceDrops

```lua
C_TransmogCollection.GetAppearanceSourceDrops(itemModifiedAppearanceID: number) -> encounterInfo: TransmogAppearanceJournalEncounterInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAppearanceSourceInfo

```lua
C_TransmogCollection.GetAppearanceSourceInfo(itemModifiedAppearanceID: number) -> info: TransmogAppearanceSourceInfoData
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetAppearanceSources

```lua
C_TransmogCollection.GetAppearanceSources(appearanceID: number, categoryType: TransmogCollectionType?, transmogLocation: TransmogLocation?) -> sources: AppearanceSourceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `appearanceID` | `number` |  |
| `categoryType` | `TransmogCollectionType?` |  |
| `transmogLocation` | `TransmogLocation?` | `Mixin=TransmogLocationMixin` |

### GetArtifactAppearanceStrings

```lua
C_TransmogCollection.GetArtifactAppearanceStrings(appearanceID: number) -> name: cstring, hyperlink: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCategoryAppearances

```lua
C_TransmogCollection.GetCategoryAppearances(category: TransmogCollectionType, transmogLocation: TransmogLocation?, option: TransmogOutfitSlotOption?) -> appearances: TransmogCategoryAppearanceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `category` | `TransmogCollectionType` |  |
| `transmogLocation` | `TransmogLocation?` | `Mixin=TransmogLocationMixin` |
| `option` | `TransmogOutfitSlotOption?` |  |

### GetCategoryCollectedCount

```lua
C_TransmogCollection.GetCategoryCollectedCount(category: TransmogCollectionType) -> count: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCategoryForItem

```lua
C_TransmogCollection.GetCategoryForItem(itemModifiedAppearanceID: number) -> collectionCategory: TransmogCollectionType
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCategoryInfo

```lua
C_TransmogCollection.GetCategoryInfo(category: TransmogCollectionType) -> name: cstring, isWeapon: bool, canHaveIllusions: bool, canMainHand: bool, canOffHand: bool, canRanged: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `isWeapon` | `bool` | default `false` |
| `canHaveIllusions` | `bool` | default `false` |
| `canMainHand` | `bool` | default `false` |
| `canOffHand` | `bool` | default `false` |
| `canRanged` | `bool` | default `false` |

### GetCategoryTotal

```lua
C_TransmogCollection.GetCategoryTotal(category: TransmogCollectionType) -> total: number
```

`SecretArguments=AllowedWhenUntainted`

### GetClassFilter

```lua
C_TransmogCollection.GetClassFilter() -> classID: number
```

### GetCollectedShown

```lua
C_TransmogCollection.GetCollectedShown() -> shown: bool
```

### GetCustomSetHyperlinkFromItemTransmogInfoList

```lua
C_TransmogCollection.GetCustomSetHyperlinkFromItemTransmogInfoList(itemTransmogInfoList: ItemTransmogInfo[]) -> hyperlink: cstring
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCustomSetInfo

```lua
C_TransmogCollection.GetCustomSetInfo(customSetID: number) -> name: cstring, icon: fileID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCustomSetItemTransmogInfoList

```lua
C_TransmogCollection.GetCustomSetItemTransmogInfoList(customSetID: number) -> list: ItemTransmogInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCustomSets

```lua
C_TransmogCollection.GetCustomSets() -> customSetID: number[]
```

### GetFallbackWeaponAppearance

```lua
C_TransmogCollection.GetFallbackWeaponAppearance() -> appearanceID: number?
```

### GetFilteredCategoryCollectedCount

```lua
C_TransmogCollection.GetFilteredCategoryCollectedCount(category: TransmogCollectionType) -> count: number
```

`SecretArguments=AllowedWhenUntainted`

### GetFilteredCategoryTotal

```lua
C_TransmogCollection.GetFilteredCategoryTotal(category: TransmogCollectionType) -> total: number
```

`SecretArguments=AllowedWhenUntainted`

### GetIllusionInfo

```lua
C_TransmogCollection.GetIllusionInfo(illusionID: number) -> info: TransmogIllusionInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetIllusions

```lua
C_TransmogCollection.GetIllusions(category: TransmogCollectionType?) -> illusions: TransmogIllusionInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetIllusionStrings

```lua
C_TransmogCollection.GetIllusionStrings(illusionID: number) -> name: string, hyperlink: string, sourceText: string?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInspectItemTransmogInfoList

```lua
C_TransmogCollection.GetInspectItemTransmogInfoList() -> list: ItemTransmogInfo[]
```

`MayReturnNothing`

### GetIsAppearanceFavorite

```lua
C_TransmogCollection.GetIsAppearanceFavorite(itemAppearanceID: number) -> isFavorite: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetItemInfo

```lua
C_TransmogCollection.GetItemInfo(itemInfo: ItemInfo) -> itemAppearanceID: number, itemModifiedAppearanceID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemTransmogInfoListFromCustomSetHyperlink

```lua
C_TransmogCollection.GetItemTransmogInfoListFromCustomSetHyperlink(hyperlink: cstring) -> list: ItemTransmogInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLatestAppearance

```lua
C_TransmogCollection.GetLatestAppearance() -> visualID: number, category: TransmogCollectionType
```

`MayReturnNothing`

### GetNumMaxCustomSets

```lua
C_TransmogCollection.GetNumMaxCustomSets() -> maxCustomSets: number
```

### GetNumTransmogSources

```lua
C_TransmogCollection.GetNumTransmogSources() -> count: number
```

### GetPairedArtifactAppearance

```lua
C_TransmogCollection.GetPairedArtifactAppearance(itemModifiedAppearanceID: number) -> pairedItemModifiedAppearanceID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourceIcon

```lua
C_TransmogCollection.GetSourceIcon(itemModifiedAppearanceID: number) -> icon: fileID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourceInfo

```lua
C_TransmogCollection.GetSourceInfo(sourceID: number) -> sourceInfo: AppearanceSourceInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourceItemID

```lua
C_TransmogCollection.GetSourceItemID(itemModifiedAppearanceID: number) -> itemID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSourceRequiredHoliday

```lua
C_TransmogCollection.GetSourceRequiredHoliday(itemModifiedAppearanceID: number) -> holidayName: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetUncollectedShown

```lua
C_TransmogCollection.GetUncollectedShown() -> shown: bool
```

### GetValidAppearanceSourcesForClass

```lua
C_TransmogCollection.GetValidAppearanceSourcesForClass(appearanceID: number, classID: number, categoryType: TransmogCollectionType?, transmogLocation: TransmogLocation?) -> sources: AppearanceSourceInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `appearanceID` | `number` |  |
| `classID` | `number` |  |
| `categoryType` | `TransmogCollectionType?` |  |
| `transmogLocation` | `TransmogLocation?` | `Mixin=TransmogLocationMixin` |

### HasAnyAppearance

```lua
C_TransmogCollection.HasAnyAppearance() -> hasAnyAppearance: bool
```

### HasFavorites

```lua
C_TransmogCollection.HasFavorites() -> hasFavorites: bool
```

### IsAppearanceHiddenVisual

```lua
C_TransmogCollection.IsAppearanceHiddenVisual(appearanceID: number) -> isHiddenVisual: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCategoryValidForItem

```lua
C_TransmogCollection.IsCategoryValidForItem(category: TransmogCollectionType, itemInfo: ItemInfo) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsNewAppearance

```lua
C_TransmogCollection.IsNewAppearance(visualID: number) -> isNew: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSearchDBLoading

```lua
C_TransmogCollection.IsSearchDBLoading() -> isLoading: bool
```

### IsSearchInProgress

```lua
C_TransmogCollection.IsSearchInProgress(searchType: TransmogSearchType) -> inProgress: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSourceTypeFilterChecked

```lua
C_TransmogCollection.IsSourceTypeFilterChecked(index: luaIndex) -> checked: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSpellItemEnchantmentHiddenVisual

```lua
C_TransmogCollection.IsSpellItemEnchantmentHiddenVisual(spellItemEnchantmentID: number) -> isHiddenVisual: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsUsingDefaultFilters

```lua
C_TransmogCollection.IsUsingDefaultFilters() -> isUsingDefaultFilters: bool
```

### IsValidCustomSetName

```lua
C_TransmogCollection.IsValidCustomSetName(name: cstring) -> isApproved: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidTransmogSource

```lua
C_TransmogCollection.IsValidTransmogSource(source: TransmogSource) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

### ModifyCustomSet

```lua
C_TransmogCollection.ModifyCustomSet(customSetID: number, itemTransmogInfoList: ItemTransmogInfo[])
```

`SecretArguments=AllowedWhenUntainted`

### NewCustomSet

```lua
C_TransmogCollection.NewCustomSet(name: cstring, icon: fileID, itemTransmogInfoList: ItemTransmogInfo[]) -> customSetID: number?
```

`SecretArguments=AllowedWhenUntainted`

### PlayerCanCollectSource

```lua
C_TransmogCollection.PlayerCanCollectSource(sourceID: number) -> hasItemData: bool, canCollect: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerHasTransmog

```lua
C_TransmogCollection.PlayerHasTransmog(itemID: number, itemAppearanceModID: number) -> hasTransmog: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `itemAppearanceModID` | `number` | default `0` |

### PlayerHasTransmogByItemInfo

```lua
C_TransmogCollection.PlayerHasTransmogByItemInfo(itemInfo: ItemInfo) -> hasTransmog: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerHasTransmogItemModifiedAppearance

```lua
C_TransmogCollection.PlayerHasTransmogItemModifiedAppearance(itemModifiedAppearanceID: number) -> hasTransmog: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerKnowsSource

```lua
C_TransmogCollection.PlayerKnowsSource(sourceID: number) -> isKnown: bool
```

`SecretArguments=AllowedWhenUntainted`

### RenameCustomSet

```lua
C_TransmogCollection.RenameCustomSet(customSetID: number, name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SearchProgress

```lua
C_TransmogCollection.SearchProgress(searchType: TransmogSearchType) -> progress: number
```

`SecretArguments=AllowedWhenUntainted`

### SearchSize

```lua
C_TransmogCollection.SearchSize(searchType: TransmogSearchType) -> size: number
```

`SecretArguments=AllowedWhenUntainted`

### SetAllCollectionTypeFilters

```lua
C_TransmogCollection.SetAllCollectionTypeFilters(checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllFactionsShown

```lua
C_TransmogCollection.SetAllFactionsShown(shown: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllRacesShown

```lua
C_TransmogCollection.SetAllRacesShown(shown: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetAllSourceTypeFilters

```lua
C_TransmogCollection.SetAllSourceTypeFilters(checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetClassFilter

```lua
C_TransmogCollection.SetClassFilter(classID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCollectedShown

```lua
C_TransmogCollection.SetCollectedShown(shown: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDefaultFilters

```lua
C_TransmogCollection.SetDefaultFilters()
```

### SetIsAppearanceFavorite

```lua
C_TransmogCollection.SetIsAppearanceFavorite(itemAppearanceID: number, isFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetSearch

```lua
C_TransmogCollection.SetSearch(searchType: TransmogSearchType, searchText: string) -> completed: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetSearchAndFilterCategory

```lua
C_TransmogCollection.SetSearchAndFilterCategory(category: TransmogCollectionType)
```

`SecretArguments=AllowedWhenUntainted`

### SetSourceTypeFilter

```lua
C_TransmogCollection.SetSourceTypeFilter(index: luaIndex, checked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetUncollectedShown

```lua
C_TransmogCollection.SetUncollectedShown(shown: bool)
```

`SecretArguments=AllowedWhenUntainted`

### UpdateUsableAppearances

```lua
C_TransmogCollection.UpdateUsableAppearances()
```

## Types

### TransmogCameraVariation

*Enumeration* · 3 values, 0..1

Access values as `Enum.TransmogCameraVariation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TransmogCameraVariation` | = 0 |
| `RightShoulder` | `TransmogCameraVariation` | = 1 |
| `CloakBackpack` | `TransmogCameraVariation` | = 1 |

### TransmogAppearanceInfoBySourceData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `appearanceID` | `number` |  |
| `appearanceIsCollected` | `bool` |  |
| `sourceIsCollected` | `bool` |  |
| `sourceIsCollectedPermanent` | `bool` |  |
| `sourceIsCollectedConditional` | `bool` |  |
| `meetsTransmogPlayerCondition` | `bool` |  |
| `appearanceHasAnyNonLevelRequirements` | `bool` |  |
| `appearanceMeetsNonLevelRequirements` | `bool` |  |
| `appearanceIsUsable` | `bool` |  |
| `appearanceNumSources` | `number` |  |
| `sourceIsKnown` | `bool` |  |
| `canDisplayOnPlayer` | `bool` |  |
| `isAnySourceValidForPlayer` | `bool` |  |

### TransmogAppearanceJournalEncounterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `instance` | `string` |  |
| `instanceType` | `number` |  |
| `tiers` | `string[]` |  |
| `encounter` | `string` |  |
| `difficulties` | `string[]` |  |

### TransmogAppearanceSourceInfoData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `category` | `TransmogCollectionType` |  |
| `itemAppearanceID` | `number` |  |
| `canHaveIllusion` | `bool` |  |
| `icon` | `fileID` |  |
| `isCollected` | `bool` |  |
| `itemLink` | `string` |  |
| `transmoglink` | `string` |  |
| `sourceType` | `luaIndex?` |  |
| `itemSubclass` | `number` |  |
| `ignoreModelAttachmentChecksForIllusion` | `bool` |  |

### TransmogCategoryAppearanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `visualID` | `number` |  |
| `isCollected` | `bool` |  |
| `isFavorite` | `bool` |  |
| `isHideVisual` | `bool` |  |
| `canDisplayOnPlayer` | `bool` |  |
| `uiOrder` | `number` |  |
| `exclusions` | `number` |  |
| `isUsable` | `bool` |  |
| `hasRequiredHoliday` | `bool` |  |
| `hasActiveRequiredHoliday` | `bool` |  |
| `minIlvl` | `number` |  |
| `isValidForEquippedItem` | `bool` |  |
| `alwaysShowItem` | `bool?` | For internal testing only |

### TransmogCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `isWeapon` | `bool` | default `false` |
| `canHaveIllusions` | `bool` | default `false` |
| `canMainHand` | `bool` | default `false` |
| `canOffHand` | `bool` | default `false` |
| `canRanged` | `bool` | default `false` |

### TransmogCustomSetInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `icon` | `fileID` |  |

### TransmogIllusionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `visualID` | `number` |  |
| `sourceID` | `number` |  |
| `icon` | `fileID` |  |
| `isCollected` | `bool` |  |
| `isUsable` | `bool` |  |
| `isHideVisual` | `bool` |  |
