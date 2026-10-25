# CraftingOrderUIShared

source `interface/addons/blizzard_apidocumentationgenerated/craftingorderuishareddocumentation.lua` (FileDataID 5947576)

## Types

### CraftingOrderBucketInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `spellID` | `number` |  |
| `skillLineAbilityID` | `number` |  |
| `tipAmountAvg` | `WOWMONEY` |  |
| `tipAmountMax` | `WOWMONEY` |  |
| `numAvailable` | `number` |  |

### CraftingOrderClaimsRemainingInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `claimsRemaining` | `number` | default `0` |
| `secondsToRecharge` | `number?` |  |

### CraftingOrderCustomerCategory

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `categoryName` | `string` |  |
| `categoryID` | `number` |  |
| `uiSortOrder` | `number` |  |
| `primaryCategorySortOrder` | `number?` |  |
| `secondaryCategorySortOrder` | `number?` |  |
| `type` | `CraftingOrderCustomerCategoryType` |  |

### CraftingOrderCustomerCategoryFilters

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `primaryCategoryID` | `number?` |  |
| `secondaryCategoryID` | `number?` |  |
| `tertiaryCategoryID` | `number?` |  |

### CraftingOrderCustomerOptionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `skillLineAbilityID` | `number` |  |
| `professionID` | `number` |  |
| `skillUpSkillLineID` | `number` |  |
| `spellID` | `number` |  |
| `itemID` | `number` |  |
| `itemName` | `string` |  |
| `primaryCategoryID` | `number` |  |
| `iLvlMin` | `number` |  |
| `iLvlMax` | `number?` |  |
| `canUse` | `bool` |  |
| `bindOnPickup` | `bool` |  |
| `qualityIlvlBonuses` | `number[]?` |  |
| `craftingQualityIDs` | `number[]?` |  |
| `quality` | `ItemQuality?` |  |
| `slots` | `number?` |  |
| `level` | `number?` |  |
| `skill` | `number?` |  |
| `secondaryCategoryID` | `number?` |  |
| `tertiaryCategoryID` | `number?` |  |
| `expansionID` | `number?` |  |

### CraftingOrderCustomerSearchParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `categoryFilters` | `CraftingOrderCustomerCategoryFilters` |  |
| `searchText` | `string?` |  |
| `minLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `uncollectedOnly` | `bool` |  |
| `usableOnly` | `bool` |  |
| `upgradesOnly` | `bool` |  |
| `currentExpansionOnly` | `bool` |  |
| `includePoor` | `bool` |  |
| `includeCommon` | `bool` |  |
| `includeUncommon` | `bool` |  |
| `includeRare` | `bool` |  |
| `includeEpic` | `bool` |  |
| `includeLegendary` | `bool` |  |
| `includeArtifact` | `bool` |  |
| `isFavoritesSearch` | `bool` |  |

### CraftingOrderCustomerSearchResults

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `options` | `CraftingOrderCustomerOptionInfo[]` |  |
| `extraColumnType` | `AuctionHouseExtraColumn?` |  |

### CraftingOrderInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `orderID` | `BigUInteger` |  |
| `itemID` | `number` |  |
| `spellID` | `number` |  |
| `skillLineAbilityID` | `number` |  |
| `orderType` | `CraftingOrderType` |  |
| `orderState` | `CraftingOrderState` |  |
| `expirationTime` | `time_t` |  |
| `claimEndTime` | `time_t` |  |
| `minQuality` | `number` |  |
| `tipAmount` | `WOWMONEY` |  |
| `consortiumCut` | `WOWMONEY` |  |
| `isRecraft` | `bool` |  |
| `isFulfillable` | `bool` |  |
| `reagentState` | `CraftingOrderReagentsType` |  |
| `customerGuid` | `WOWGUID?` |  |
| `customerName` | `string?` |  |
| `crafterGuid` | `WOWGUID?` |  |
| `crafterName` | `string?` |  |
| `npcCustomerCreatureID` | `number?` |  |
| `customerNotes` | `string` |  |
| `reagents` | `CraftingOrderReagentInfo[]` |  |
| `outputItemHyperlink` | `string?` |  |
| `outputItemGUID` | `WOWGUID?` |  |
| `recraftItemHyperlink` | `string?` |  |
| `npcOrderRewards` | `CraftingOrderRewardInfo[]` |  |
| `npcCraftingOrderSetID` | `number` |  |
| `npcTreasureID` | `number` |  |

### CraftingOrderMailInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reason` | `RcoCloseReason` |  |
| `recipeName` | `string` |  |
| `commissionPaid` | `WOWMONEY?` |  |
| `crafterNote` | `string?` |  |
| `crafterGUID` | `WOWGUID?` |  |
| `crafterName` | `string?` |  |
| `customerGUID` | `WOWGUID?` |  |
| `customerName` | `string?` |  |

### CraftingOrderPersonalOrdersInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `profession` | `Profession` |  |
| `numPersonalOrders` | `number` |  |
| `professionName` | `cstring` |  |

### CraftingOrderReagentInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `reagentInfo` | `CraftingReagentInfo` |  |
| `slotIndex` | `luaIndex` |  |
| `source` | `CraftingOrderReagentSource` |  |
| `isBasicReagent` | `bool` |  |

### CraftingOrderRewardInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemLink` | `string?` |  |
| `currencyType` | `number?` |  |
| `count` | `number` |  |

### CraftingOrderSortInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `sortType` | `CraftingOrderSortType` |  |
| `reversed` | `bool` |  |

### NewCraftingOrderInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `skillLineAbilityID` | `number` |  |
| `orderType` | `CraftingOrderType` |  |
| `orderDuration` | `CraftingOrderDuration` |  |
| `tipAmount` | `WOWMONEY` |  |
| `customerNotes` | `string` |  |
| `reagentInfos` | `RegularReagentInfo[]` |  |
| `craftingReagentItems` | `CraftingReagentInfo[]` |  |
| `minCraftingQualityID` | `number?` |  |
| `orderTarget` | `string?` |  |
| `recraftItem` | `WOWGUID?` |  |

### CraftingOrderRequestCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `result` | `CraftingOrderResult` |  |
| `orderType` | `CraftingOrderType` |  |
| `displayBuckets` | `bool` |  |
| `expectMoreRows` | `bool` |  |
| `offset` | `number` |  |
| `isSorted` | `bool` |  |

### CraftingOrderRequestMyOrdersCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `result` | `CraftingOrderResult` |  |
| `expectMoreRows` | `bool` |  |
| `offset` | `number` |  |
| `isSorted` | `bool` |  |
