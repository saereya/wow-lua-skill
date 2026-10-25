# HousingCatalogUI

Namespace `C_HousingCatalog` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingcataloguidocumentation.lua` (FileDataID 6225878)

## Functions

### CreateCatalogSearcher

```lua
C_HousingCatalog.CreateCatalogSearcher() -> searcher: HousingCatalogSearcher
```

Creates a new instance of a HousingCatalog searcher; This can be used to asynchronously search/filter the HousingCatalog without affecting/being restricted by the filter state of other Housing Catalog UI displays

### DeletePreviewCartDecor

```lua
C_HousingCatalog.DeletePreviewCartDecor(decorGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### DestroyEntry

```lua
C_HousingCatalog.DestroyEntry(entryVariantID: HousingCatalogEntryVariantID, destroyAll: bool)
```

Attempt to delete the entry from storage

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `entryVariantID` | `HousingCatalogEntryVariantID` |  |
| `destroyAll` | `bool` | If true, deletes all entries within the stack; If false, will only delete one |

### GetAllFilterTagGroups

```lua
C_HousingCatalog.GetAllFilterTagGroups() -> filterTagGroups: HousingCatalogFilterTagGroupInfo[]
```

### GetAllVariantInfosForEntry

```lua
C_HousingCatalog.GetAllVariantInfosForEntry(entryID: HousingCatalogEntryID) -> variantInfos: HousingCatalogEntryVariantInfo[]
```

Returns variant info for all variants of a given catalog entry; Variants represent different visual modifications of the same base entry (ex: dyed versions)

`SecretArguments=AllowedWhenUntainted`

### GetBundleInfo

```lua
C_HousingCatalog.GetBundleInfo(bundleCatalogShopProductID: number) -> bundleInfo: HousingBundleInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCartSizeLimit

```lua
C_HousingCatalog.GetCartSizeLimit() -> cartSizeLimit: number
```

### GetCatalogCategoryAndSubcategoryNames

```lua
C_HousingCatalog.GetCatalogCategoryAndSubcategoryNames(subcategoryID: number) -> categoryName: string, subcategoryName: string
```

If found, returns the names of the parent category and the specified subcategory

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCatalogCategoryInfo

```lua
C_HousingCatalog.GetCatalogCategoryInfo(categoryID: number) -> info: HousingCatalogCategoryInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCatalogEntryInfo

```lua
C_HousingCatalog.GetCatalogEntryInfo(entryID: HousingCatalogEntryID) -> info: HousingCatalogEntryInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCatalogEntryInfoByItem

```lua
C_HousingCatalog.GetCatalogEntryInfoByItem(itemInfo: ItemInfo) -> info: HousingCatalogEntryInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemInfo` | `ItemInfo` | ItemID, name, or link of an item that grants/corresponds to a particular type of housing catalog object (ex: decor) |

### GetCatalogEntryInfoByRecordID

```lua
C_HousingCatalog.GetCatalogEntryInfoByRecordID(entryType: HousingCatalogEntryType, recordID: number) -> info: HousingCatalogEntryInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCatalogEntryRefundTimeStampByRecordID

```lua
C_HousingCatalog.GetCatalogEntryRefundTimeStampByRecordID(entryType: HousingCatalogEntryType, recordID: number) -> refundTimeStamp: time_t?
```

`SecretArguments=AllowedWhenUntainted`

### GetCatalogEntryVariantInfo

```lua
C_HousingCatalog.GetCatalogEntryVariantInfo(entryVariantID: HousingCatalogEntryVariantID) -> info: HousingCatalogEntryVariantInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCatalogSubcategoryInfo

```lua
C_HousingCatalog.GetCatalogSubcategoryInfo(subcategoryID: number) -> info: HousingCatalogSubcategoryInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetDecorMaxOwnedCount

```lua
C_HousingCatalog.GetDecorMaxOwnedCount() -> maxOwnedCount: number
```

Returns the maximum total number of decor that can be in storage/in the house chest; Note that not all decor entries in storage count towards this limit (see GetDecorTotalOwnedCount)

### GetDecorTotalOwnedCount

```lua
C_HousingCatalog.GetDecorTotalOwnedCount() -> totalOwnedCount: number, exemptDecorCount: number
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `totalOwnedCount` | `number` | The total number of owned decor in storage, including both exempt and non-exempt decor |
| `exemptDecorCount` | `number` | The number of decor that do not count against the max storage limit |

### GetDestroyableInstanceCount

```lua
C_HousingCatalog.GetDestroyableInstanceCount(entryVariantID: HousingCatalogEntryVariantID) -> destroyableInstanceCount: number
```

Returns the number of instances that can be to be destroyed in storage; These instances count towards the max storage limit

`SecretArguments=AllowedWhenUntainted`

### GetFeaturedBundles

```lua
C_HousingCatalog.GetFeaturedBundles() -> bundleInfos: HousingBundleInfo[]
```

### GetFeaturedSmallProducts

```lua
C_HousingCatalog.GetFeaturedSmallProducts() -> infos: HousingFeaturedSmallProductInfo[]
```

### GetMarketInfoForDecor

```lua
C_HousingCatalog.GetMarketInfoForDecor(decorID: number) -> marketInfo: HousingMarketInfo?
```

Returns market info for a specific decor. This is decor-only for now but should be extended to support entry type and recordID generically

`SecretArguments=AllowedWhenUntainted`

### HasFeaturedEntries

```lua
C_HousingCatalog.HasFeaturedEntries() -> hasEntries: bool
```

### HousingMarketActionAddToCart

```lua
C_HousingCatalog.HousingMarketActionAddToCart(productID: number, withPreview: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### HousingMarketActionClearCart

```lua
C_HousingCatalog.HousingMarketActionClearCart()
```

`HasRestrictions`

### HousingMarketActionRemoveFromCart

```lua
C_HousingCatalog.HousingMarketActionRemoveFromCart(productID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### HousingMarketActionViewBundle

```lua
C_HousingCatalog.HousingMarketActionViewBundle(productID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### HousingMarketActionViewInStore

```lua
C_HousingCatalog.HousingMarketActionViewInStore(productID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### IsPreviewCartItemShown

```lua
C_HousingCatalog.IsPreviewCartItemShown(decorGUID: WOWGUID) -> isShown: bool
```

`SecretArguments=AllowedWhenUntainted`

### PromotePreviewDecor

```lua
C_HousingCatalog.PromotePreviewDecor(decorID: number, previewDecorGUID: WOWGUID) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestHousingMarketInfoRefresh

```lua
C_HousingCatalog.RequestHousingMarketInfoRefresh()
```

### RequestHousingMarketRefundInfo

```lua
C_HousingCatalog.RequestHousingMarketRefundInfo()
```

### SearchCatalogCategories

```lua
C_HousingCatalog.SearchCatalogCategories(searchParams: HousingCategorySearchInfo) -> categoryIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### SearchCatalogSubcategories

```lua
C_HousingCatalog.SearchCatalogSubcategories(searchParams: HousingCategorySearchInfo) -> subcategoryIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### SetPreviewCartItemShown

```lua
C_HousingCatalog.SetPreviewCartItemShown(decorGUID: WOWGUID, shown: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### HOUSING_CATALOG_CATEGORY_UPDATED

```lua
HOUSING_CATALOG_CATEGORY_UPDATED(categoryID: number)
```

`UniqueEvent`

### HOUSING_CATALOG_SUBCATEGORY_UPDATED

```lua
HOUSING_CATALOG_SUBCATEGORY_UPDATED(subcategoryID: number)
```

`UniqueEvent`

### HOUSING_DECOR_ADD_TO_PREVIEW_LIST

```lua
HOUSING_DECOR_ADD_TO_PREVIEW_LIST(previewItemData: HousingPreviewItemData)
```

`SynchronousEvent`

### HOUSING_DECOR_PREVIEW_LIST_REMOVE_FROM_WORLD

```lua
HOUSING_DECOR_PREVIEW_LIST_REMOVE_FROM_WORLD(decorGUID: WOWGUID)
```

`SynchronousEvent`

### HOUSING_DECOR_PREVIEW_LIST_UPDATED

```lua
HOUSING_DECOR_PREVIEW_LIST_UPDATED()
```

`SynchronousEvent`

### HOUSING_REFUND_LIST_UPDATED

```lua
HOUSING_REFUND_LIST_UPDATED()
```

`SynchronousEvent`

### HOUSING_STORAGE_ENTRY_UPDATED

```lua
HOUSING_STORAGE_ENTRY_UPDATED(entryVariantID: HousingCatalogEntryVariantID)
```

`UniqueEvent`

### HOUSING_STORAGE_UPDATED

```lua
HOUSING_STORAGE_UPDATED()
```

`UniqueEvent`

## Types

### HousingBundleDecorEntryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `decorID` | `number` |  |
| `quantity` | `number` |  |

### HousingBundleInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `productID` | `number` |  |
| `price` | `number` |  |
| `originalPrice` | `number?` |  |
| `nonDecorProducts` | `number[]` |  |
| `decorEntries` | `HousingBundleDecorEntryInfo[]` |  |
| `canPreview` | `bool` | default `true`; Bundles containing non-decor items cannot be previewed |

### HousingCatalogCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `orderIndex` | `number` |  |
| `name` | `cstring?` |  |
| `icon` | `textureAtlas?` |  |
| `subcategoryIDs` | `number[]` |  |
| `anyStoredEntries` | `bool` | True if the player owns anything that falls under this category |

### HousingCatalogEntryInfo

*Structure*

Base information about an object in the Catalog; For info for a specific owned stack of this object, see HousingCatalogEntryVariantInfo

Fields:

| Name | Type | Notes |
|---|---|---|
| `recordID` | `number` |  |
| `entryType` | `HousingCatalogEntryType` |  |
| `itemID` | `number?` |  |
| `name` | `cstring` |  |
| `asset` | `ModelAsset?` | 3D model asset for displaying in the UI; May be nil if the entry doesn't have a model, or has one that isn't supported by UI model scenes |
| `iconTexture` | `FileAsset?` | Entry icon in the form of a texture file; Catalog entries should have either this OR an iconAtlas set |
| `iconAtlas` | `textureAtlas?` | Entry icon in the form a texture atlas element; Catalog entries should have either this OR an iconTexture set |
| `uiModelSceneID` | `number?` | Specific UI model scene ID to use when previewing this entry's 3D model; If not set, the default catalog model scene is used |
| `categoryIDs` | `number[]` |  |
| `subcategoryIDs` | `number[]` |  |
| `dataTagsByID` | `LuaValueVariant` | Simple localized 'tag' strings that are primarily used for things like categorization and filtering |
| `size` | `HousingCatalogEntrySize` |  |
| `placementCost` | `number` | How much of the applicable budget placing this entry would cost (if any) |
| `totalNumStored` | `number` | The total number of instances of this entry that exist in storage across all variants; Does not include unredeemed instances (see remainingRedeemable) |
| `remainingRedeemable` | `number` | The number of unredeemed instances of this entry that exist in storage; Some auto-awarded housing objects are granted in this 'lazily-instantiated' way, and will be 'redeemed' on first being placed |
| `totalNumPlaced` | `number` | The total number of instances of this entry that have been placed across all of the player's houses and plots, across all variants |
| `destroyableInstanceCount` | `number` | The number of instances that can be destroyed for this entry. |
| `isUniqueTrophy` | `bool` | This decor is flagged to display as a unique trophy item. |
| `isAllowedOutdoors` | `bool` | True if this entry is something that is allowed to be placed outside, within a plot |
| `isAllowedIndoors` | `bool` | True if this entry is something that is allowed to be placed indoors, within a house interior |
| `canCustomize` | `bool` | True if this entry is something that can be customized; Kinds of customization vary depending on the entry type |
| `isPrefab` | `bool` |  |
| `quality` | `ItemQuality?` |  |
| `firstAcquisitionBonus` | `number` | House XP that can be gained upon acquiring this entry for the first time |
| `sourceText` | `cstring` | Describes specific sources this entry may be gained from; Faction-specific sources may or may not be included based on the current player's faction |

### HousingCatalogEntryVariantInfo

*Structure*

Represents a single stack of instances of an object in the Catalog, that are all of a specific variation; For example, a stack of undyed chairs, or blue-dyed tables

Fields:

| Name | Type | Notes |
|---|---|---|
| `entryVariantID` | `HousingCatalogEntryVariantID` |  |
| `numStored` | `number` | The number of instances of this specific variant that exist in storage |
| `dyeSlots` | `HousingDecorDyeSlot[]` | Dye slot information for this variant; Empty for entries that can't be dyed |

### HousingCatalogSubcategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `orderIndex` | `number` |  |
| `parentCategoryID` | `number` |  |
| `name` | `cstring?` |  |
| `icon` | `textureAtlas?` |  |
| `anyStoredEntries` | `bool` | True if the player owns anything that falls under this subcategory |

### HousingCategorySearchInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `withStoredEntriesOnly` | `bool` | default `false`; If true, search will only return categories/subcategories that the player has something stored under |
| `includeFeaturedCategory` | `bool` | default `false` |
| `editorModeContext` | `HouseEditorMode?` | If set, will restrict results to only categories associated with/used by this Editor Mode |

### HousingFeaturedSmallProductInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `entryVariantID` | `HousingCatalogEntryVariantID?` |  |
| `productID` | `number` |  |
| `price` | `number` |  |
| `originalPrice` | `number?` |  |
| `canPreview` | `bool` |  |

### HousingMarketInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `price` | `number` |  |
| `productID` | `number` |  |
| `bundleIDs` | `number[]` |  |

### HousingPreviewItemData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `decorGUID` | `WOWGUID?` |  |
| `productID` | `number?` |  |
| `bundleCatalogShopProductID` | `number?` |  |
| `isBundleParent` | `bool` |  |
| `isBundleChild` | `bool` |  |
| `id` | `number` |  |
| `decorID` | `number` |  |
| `name` | `string` |  |
| `icon` | `number` |  |
| `price` | `number` |  |
| `salePrice` | `number?` |  |
