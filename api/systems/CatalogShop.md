# CatalogShop

Namespace `C_CatalogShop` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/catalogshopdocumentation.lua` (FileDataID 6686505)

## Functions

### BulkPurchaseProducts

```lua
C_CatalogShop.BulkPurchaseProducts(productIDs: number[]) -> canPurchaseProducts: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### BulkRefundDecors

```lua
C_CatalogShop.BulkRefundDecors(decorGUIDs: WOWGUID[])
```

`SecretArguments=AllowedWhenUntainted`

### CloseCatalogShopInteraction

```lua
C_CatalogShop.CloseCatalogShopInteraction()
```

### ConfirmHousingPurchase

```lua
C_CatalogShop.ConfirmHousingPurchase(productIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### FindBestCurrencyProductForNeededAmount

```lua
C_CatalogShop.FindBestCurrencyProductForNeededAmount(vcCurrencyCode: string, amountNeeded: number) -> vcProductID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetAvailableCategoryIDs

```lua
C_CatalogShop.GetAvailableCategoryIDs() -> categoryIDs: number[]
```

### GetAvailableTransmogRaceInfos

```lua
C_CatalogShop.GetAvailableTransmogRaceInfos() -> raceIDs: AvailableRaceInfo[]
```

### GetCatalogShopProductDisplayInfo

```lua
C_CatalogShop.GetCatalogShopProductDisplayInfo(catalogShopProductID: number) -> item: CatalogShopProductDisplayInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetCategoryInfo

```lua
C_CatalogShop.GetCategoryInfo(categoryID: number) -> categoryInfo: CatalogShopCategoryInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetCategorySectionInfo

```lua
C_CatalogShop.GetCategorySectionInfo(categoryID: number, sectionID: number) -> sectionInfo: CatalogShopSectionInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetFailureInfo

```lua
C_CatalogShop.GetFailureInfo() -> errorResultEnum: StoreError?, errorResultRaw: number?
```

### GetFirstCategoryByProductID

```lua
C_CatalogShop.GetFirstCategoryByProductID(productID: number) -> categoryInfo: CatalogShopCategoryInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetNewProducts

```lua
C_CatalogShop.GetNewProducts() -> newProducts: number[]
```

### GetProductAvailabilityTimeRemainingSecs

```lua
C_CatalogShop.GetProductAvailabilityTimeRemainingSecs(catalogShopProductID: number) -> timeRemainingSecs: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetProductIDsForBundle

```lua
C_CatalogShop.GetProductIDsForBundle(bundleProductID: number) -> childIDs: CatalogShopBundleChildInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetProductIDsForCategory

```lua
C_CatalogShop.GetProductIDsForCategory(categoryID: number) -> productIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetProductIDsForCategorySection

```lua
C_CatalogShop.GetProductIDsForCategorySection(categoryID: number, sectionID: number) -> productIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetProductInfo

```lua
C_CatalogShop.GetProductInfo(productID: number) -> productInfo: CatalogShopProductInfo?
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetProductSortOrder

```lua
C_CatalogShop.GetProductSortOrder(categoryID: number, sectionID: number, productID: number) -> sortOrder: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetRefundableDecors

```lua
C_CatalogShop.GetRefundableDecors(productIdFilterOpt: number?) -> refundableDecorInfos: RefundableDecorInfo[], minTimeRemainingSeconds: time_t
```

`SecretArguments=AllowedWhenUntainted`

### GetSectionIDsForCategory

```lua
C_CatalogShop.GetSectionIDsForCategory(categoryID: number) -> sectionIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSpellVisualInfoForMount

```lua
C_CatalogShop.GetSpellVisualInfoForMount(spellVisualID: number) -> spellVisualInfo: CatalogShopSpellVisualInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetVCProductInfos

```lua
C_CatalogShop.GetVCProductInfos() -> vcProductInfos: CatalogShopVCProductInfo[]
```

### GetVirtualCurrencyBalance

```lua
C_CatalogShop.GetVirtualCurrencyBalance(currencyCode: string) -> balance: string?
```

`SecretArguments=AllowedWhenUntainted`

### HasNewProducts

```lua
C_CatalogShop.HasNewProducts() -> hasNewProducts: bool
```

### IsProductIncludedInAnyBundle

```lua
C_CatalogShop.IsProductIncludedInAnyBundle(productID: number) -> isIncludedInAnyBundle: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsShop2Enabled

```lua
C_CatalogShop.IsShop2Enabled() -> value: bool?
```

### OnLegalDisclaimerClicked

```lua
C_CatalogShop.OnLegalDisclaimerClicked(catalogShopProductID: number)
```

`SecretArguments=AllowedWhenUntainted`

### OnLegalPersonalizedOptOutClicked

```lua
C_CatalogShop.OnLegalPersonalizedOptOutClicked()
```

### OpenCatalogShopInteractionFromHouse

```lua
C_CatalogShop.OpenCatalogShopInteractionFromHouse() -> shoppingSessionUUIDStr: string
```

### OpenCatalogShopInteractionFromShop

```lua
C_CatalogShop.OpenCatalogShopInteractionFromShop() -> shoppingSessionUUIDStr: string
```

### ProductDisplayedTelemetry

```lua
C_CatalogShop.ProductDisplayedTelemetry(categoryId: number, sectionId: number, catalogShopProductID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ProductSelectedTelemetry

```lua
C_CatalogShop.ProductSelectedTelemetry(categoryId: number, sectionId: number, catalogShopProductID: number, wasCodeSelection: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### PurchaseProduct

```lua
C_CatalogShop.PurchaseProduct(productID: number) -> canPurchase: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RefreshRefundableDecors

```lua
C_CatalogShop.RefreshRefundableDecors()
```

### RefreshVirtualCurrencyBalance

```lua
C_CatalogShop.RefreshVirtualCurrencyBalance(currencyCode: string)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowHousingWarning

```lua
C_CatalogShop.ShouldShowHousingWarning() -> shouldShowHousingWarning: bool
```

### StartHousingVCPurchaseConfirmation

```lua
C_CatalogShop.StartHousingVCPurchaseConfirmation(productID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### BULK_PURCHASE_RESULT_RECEIVED

```lua
BULK_PURCHASE_RESULT_RECEIVED(result: BulkPurchaseResult, productResults: BulkPurchaseIndividualProductResult[], bestTopUpProductID: number?, totalCost: number?)
```

`SynchronousEvent`

### BULK_REFUND_RESULT_RECEIVED

```lua
BULK_REFUND_RESULT_RECEIVED(result: BulkRefundResult)
```

`SynchronousEvent`

### CATALOG_SHOP_ADD_PENDING_PRODUCT

```lua
CATALOG_SHOP_ADD_PENDING_PRODUCT(productID: number)
```

`SynchronousEvent`

### CATALOG_SHOP_DATA_REFRESH

```lua
CATALOG_SHOP_DATA_REFRESH(shoppingSessionUUIDStr: string?)
```

`SynchronousEvent`

### CATALOG_SHOP_DISABLED

```lua
CATALOG_SHOP_DISABLED()
```

`SynchronousEvent`

### CATALOG_SHOP_FETCH_FAILURE

```lua
CATALOG_SHOP_FETCH_FAILURE(shoppingSessionUUIDStr: string?)
```

`SynchronousEvent`

### CATALOG_SHOP_FETCH_SUCCESS

```lua
CATALOG_SHOP_FETCH_SUCCESS(shoppingSessionUUIDStr: string?)
```

`SynchronousEvent`

### CATALOG_SHOP_OPEN_SIMPLE_CHECKOUT

```lua
CATALOG_SHOP_OPEN_SIMPLE_CHECKOUT(checkoutID: number)
```

`SynchronousEvent`

### CATALOG_SHOP_PURCHASE_SUCCESS

```lua
CATALOG_SHOP_PURCHASE_SUCCESS(productID: number)
```

`SynchronousEvent`

### CATALOG_SHOP_REBUILD_SCROLL_BOX

```lua
CATALOG_SHOP_REBUILD_SCROLL_BOX()
```

`SynchronousEvent`

### CATALOG_SHOP_REFUNDABLE_DECORS_UPDATED

```lua
CATALOG_SHOP_REFUNDABLE_DECORS_UPDATED()
```

`SynchronousEvent`

### CATALOG_SHOP_REMOVE_PENDING_PRODUCT

```lua
CATALOG_SHOP_REMOVE_PENDING_PRODUCT(productID: number)
```

`SynchronousEvent`

### CATALOG_SHOP_RESULT_ERROR

```lua
CATALOG_SHOP_RESULT_ERROR()
```

`SynchronousEvent`

### CATALOG_SHOP_SPECIFIC_PRODUCT_REFRESH

```lua
CATALOG_SHOP_SPECIFIC_PRODUCT_REFRESH(productID: number)
```

`SynchronousEvent`

### CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE

```lua
CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE(currencyCode: string, balance: string)
```

`SynchronousEvent`

### CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE_FAILURE

```lua
CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE_FAILURE(currencyCode: string)
```

`SynchronousEvent`

### SET_SEEN_PRODUCTS

```lua
SET_SEEN_PRODUCTS(productIds: number[])
```

`SynchronousEvent`

### SHOW_NEW_PRODUCT_NOTIFICATION

```lua
SHOW_NEW_PRODUCT_NOTIFICATION()
```

`SynchronousEvent`

## Types

### AvailableRaceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `raceID` | `number` |  |
| `displayName` | `string` |  |

### BulkPurchaseIndividualProductResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `recordId` | `number` |  |
| `parentProductId` | `number?` |  |
| `entitlementId` | `string` |  |
| `externalTransactionId` | `string` |  |
| `status` | `SimpleOrderStatus` |  |

### CatalogShopBundleChildInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `childProductID` | `number` |  |
| `displayOrder` | `number` |  |
| `quantityInBundle` | `number` |  |

### CatalogShopCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `displayName` | `string` |  |
| `iconTexture` | `string` |  |
| `linkTag` | `string` |  |
| `isDisabled` | `bool` |  |
| `showPersistentRefundButton` | `bool` |  |

### CatalogShopProductDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `defaultPreviewModelSceneID` | `number` |  |
| `defaultCardModelSceneID` | `number` |  |
| `defaultWideCardModelSceneID` | `number` |  |
| `itemID` | `number` |  |
| `overridePreviewModelSceneID` | `number?` |  |
| `overrideCardModelSceneID` | `number?` |  |
| `overrideWideCardModelSceneID` | `number?` |  |
| `creatureDisplayInfoIDs` | `number[]` |  |
| `spellVisualIDs` | `number[]` |  |
| `mainHandItemModifiedAppearanceID` | `number?` |  |
| `offHandItemModifiedAppearanceID` | `number?` |  |
| `itemModifiedAppearanceIDs` | `number[]` |  |
| `iconFileDataID` | `number?` |  |
| `iconTextureKit` | `textureKit?` |  |
| `productType` | `string?` |  |
| `itemDescription` | `string?` |  |
| `hasUnknownLicense` | `bool` |  |
| `productPMTURL` | `string?` |  |
| `additionalProductPMTURLs` | `string[]` |  |
| `otherProductImageAtlasName` | `string?` |  |
| `otherProductGameTitleBaseTag` | `string?` |  |
| `otherProductGameType` | `string?` |  |
| `customLoopingSoundStart` | `number?` |  |
| `customLoopingSoundMiddle` | `number?` |  |
| `customLoopingSoundEnd` | `number?` |  |
| `specialActorID_1` | `string?` |  |
| `specialActorID_2` | `string?` |  |
| `specialActorID_3` | `string?` |  |
| `specialActorID_4` | `string?` |  |
| `specialActorID_5` | `string?` |  |
| `gameFlavorID` | `number?` |  |
| `decorFileDataID` | `number?` |  |
| `quantity` | `number?` |  |
| `houseTextureAtlas` | `textureAtlas?` |  |

### CatalogShopProductInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `catalogShopProductID` | `number` |  |
| `name` | `string` |  |
| `type` | `string?` |  |
| `description` | `string` |  |
| `iconTexture` | `string` |  |
| `isFullyOwned` | `bool` |  |
| `isPurchasePending` | `bool` |  |
| `refundable` | `bool` |  |
| `price` | `string` |  |
| `originalPrice` | `string` |  |
| `discountPercentage` | `number` |  |
| `itemID` | `number` |  |
| `mountID` | `number` |  |
| `mountTypeName` | `string` |  |
| `speciesID` | `number` |  |
| `transmogSetID` | `number` |  |
| `itemModifiedAppearanceID` | `number` |  |
| `subItems` | `CatalogShopSubItemInfo[]` |  |
| `subItemsLoaded` | `bool` |  |
| `backgroundTexture` | `string` |  |
| `foregroundTexture` | `string?` |  |
| `smallCardBGTexture` | `string?` |  |
| `smallCardFGTexture` | `string?` |  |
| `wideCardBGTexture` | `string?` |  |
| `wideCardFGTexture` | `string?` |  |
| `previewIconTexture` | `string?` |  |
| `optionalWideCardBackgroundTexture` | `string?` |  |
| `isBundle` | `bool` |  |
| `bundleChildrenSize` | `number` |  |
| `licenseTermType` | `number` |  |
| `licenseTermDuration` | `number` |  |
| `virtualCurrencies` | `CatalogShopVirtualCurrency[]` |  |
| `isHidden` | `bool` |  |
| `isMystery` | `bool` |  |
| `hasPendingOrders` | `bool` |  |
| `numBundleDetailCards` | `number` |  |
| `isDynamicallyDiscounted` | `bool` |  |
| `shouldShowOriginalPrice` | `bool` |  |
| `wideCardBGOverrideProductURL` | `string?` |  |
| `previewBGOverrideProductURL` | `string?` |  |
| `previewSmallBGOverrideProductURL` | `string?` |  |
| `decorQuantity` | `DecorQuantity?` |  |
| `isVCProduct` | `bool` |  |
| `containsHousingItem` | `bool` |  |
| `deferredGameTimeDays` | `number` |  |

### CatalogShopSectionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `displayName` | `string` |  |
| `parentCatalogShopCategoryInfoID` | `number?` |  |
| `cardType` | `string?` |  |
| `scrollGridSize` | `number?` |  |
| `shouldShowRecommendationOptOutDisclaimer` | `bool` |  |

### CatalogShopSpellVisualInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `animID` | `number?` |  |
| `spellVisualKitID` | `number?` |  |

### CatalogShopSubItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `itemID` | `number` |  |
| `itemAppearanceID` | `number` |  |
| `invType` | `string` |  |
| `quality` | `ItemQuality` |  |

### CatalogShopVCProductInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `vcProductID` | `number` |  |

### CatalogShopVirtualCurrency

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `amount` | `number` |  |
| `currencyCode` | `string` |  |

### DecorQuantity

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `placedQuantity` | `number` |  |
| `storedQuantity` | `number` |  |

### RefundableDecorInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `decorGUID` | `WOWGUID` |  |
| `timeRemainingSeconds` | `time_t` |  |
| `name` | `string` |  |
| `price` | `string` |  |
