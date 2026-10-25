# AuctionHouse

Namespace `C_AuctionHouse` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/auctionhousedocumentation.lua` (FileDataID 4637023)

## Functions

### CalculateCommodityDeposit

```lua
C_AuctionHouse.CalculateCommodityDeposit(itemID: number, duration: luaIndex, quantity: number) -> depositCost: number?
```

`SecretArguments=AllowedWhenUntainted`

### CalculateItemDeposit

```lua
C_AuctionHouse.CalculateItemDeposit(item: ItemLocation, duration: luaIndex, quantity: number) -> depositCost: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `duration` | `luaIndex` |  |
| `quantity` | `number` |  |

### CanCancelAuction

```lua
C_AuctionHouse.CanCancelAuction(ownedAuctionID: number) -> canCancelAuction: bool
```

`SecretArguments=AllowedWhenUntainted`

### CancelAuction

```lua
C_AuctionHouse.CancelAuction(ownedAuctionID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CancelCommoditiesPurchase

```lua
C_AuctionHouse.CancelCommoditiesPurchase()
```

### CancelSell

```lua
C_AuctionHouse.CancelSell()
```

### CloseAuctionHouse

```lua
C_AuctionHouse.CloseAuctionHouse()
```

### ConfirmCommoditiesPurchase

```lua
C_AuctionHouse.ConfirmCommoditiesPurchase(itemID: number, quantity: number)
```

`SecretArguments=AllowedWhenUntainted`

### ConfirmPostCommodity

```lua
C_AuctionHouse.ConfirmPostCommodity(item: ItemLocation, duration: luaIndex, quantity: number, unitPrice: BigUInteger)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `duration` | `luaIndex` |  |
| `quantity` | `number` |  |
| `unitPrice` | `BigUInteger` |  |

### ConfirmPostItem

```lua
C_AuctionHouse.ConfirmPostItem(item: ItemLocation, duration: luaIndex, quantity: number, bid: BigUInteger?, buyout: BigUInteger?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `duration` | `luaIndex` |  |
| `quantity` | `number` |  |
| `bid` | `BigUInteger?` |  |
| `buyout` | `BigUInteger?` |  |

### FavoritesAreAvailable

```lua
C_AuctionHouse.FavoritesAreAvailable() -> favoritesAreAvailable: bool
```

### GetAuctionInfoByID

```lua
C_AuctionHouse.GetAuctionInfoByID(auctionID: number) -> priceInfo: AuctionInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetAuctionItemSubClasses

```lua
C_AuctionHouse.GetAuctionItemSubClasses(classID: number) -> subClasses: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAvailablePostCount

```lua
C_AuctionHouse.GetAvailablePostCount(item: ItemLocation) -> listCount: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetBidInfo

```lua
C_AuctionHouse.GetBidInfo(bidIndex: luaIndex) -> bid: BidInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetBids

```lua
C_AuctionHouse.GetBids() -> bids: BidInfo[]
```

### GetBidType

```lua
C_AuctionHouse.GetBidType(bidTypeIndex: luaIndex) -> typeItemKey: ItemKey?
```

`SecretArguments=AllowedWhenUntainted`

### GetBrowseResults

```lua
C_AuctionHouse.GetBrowseResults() -> browseResults: BrowseResultInfo[]
```

### GetCancelCost

```lua
C_AuctionHouse.GetCancelCost(ownedAuctionID: number) -> cancelCost: BigUInteger
```

`SecretArguments=AllowedWhenUntainted`

### GetCommoditySearchResultInfo

```lua
C_AuctionHouse.GetCommoditySearchResultInfo(itemID: number, commoditySearchResultIndex: luaIndex) -> result: CommoditySearchResultInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetCommoditySearchResultsQuantity

```lua
C_AuctionHouse.GetCommoditySearchResultsQuantity(itemID: number) -> totalQuantity: number
```

`SecretArguments=AllowedWhenUntainted`

### GetExtraBrowseInfo

```lua
C_AuctionHouse.GetExtraBrowseInfo(itemKey: ItemKey) -> extraInfo: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetFilterGroups

```lua
C_AuctionHouse.GetFilterGroups() -> filterGroups: AuctionHouseFilterGroup[]
```

### GetItemCommodityStatus

```lua
C_AuctionHouse.GetItemCommodityStatus(item: ItemLocation) -> isCommodity: ItemCommodityStatus
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemKeyFromItem

```lua
C_AuctionHouse.GetItemKeyFromItem(item: ItemLocation) -> itemKey: ItemKey
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### GetItemKeyInfo

```lua
C_AuctionHouse.GetItemKeyInfo(itemKey: ItemKey, restrictQualityToFilter: bool) -> itemKeyInfo: ItemKeyInfo?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemKey` | `ItemKey` |  |
| `restrictQualityToFilter` | `bool` | default `false` |

### GetItemKeyRequiredLevel

```lua
C_AuctionHouse.GetItemKeyRequiredLevel(itemKey: ItemKey) -> requiredLevel: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemKeySampleLink

```lua
C_AuctionHouse.GetItemKeySampleLink(itemKey: ItemKey) -> sampleItemLink: string?
```

Returns a link for an item in this key's results with player-applied enchants, gems and reforges stripped

`SecretArguments=AllowedWhenUntainted`

### GetItemSearchResultInfo

```lua
C_AuctionHouse.GetItemSearchResultInfo(itemKey: ItemKey, itemSearchResultIndex: luaIndex) -> result: ItemSearchResultInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemSearchResultsQuantity

```lua
C_AuctionHouse.GetItemSearchResultsQuantity(itemKey: ItemKey) -> totalQuantity: number
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxBidItemBid

```lua
C_AuctionHouse.GetMaxBidItemBid() -> maxBid: BigUInteger?
```

### GetMaxBidItemBuyout

```lua
C_AuctionHouse.GetMaxBidItemBuyout() -> maxBuyout: BigUInteger?
```

### GetMaxCommoditySearchResultPrice

```lua
C_AuctionHouse.GetMaxCommoditySearchResultPrice(itemID: number) -> maxUnitPrice: BigUInteger?
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxItemSearchResultBid

```lua
C_AuctionHouse.GetMaxItemSearchResultBid(itemKey: ItemKey) -> maxBid: BigUInteger?
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxItemSearchResultBuyout

```lua
C_AuctionHouse.GetMaxItemSearchResultBuyout(itemKey: ItemKey) -> maxBuyout: BigUInteger?
```

`SecretArguments=AllowedWhenUntainted`

### GetMaxOwnedAuctionBid

```lua
C_AuctionHouse.GetMaxOwnedAuctionBid() -> maxBid: BigUInteger?
```

### GetMaxOwnedAuctionBuyout

```lua
C_AuctionHouse.GetMaxOwnedAuctionBuyout() -> maxBuyout: BigUInteger?
```

### GetNumBids

```lua
C_AuctionHouse.GetNumBids() -> numBids: number
```

### GetNumBidTypes

```lua
C_AuctionHouse.GetNumBidTypes() -> numBidTypes: number
```

### GetNumCommoditySearchResults

```lua
C_AuctionHouse.GetNumCommoditySearchResults(itemID: number) -> numSearchResults: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNumItemSearchResults

```lua
C_AuctionHouse.GetNumItemSearchResults(itemKey: ItemKey) -> numItemSearchResults: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNumOwnedAuctions

```lua
C_AuctionHouse.GetNumOwnedAuctions() -> numOwnedAuctions: number
```

### GetNumOwnedAuctionTypes

```lua
C_AuctionHouse.GetNumOwnedAuctionTypes() -> numOwnedAuctionTypes: number
```

### GetNumReplicateItems

```lua
C_AuctionHouse.GetNumReplicateItems() -> numReplicateItems: number
```

### GetOwnedAuctionInfo

```lua
C_AuctionHouse.GetOwnedAuctionInfo(ownedAuctionIndex: luaIndex) -> ownedAuction: OwnedAuctionInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetOwnedAuctions

```lua
C_AuctionHouse.GetOwnedAuctions() -> ownedAuctions: OwnedAuctionInfo[]
```

### GetOwnedAuctionType

```lua
C_AuctionHouse.GetOwnedAuctionType(ownedAuctionTypeIndex: luaIndex) -> typeItemKey: ItemKey?
```

`SecretArguments=AllowedWhenUntainted`

### GetQuoteDurationRemaining

```lua
C_AuctionHouse.GetQuoteDurationRemaining() -> quoteDurationSeconds: number
```

### GetReplicateItemBattlePetInfo

```lua
C_AuctionHouse.GetReplicateItemBattlePetInfo(index: number) -> creatureID: number, displayID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetReplicateItemInfo

```lua
C_AuctionHouse.GetReplicateItemInfo(index: number) -> name: string?, texture: fileID?, count: number, qualityID: number, usable: bool?, level: number, levelType: string?, minBid: BigUInteger, minIncrement: BigUInteger, buyoutPrice: BigUInteger, bidAmount: BigUInteger, highBidder: string?, bidderFullName: string?, owner: string?, ownerFullName: string?, saleStatus: number, itemID: number, hasAllInfo: bool?
```

`SecretArguments=AllowedWhenUntainted`

### GetReplicateItemLink

```lua
C_AuctionHouse.GetReplicateItemLink(index: number) -> itemLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetReplicateItemTimeLeft

```lua
C_AuctionHouse.GetReplicateItemTimeLeft(index: number) -> timeLeft: number
```

`SecretArguments=AllowedWhenUntainted`

### GetTimeLeftBandInfo

```lua
C_AuctionHouse.GetTimeLeftBandInfo(timeLeftBand: AuctionHouseTimeLeftBand) -> timeLeftMinSeconds: number, timeLeftMaxSeconds: number
```

`SecretArguments=AllowedWhenUntainted`

### HasFavorites

```lua
C_AuctionHouse.HasFavorites() -> hasFavorites: bool
```

### HasFullBidResults

```lua
C_AuctionHouse.HasFullBidResults() -> hasFullBidResults: bool
```

### HasFullBrowseResults

```lua
C_AuctionHouse.HasFullBrowseResults() -> hasFullBrowseResults: bool
```

### HasFullCommoditySearchResults

```lua
C_AuctionHouse.HasFullCommoditySearchResults(itemID: number) -> hasFullResults: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasFullItemSearchResults

```lua
C_AuctionHouse.HasFullItemSearchResults(itemKey: ItemKey) -> hasFullResults: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasFullOwnedAuctionResults

```lua
C_AuctionHouse.HasFullOwnedAuctionResults() -> hasFullOwnedAuctionResults: bool
```

### HasMaxFavorites

```lua
C_AuctionHouse.HasMaxFavorites() -> hasMaxFavorites: bool
```

### HasSearchResults

```lua
C_AuctionHouse.HasSearchResults(itemKey: ItemKey) -> hasSearchResults: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsFavoriteItem

```lua
C_AuctionHouse.IsFavoriteItem(itemKey: ItemKey) -> isFavorite: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSellItemValid

```lua
C_AuctionHouse.IsSellItemValid(item: ItemLocation, displayError: bool) -> valid: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `displayError` | `bool` | default `true` |

### IsThrottledMessageSystemReady

```lua
C_AuctionHouse.IsThrottledMessageSystemReady() -> canSendThrottledMessage: bool
```

### MakeItemKey

```lua
C_AuctionHouse.MakeItemKey(itemID: number, itemLevel: number, itemSuffix: number, battlePetSpeciesID: number) -> itemKey: ItemKey
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `itemLevel` | `number` | default `0` |
| `itemSuffix` | `number` | default `0` |
| `battlePetSpeciesID` | `number` | default `0` |

### PlaceBid

```lua
C_AuctionHouse.PlaceBid(auctionID: number, bidAmount: BigUInteger)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### PostCommodity

```lua
C_AuctionHouse.PostCommodity(item: ItemLocation, duration: luaIndex, quantity: number, unitPrice: BigUInteger) -> needsConfirmation: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `duration` | `luaIndex` |  |
| `quantity` | `number` |  |
| `unitPrice` | `BigUInteger` |  |

### PostItem

```lua
C_AuctionHouse.PostItem(item: ItemLocation, duration: luaIndex, quantity: number, bid: BigUInteger?, buyout: BigUInteger?) -> needsConfirmation: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `item` | `ItemLocation` | `Mixin=ItemLocationMixin` |
| `duration` | `luaIndex` |  |
| `quantity` | `number` |  |
| `bid` | `BigUInteger?` |  |
| `buyout` | `BigUInteger?` |  |

### QueryBids

```lua
C_AuctionHouse.QueryBids(sorts: AuctionHouseSortType[], auctionIDs: number[])
```

`SecretArguments=AllowedWhenUntainted`

### QueryOwnedAuctions

```lua
C_AuctionHouse.QueryOwnedAuctions(sorts: AuctionHouseSortType[])
```

`SecretArguments=AllowedWhenUntainted`

### RefreshCommoditySearchResults

```lua
C_AuctionHouse.RefreshCommoditySearchResults(itemID: number)
```

`SecretArguments=AllowedWhenUntainted`

### RefreshItemSearchResults

```lua
C_AuctionHouse.RefreshItemSearchResults(itemKey: ItemKey, minLevelFilter: number?, maxLevelFilter: number?)
```

`SecretArguments=AllowedWhenUntainted`

### ReplicateItems

```lua
C_AuctionHouse.ReplicateItems()
```

This function should be used in place of an 'allItem' QueryAuctionItems call to query the entire auction house.

### RequestMoreBrowseResults

```lua
C_AuctionHouse.RequestMoreBrowseResults()
```

### RequestMoreCommoditySearchResults

```lua
C_AuctionHouse.RequestMoreCommoditySearchResults(itemID: number) -> hasFullResults: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestMoreItemSearchResults

```lua
C_AuctionHouse.RequestMoreItemSearchResults(itemKey: ItemKey) -> hasFullResults: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestOwnedAuctionBidderInfo

```lua
C_AuctionHouse.RequestOwnedAuctionBidderInfo(auctionID: number) -> bidderName: cstring
```

`SecretArguments=AllowedWhenUntainted`

### SearchForFavorites

```lua
C_AuctionHouse.SearchForFavorites(sorts: AuctionHouseSortType[])
```

`SecretArguments=AllowedWhenUntainted`

### SearchForItemKeys

```lua
C_AuctionHouse.SearchForItemKeys(itemKeys: ItemKey[], sorts: AuctionHouseSortType[])
```

`SecretArguments=AllowedWhenUntainted`

### SendBrowseQuery

```lua
C_AuctionHouse.SendBrowseQuery(query: AuctionHouseBrowseQuery)
```

`SecretArguments=AllowedWhenUntainted`

### SendSearchQuery

```lua
C_AuctionHouse.SendSearchQuery(itemKey: ItemKey, sorts: AuctionHouseSortType[], separateOwnerItems: bool, minLevelFilter: number, maxLevelFilter: number)
```

Search queries are restricted to 100 calls per minute. These should not be used to query the entire auction house. See ReplicateItems

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemKey` | `ItemKey` |  |
| `sorts` | `AuctionHouseSortType[]` |  |
| `separateOwnerItems` | `bool` |  |
| `minLevelFilter` | `number` | default `0` |
| `maxLevelFilter` | `number` | default `0` |

### SendSellSearchQuery

```lua
C_AuctionHouse.SendSellSearchQuery(itemKey: ItemKey, sorts: AuctionHouseSortType[], separateOwnerItems: bool)
```

Search queries are restricted to 100 calls per minute. These should not be used to query the entire auction house. See ReplicateItems. ItemKey should have its iLVL and suffix cleared before calling.

`SecretArguments=AllowedWhenUntainted`

### SetFavoriteItem

```lua
C_AuctionHouse.SetFavoriteItem(itemKey: ItemKey, setFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldAutoPopulatePrice

```lua
C_AuctionHouse.ShouldAutoPopulatePrice() -> shouldAutoPopulatePrice: bool
```

### StartCommoditiesPurchase

```lua
C_AuctionHouse.StartCommoditiesPurchase(itemID: number, quantity: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SupportsCopperValues

```lua
C_AuctionHouse.SupportsCopperValues() -> supportsCopperValues: bool
```

## Events

### AUCTION_CANCELED

```lua
AUCTION_CANCELED(auctionID: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_AUCTION_CREATED

```lua
AUCTION_HOUSE_AUCTION_CREATED(auctionID: number)
```

This signal is not used in the base UI but is included for AddOn ease-of-use.

`SynchronousEvent`

### AUCTION_HOUSE_AUCTIONS_EXPIRED

```lua
AUCTION_HOUSE_AUCTIONS_EXPIRED(auctionID: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_BROWSE_FAILURE

```lua
AUCTION_HOUSE_BROWSE_FAILURE()
```

`SynchronousEvent`

### AUCTION_HOUSE_BROWSE_RESULTS_ADDED

```lua
AUCTION_HOUSE_BROWSE_RESULTS_ADDED(addedBrowseResults: BrowseResultInfo[])
```

`SynchronousEvent`

### AUCTION_HOUSE_BROWSE_RESULTS_UPDATED

```lua
AUCTION_HOUSE_BROWSE_RESULTS_UPDATED()
```

`SynchronousEvent`

### AUCTION_HOUSE_CLOSED

```lua
AUCTION_HOUSE_CLOSED()
```

`SynchronousEvent`

### AUCTION_HOUSE_DISABLED

```lua
AUCTION_HOUSE_DISABLED()
```

`SynchronousEvent`

### AUCTION_HOUSE_FAVORITES_UPDATED

```lua
AUCTION_HOUSE_FAVORITES_UPDATED()
```

`SynchronousEvent`

### AUCTION_HOUSE_ITEM_DELIVERY_DELAY_UPDATE

```lua
AUCTION_HOUSE_ITEM_DELIVERY_DELAY_UPDATE(purchasedItemDeliveryDelay: number, cancelledItemDeliveryDelay: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_NEW_BID_RECEIVED

```lua
AUCTION_HOUSE_NEW_BID_RECEIVED(auctionID: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_NEW_RESULTS_RECEIVED

```lua
AUCTION_HOUSE_NEW_RESULTS_RECEIVED(itemKey: ItemKey?)
```

This signal is not used in the base UI but is included for AddOn ease-of-use. Payload is nil for browse queries.

`SynchronousEvent`

### AUCTION_HOUSE_POST_ERROR

```lua
AUCTION_HOUSE_POST_ERROR()
```

`SynchronousEvent`

### AUCTION_HOUSE_POST_WARNING

```lua
AUCTION_HOUSE_POST_WARNING()
```

`SynchronousEvent`

### AUCTION_HOUSE_PURCHASE_COMPLETED

```lua
AUCTION_HOUSE_PURCHASE_COMPLETED(auctionID: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_SCRIPT_DEPRECATED

```lua
AUCTION_HOUSE_SCRIPT_DEPRECATED()
```

`SynchronousEvent`

### AUCTION_HOUSE_SHOW

```lua
AUCTION_HOUSE_SHOW()
```

`SynchronousEvent`

### AUCTION_HOUSE_SHOW_COMMODITY_WON_NOTIFICATION

```lua
AUCTION_HOUSE_SHOW_COMMODITY_WON_NOTIFICATION(commodityName: string, commodityQuantity: number)
```

`SynchronousEvent`

### AUCTION_HOUSE_SHOW_ERROR

```lua
AUCTION_HOUSE_SHOW_ERROR(error: AuctionHouseError)
```

`SynchronousEvent`

### AUCTION_HOUSE_SHOW_FORMATTED_NOTIFICATION

```lua
AUCTION_HOUSE_SHOW_FORMATTED_NOTIFICATION(notification: AuctionHouseNotification, text: string, auctionID: number?)
```

`SynchronousEvent`

### AUCTION_HOUSE_SHOW_NOTIFICATION

```lua
AUCTION_HOUSE_SHOW_NOTIFICATION(notification: AuctionHouseNotification)
```

`SynchronousEvent`

### AUCTION_HOUSE_THROTTLED_MESSAGE_DROPPED

```lua
AUCTION_HOUSE_THROTTLED_MESSAGE_DROPPED()
```

`SynchronousEvent`

### AUCTION_HOUSE_THROTTLED_MESSAGE_QUEUED

```lua
AUCTION_HOUSE_THROTTLED_MESSAGE_QUEUED()
```

`SynchronousEvent`

### AUCTION_HOUSE_THROTTLED_MESSAGE_RESPONSE_RECEIVED

```lua
AUCTION_HOUSE_THROTTLED_MESSAGE_RESPONSE_RECEIVED()
```

`SynchronousEvent`

### AUCTION_HOUSE_THROTTLED_MESSAGE_SENT

```lua
AUCTION_HOUSE_THROTTLED_MESSAGE_SENT()
```

`SynchronousEvent`

### AUCTION_HOUSE_THROTTLED_SYSTEM_READY

```lua
AUCTION_HOUSE_THROTTLED_SYSTEM_READY()
```

`SynchronousEvent`

### AUCTION_MULTISELL_FAILURE

```lua
AUCTION_MULTISELL_FAILURE()
```

`SynchronousEvent`

### AUCTION_MULTISELL_START

```lua
AUCTION_MULTISELL_START(numRepetitions: number)
```

`SynchronousEvent`

### AUCTION_MULTISELL_UPDATE

```lua
AUCTION_MULTISELL_UPDATE(createdCount: number, totalToCreate: number)
```

`SynchronousEvent`

### BID_ADDED

```lua
BID_ADDED(bidID: number)
```

`SynchronousEvent`

### BIDS_UPDATED

```lua
BIDS_UPDATED()
```

`SynchronousEvent`

### COMMODITY_PRICE_UNAVAILABLE

```lua
COMMODITY_PRICE_UNAVAILABLE()
```

`SynchronousEvent`

### COMMODITY_PRICE_UPDATED

```lua
COMMODITY_PRICE_UPDATED(updatedUnitPrice: BigUInteger, updatedTotalPrice: BigUInteger)
```

`SynchronousEvent`

### COMMODITY_PURCHASED

```lua
COMMODITY_PURCHASED(itemID: number, quantity: number)
```

`SynchronousEvent`

### COMMODITY_PURCHASE_FAILED

```lua
COMMODITY_PURCHASE_FAILED()
```

`SynchronousEvent`

### COMMODITY_PURCHASE_SUCCEEDED

```lua
COMMODITY_PURCHASE_SUCCEEDED()
```

`SynchronousEvent`

### COMMODITY_SEARCH_RESULTS_ADDED

```lua
COMMODITY_SEARCH_RESULTS_ADDED(itemID: number)
```

`SynchronousEvent`

### COMMODITY_SEARCH_RESULTS_RECEIVED

```lua
COMMODITY_SEARCH_RESULTS_RECEIVED()
```

`UniqueEvent`

### COMMODITY_SEARCH_RESULTS_UPDATED

```lua
COMMODITY_SEARCH_RESULTS_UPDATED(itemID: number)
```

`UniqueEvent`

### EXTRA_BROWSE_INFO_RECEIVED

```lua
EXTRA_BROWSE_INFO_RECEIVED(itemID: number)
```

`SynchronousEvent`

### ITEM_KEY_ITEM_INFO_RECEIVED

```lua
ITEM_KEY_ITEM_INFO_RECEIVED(itemID: number)
```

`SynchronousEvent`

### ITEM_PURCHASED

```lua
ITEM_PURCHASED(itemID: number)
```

`SynchronousEvent`

### ITEM_SEARCH_RESULTS_ADDED

```lua
ITEM_SEARCH_RESULTS_ADDED(itemKey: ItemKey)
```

`SynchronousEvent`

### ITEM_SEARCH_RESULTS_UPDATED

```lua
ITEM_SEARCH_RESULTS_UPDATED(itemKey: ItemKey, newAuctionID: number?)
```

`UniqueEvent`

### OWNED_AUCTION_BIDDER_INFO_RECEIVED

```lua
OWNED_AUCTION_BIDDER_INFO_RECEIVED(auctionID: number, bidderName: cstring)
```

`SynchronousEvent`

### OWNED_AUCTIONS_UPDATED

```lua
OWNED_AUCTIONS_UPDATED()
```

`SynchronousEvent`

### REPLICATE_ITEM_LIST_UPDATE

```lua
REPLICATE_ITEM_LIST_UPDATE()
```

`SynchronousEvent`

## Types

### AuctionHouseFilterCategory

*Enumeration* · 3 values, 0..2

Access values as `Enum.AuctionHouseFilterCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Uncategorized` | `AuctionHouseFilterCategory` | = 0 |
| `Equipment` | `AuctionHouseFilterCategory` | = 1 |
| `Rarity` | `AuctionHouseFilterCategory` | = 2 |

### AuctionStatus

*Enumeration* · 2 values, 0..1

Access values as `Enum.AuctionStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Active` | `AuctionStatus` | = 0 |
| `Sold` | `AuctionStatus` | = 1 |

### ItemCommodityStatus

*Enumeration* · 3 values, 0..2

Access values as `Enum.ItemCommodityStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unknown` | `ItemCommodityStatus` | = 0 |
| `Item` | `ItemCommodityStatus` | = 1 |
| `Commodity` | `ItemCommodityStatus` | = 2 |

### AuctionHouseBrowseQuery

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `searchString` | `string` |  |
| `sorts` | `AuctionHouseSortType[]` |  |
| `minLevel` | `number?` |  |
| `maxLevel` | `number?` |  |
| `filters` | `AuctionHouseFilter[]?` |  |
| `itemClassFilters` | `AuctionHouseItemClassFilter[]?` |  |

### AuctionHouseFilterGroup

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `category` | `AuctionHouseFilterCategory` |  |
| `filters` | `AuctionHouseFilter[]` |  |

### AuctionHouseItemClassFilter

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `classID` | `number` |  |
| `subClassID` | `number?` |  |
| `inventoryType` | `InventoryType?` |  |

### AuctionHouseSortType

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `sortOrder` | `AuctionHouseSortOrder` |  |
| `reverseSort` | `bool` |  |

### AuctionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemKey` | `ItemKey` |  |
| `itemLink` | `string?` |  |
| `minBid` | `WOWMONEY?` |  |
| `bidAmount` | `WOWMONEY?` |  |
| `buyoutAmount` | `WOWMONEY?` |  |
| `bidder` | `WOWGUID?` |  |

### BidInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `auctionID` | `number` |  |
| `itemKey` | `ItemKey` |  |
| `itemLink` | `string?` |  |
| `timeLeft` | `AuctionHouseTimeLeftBand` |  |
| `minBid` | `BigUInteger?` |  |
| `bidAmount` | `BigUInteger?` |  |
| `buyoutAmount` | `BigUInteger?` |  |
| `bidder` | `WOWGUID?` |  |

### BrowseResultInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemKey` | `ItemKey` |  |
| `appearanceLink` | `string?` |  |
| `totalQuantity` | `number` |  |
| `minPrice` | `BigUInteger` |  |
| `containsOwnerItem` | `bool` |  |

### CommoditySearchResultInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `quantity` | `number` |  |
| `unitPrice` | `BigUInteger` |  |
| `auctionID` | `number` |  |
| `owners` | `string[]` |  |
| `totalNumberOfOwners` | `number` |  |
| `timeLeftSeconds` | `number?` |  |
| `numOwnerItems` | `number` |  |
| `containsOwnerItem` | `bool` |  |
| `containsAccountItem` | `bool` |  |

### ItemKey

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `itemLevel` | `number` | default `0` |
| `itemSuffix` | `number` | default `0` |
| `battlePetSpeciesID` | `number` | default `0` |

### ItemKeyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `battlePetSpeciesID` | `number` |  |
| `itemName` | `string` |  |
| `battlePetLink` | `string?` |  |
| `appearanceLink` | `string?` |  |
| `quality` | `ItemQuality` |  |
| `iconFileID` | `number` |  |
| `isPet` | `bool` |  |
| `isCommodity` | `bool` |  |
| `isEquipment` | `bool` |  |

### ItemSearchResultInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemKey` | `ItemKey` |  |
| `owners` | `string[]` |  |
| `totalNumberOfOwners` | `number` |  |
| `timeLeft` | `AuctionHouseTimeLeftBand` |  |
| `auctionID` | `number` |  |
| `quantity` | `number` |  |
| `itemLink` | `string?` |  |
| `containsOwnerItem` | `bool` |  |
| `containsAccountItem` | `bool` |  |
| `containsSocketedItem` | `bool` |  |
| `bidder` | `WOWGUID?` |  |
| `minBid` | `BigUInteger?` |  |
| `bidAmount` | `BigUInteger?` |  |
| `buyoutAmount` | `BigUInteger?` |  |
| `timeLeftSeconds` | `number?` |  |

### OwnedAuctionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `auctionID` | `number` |  |
| `itemKey` | `ItemKey` |  |
| `itemLink` | `string?` |  |
| `status` | `AuctionStatus` |  |
| `quantity` | `number` |  |
| `timeLeftSeconds` | `number?` |  |
| `timeLeft` | `AuctionHouseTimeLeftBand?` |  |
| `bidAmount` | `BigUInteger?` |  |
| `buyoutAmount` | `BigUInteger?` |  |
| `bidder` | `string?` |  |

### ReplicateItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `texture` | `fileID?` |  |
| `count` | `number` |  |
| `qualityID` | `number` |  |
| `usable` | `bool?` |  |
| `level` | `number` |  |
| `levelType` | `string?` |  |
| `minBid` | `BigUInteger` |  |
| `minIncrement` | `BigUInteger` |  |
| `buyoutPrice` | `BigUInteger` |  |
| `bidAmount` | `BigUInteger` |  |
| `highBidder` | `string?` |  |
| `bidderFullName` | `string?` |  |
| `owner` | `string?` |  |
| `ownerFullName` | `string?` |  |
| `saleStatus` | `number` |  |
| `itemID` | `number` |  |
| `hasAllInfo` | `bool?` |  |
