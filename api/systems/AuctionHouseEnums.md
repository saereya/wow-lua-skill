# AuctionHouseEnums

source `interface/addons/blizzard_apidocumentationgenerated/auctionhouseenumsdocumentation.lua` (FileDataID 4637020)

## Types

### AuctionHouseCommoditySortOrder

*Enumeration* · 2 values, 0..1

Access values as `Enum.AuctionHouseCommoditySortOrder.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UnitPrice` | `AuctionHouseCommoditySortOrder` | = 0 |
| `Quantity` | `AuctionHouseCommoditySortOrder` | = 1 |

### AuctionHouseError

*Enumeration* · 27 values, 0..26

Access values as `Enum.AuctionHouseError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NotEnoughMoney` | `AuctionHouseError` | = 0 |
| `HigherBid` | `AuctionHouseError` | = 1 |
| `BidIncrement` | `AuctionHouseError` | = 2 |
| `BidOwn` | `AuctionHouseError` | = 3 |
| `ItemNotFound` | `AuctionHouseError` | = 4 |
| `RestrictedAccountTrial` | `AuctionHouseError` | = 5 |
| `HasRestriction` | `AuctionHouseError` | = 6 |
| `IsBusy` | `AuctionHouseError` | = 7 |
| `Unavailable` | `AuctionHouseError` | = 8 |
| `ItemHasQuote` | `AuctionHouseError` | = 9 |
| `DatabaseError` | `AuctionHouseError` | = 10 |
| `MinBid` | `AuctionHouseError` | = 11 |
| `NotEnoughItems` | `AuctionHouseError` | = 12 |
| `RepairItem` | `AuctionHouseError` | = 13 |
| `UsedCharges` | `AuctionHouseError` | = 14 |
| `QuestItem` | `AuctionHouseError` | = 15 |
| `BoundItem` | `AuctionHouseError` | = 16 |
| `ConjuredItem` | `AuctionHouseError` | = 17 |
| `LimitedDurationItem` | `AuctionHouseError` | = 18 |
| `IsBag` | `AuctionHouseError` | = 19 |
| `EquippedBag` | `AuctionHouseError` | = 20 |
| `WrappedItem` | `AuctionHouseError` | = 21 |
| `LootItem` | `AuctionHouseError` | = 22 |
| `DoubleBid` | `AuctionHouseError` | = 23 |
| `FavoritesMaxed` | `AuctionHouseError` | = 24 |
| `ItemNotAvailable` | `AuctionHouseError` | = 25 |
| `ItemBoundToAccountUntilEquip` | `AuctionHouseError` | = 26 |

### AuctionHouseExtraColumn

*Enumeration* · 5 values, 0..4

Access values as `Enum.AuctionHouseExtraColumn.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `AuctionHouseExtraColumn` | = 0 |
| `Ilvl` | `AuctionHouseExtraColumn` | = 1 |
| `Slots` | `AuctionHouseExtraColumn` | = 2 |
| `Level` | `AuctionHouseExtraColumn` | = 3 |
| `Skill` | `AuctionHouseExtraColumn` | = 4 |

### AuctionHouseFilter

*Enumeration* · 14 values, 0..13

Access values as `Enum.AuctionHouseFilter.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `AuctionHouseFilter` | = 0 |
| `UncollectedOnly` | `AuctionHouseFilter` | = 1 |
| `UsableOnly` | `AuctionHouseFilter` | = 2 |
| `CurrentExpansionOnly` | `AuctionHouseFilter` | = 3 |
| `UpgradesOnly` | `AuctionHouseFilter` | = 4 |
| `ExactMatch` | `AuctionHouseFilter` | = 5 |
| `PoorQuality` | `AuctionHouseFilter` | = 6 |
| `CommonQuality` | `AuctionHouseFilter` | = 7 |
| `UncommonQuality` | `AuctionHouseFilter` | = 8 |
| `RareQuality` | `AuctionHouseFilter` | = 9 |
| `EpicQuality` | `AuctionHouseFilter` | = 10 |
| `LegendaryQuality` | `AuctionHouseFilter` | = 11 |
| `ArtifactQuality` | `AuctionHouseFilter` | = 12 |
| `LegendaryCraftedItemOnly` | `AuctionHouseFilter` | = 13 |

### AuctionHouseItemSortOrder

*Enumeration* · 2 values, 0..1

Access values as `Enum.AuctionHouseItemSortOrder.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Bid` | `AuctionHouseItemSortOrder` | = 0 |
| `Buyout` | `AuctionHouseItemSortOrder` | = 1 |

### AuctionHouseNotification

*Enumeration* · 6 values, 0..5

Access values as `Enum.AuctionHouseNotification.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `BidPlaced` | `AuctionHouseNotification` | = 0 |
| `AuctionRemoved` | `AuctionHouseNotification` | = 1 |
| `AuctionWon` | `AuctionHouseNotification` | = 2 |
| `AuctionOutbid` | `AuctionHouseNotification` | = 3 |
| `AuctionSold` | `AuctionHouseNotification` | = 4 |
| `AuctionExpired` | `AuctionHouseNotification` | = 5 |

### AuctionHouseSortOrder

*Enumeration* · 6 values, 0..5

Access values as `Enum.AuctionHouseSortOrder.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Price` | `AuctionHouseSortOrder` | = 0 |
| `Name` | `AuctionHouseSortOrder` | = 1 |
| `Level` | `AuctionHouseSortOrder` | = 2 |
| `Bid` | `AuctionHouseSortOrder` | = 3 |
| `Buyout` | `AuctionHouseSortOrder` | = 4 |
| `TimeRemaining` | `AuctionHouseSortOrder` | = 5 |

### AuctionHouseTimeLeftBand

*Enumeration* · 4 values, 0..3

Access values as `Enum.AuctionHouseTimeLeftBand.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Short` | `AuctionHouseTimeLeftBand` | = 0 |
| `Medium` | `AuctionHouseTimeLeftBand` | = 1 |
| `Long` | `AuctionHouseTimeLeftBand` | = 2 |
| `VeryLong` | `AuctionHouseTimeLeftBand` | = 3 |
