# CraftingOrderUI

Namespace `C_CraftingOrders` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/craftingorderuidocumentation.lua` (FileDataID 4637077)

## Functions

### AreOrderNotesDisabled

```lua
C_CraftingOrders.AreOrderNotesDisabled() -> areNotesDisabled: bool
```

### CalculateCraftingOrderPostingFee

```lua
C_CraftingOrders.CalculateCraftingOrderPostingFee(skillLineAbilityID: number, orderType: CraftingOrderType, orderDuration: CraftingOrderDuration) -> deposit: WOWMONEY
```

`SecretArguments=AllowedWhenUntainted`

### CancelOrder

```lua
C_CraftingOrders.CancelOrder(orderID: BigUInteger)
```

`SecretArguments=AllowedWhenUntainted`

### CanOrderSkillAbility

```lua
C_CraftingOrders.CanOrderSkillAbility(skillLineAbilityID: number) -> canOrder: bool
```

`SecretArguments=AllowedWhenUntainted`

### ClaimOrder

```lua
C_CraftingOrders.ClaimOrder(orderID: BigUInteger, profession: Profession)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CloseCrafterCraftingOrders

```lua
C_CraftingOrders.CloseCrafterCraftingOrders()
```

### CloseCustomerCraftingOrders

```lua
C_CraftingOrders.CloseCustomerCraftingOrders()
```

### FulfillOrder

```lua
C_CraftingOrders.FulfillOrder(orderID: BigUInteger, crafterNote: string, profession: Profession)
```

`SecretArguments=AllowedWhenUntainted`

### GetClaimedOrder

```lua
C_CraftingOrders.GetClaimedOrder() -> order: CraftingOrderInfo?
```

### GetCrafterBuckets

```lua
C_CraftingOrders.GetCrafterBuckets() -> buckets: CraftingOrderBucketInfo[]
```

### GetCrafterOrders

```lua
C_CraftingOrders.GetCrafterOrders() -> orders: CraftingOrderInfo[]
```

### GetCraftingOrderTime

```lua
C_CraftingOrders.GetCraftingOrderTime() -> time: BigUInteger
```

### GetCustomerCategories

```lua
C_CraftingOrders.GetCustomerCategories() -> categories: CraftingOrderCustomerCategory[]
```

### GetCustomerOptions

```lua
C_CraftingOrders.GetCustomerOptions(params: CraftingOrderCustomerSearchParams) -> results: CraftingOrderCustomerSearchResults
```

`SecretArguments=AllowedWhenUntainted`

### GetCustomerOrders

```lua
C_CraftingOrders.GetCustomerOrders() -> customerOrders: CraftingOrderInfo[]
```

### GetDefaultOrdersSkillLine

```lua
C_CraftingOrders.GetDefaultOrdersSkillLine() -> skillLineID: number?
```

### GetMyOrders

```lua
C_CraftingOrders.GetMyOrders() -> myOrders: CraftingOrderInfo[]
```

### GetNumFavoriteCustomerOptions

```lua
C_CraftingOrders.GetNumFavoriteCustomerOptions() -> numFavorites: BigUInteger
```

### GetOrderClaimInfo

```lua
C_CraftingOrders.GetOrderClaimInfo(profession: Profession) -> claimInfo: CraftingOrderClaimsRemainingInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetPersonalOrdersInfo

```lua
C_CraftingOrders.GetPersonalOrdersInfo() -> infos: CraftingOrderPersonalOrdersInfo[]
```

### HasFavoriteCustomerOptions

```lua
C_CraftingOrders.HasFavoriteCustomerOptions() -> hasFavorites: bool
```

### IsCustomerOptionFavorited

```lua
C_CraftingOrders.IsCustomerOptionFavorited(recipeID: number) -> favorited: bool
```

`SecretArguments=AllowedWhenUntainted`

### ListMyOrders

```lua
C_CraftingOrders.ListMyOrders(request: CraftingOrderRequestMyOrdersInfo)
```

`SecretArguments=AllowedWhenUntainted`

### OpenCrafterCraftingOrders

```lua
C_CraftingOrders.OpenCrafterCraftingOrders()
```

### OpenCustomerCraftingOrders

```lua
C_CraftingOrders.OpenCustomerCraftingOrders()
```

### OrderCanBeRecrafted

```lua
C_CraftingOrders.OrderCanBeRecrafted(orderID: BigUInteger) -> recraftable: bool
```

`SecretArguments=AllowedWhenUntainted`

### ParseCustomerOptions

```lua
C_CraftingOrders.ParseCustomerOptions()
```

### PlaceNewOrder

```lua
C_CraftingOrders.PlaceNewOrder(orderInfo: NewCraftingOrderInfo)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RejectOrder

```lua
C_CraftingOrders.RejectOrder(orderID: BigUInteger, crafterNote: string, profession: Profession)
```

`SecretArguments=AllowedWhenUntainted`

### ReleaseOrder

```lua
C_CraftingOrders.ReleaseOrder(orderID: BigUInteger, profession: Profession)
```

`SecretArguments=AllowedWhenUntainted`

### RequestCrafterOrders

```lua
C_CraftingOrders.RequestCrafterOrders(request: CraftingOrderRequestInfo)
```

`SecretArguments=AllowedWhenUntainted`

### RequestCustomerOrders

```lua
C_CraftingOrders.RequestCustomerOrders(request: CraftingOrderRequestInfo)
```

`SecretArguments=AllowedWhenUntainted`

### SetCustomerOptionFavorited

```lua
C_CraftingOrders.SetCustomerOptionFavorited(recipeID: number, favorited: bool)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldShowCraftingOrderTab

```lua
C_CraftingOrders.ShouldShowCraftingOrderTab() -> showTab: bool
```

### SkillLineHasOrders

```lua
C_CraftingOrders.SkillLineHasOrders(skillLineID: number) -> hasOrders: bool
```

`SecretArguments=AllowedWhenUntainted`

### UpdateIgnoreList

```lua
C_CraftingOrders.UpdateIgnoreList()
```

## Events

### CRAFTING_HOUSE_DISABLED

```lua
CRAFTING_HOUSE_DISABLED()
```

`SynchronousEvent`

### CRAFTINGORDERS_CAN_REQUEST

```lua
CRAFTINGORDERS_CAN_REQUEST()
```

`SynchronousEvent`

### CRAFTINGORDERS_CLAIMED_ORDER_ADDED

```lua
CRAFTINGORDERS_CLAIMED_ORDER_ADDED()
```

`SynchronousEvent`

### CRAFTINGORDERS_CLAIMED_ORDER_REMOVED

```lua
CRAFTINGORDERS_CLAIMED_ORDER_REMOVED()
```

`SynchronousEvent`

### CRAFTINGORDERS_CLAIMED_ORDER_UPDATED

```lua
CRAFTINGORDERS_CLAIMED_ORDER_UPDATED(orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_CLAIM_ORDER_RESPONSE

```lua
CRAFTINGORDERS_CLAIM_ORDER_RESPONSE(result: CraftingOrderResult, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_CRAFT_ORDER_RESPONSE

```lua
CRAFTINGORDERS_CRAFT_ORDER_RESPONSE(result: CraftingOrderResult, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_CUSTOMER_FAVORITES_CHANGED

```lua
CRAFTINGORDERS_CUSTOMER_FAVORITES_CHANGED()
```

`SynchronousEvent`

### CRAFTINGORDERS_CUSTOMER_OPTIONS_PARSED

```lua
CRAFTINGORDERS_CUSTOMER_OPTIONS_PARSED()
```

`SynchronousEvent`

### CRAFTINGORDERS_DISPLAY_CRAFTER_FULFILLED_MSG

```lua
CRAFTINGORDERS_DISPLAY_CRAFTER_FULFILLED_MSG(orderTypeString: cstring, itemNameString: cstring, playerNameString: cstring, tipAmount: WOWMONEY, quantityCrafted: number)
```

`SynchronousEvent`

### CRAFTINGORDERS_FULFILL_ORDER_RESPONSE

```lua
CRAFTINGORDERS_FULFILL_ORDER_RESPONSE(result: CraftingOrderResult, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_HIDE_CRAFTER

```lua
CRAFTINGORDERS_HIDE_CRAFTER()
```

`SynchronousEvent`

### CRAFTINGORDERS_HIDE_CUSTOMER

```lua
CRAFTINGORDERS_HIDE_CUSTOMER()
```

`SynchronousEvent`

### CRAFTINGORDERS_ORDER_CANCEL_RESPONSE

```lua
CRAFTINGORDERS_ORDER_CANCEL_RESPONSE(result: CraftingOrderResult)
```

`SynchronousEvent`

### CRAFTINGORDERS_ORDER_PLACEMENT_RESPONSE

```lua
CRAFTINGORDERS_ORDER_PLACEMENT_RESPONSE(result: CraftingOrderResult)
```

`SynchronousEvent`

### CRAFTINGORDERS_REJECT_ORDER_RESPONSE

```lua
CRAFTINGORDERS_REJECT_ORDER_RESPONSE(result: CraftingOrderResult, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_RELEASE_ORDER_RESPONSE

```lua
CRAFTINGORDERS_RELEASE_ORDER_RESPONSE(result: CraftingOrderResult, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_SHOW_CRAFTER

```lua
CRAFTINGORDERS_SHOW_CRAFTER()
```

`SynchronousEvent`

### CRAFTINGORDERS_SHOW_CUSTOMER

```lua
CRAFTINGORDERS_SHOW_CUSTOMER()
```

`SynchronousEvent`

### CRAFTINGORDERS_UNEXPECTED_ERROR

```lua
CRAFTINGORDERS_UNEXPECTED_ERROR()
```

`SynchronousEvent`

### CRAFTINGORDERS_UPDATE_CUSTOMER_NAME

```lua
CRAFTINGORDERS_UPDATE_CUSTOMER_NAME(customerName: cstring, orderID: BigUInteger)
```

`SynchronousEvent`

### CRAFTINGORDERS_UPDATE_ORDER_COUNT

```lua
CRAFTINGORDERS_UPDATE_ORDER_COUNT(orderType: CraftingOrderType, numOrders: number)
```

`SynchronousEvent`

### CRAFTINGORDERS_UPDATE_PERSONAL_ORDER_COUNTS

```lua
CRAFTINGORDERS_UPDATE_PERSONAL_ORDER_COUNTS()
```

`SynchronousEvent`

### CRAFTINGORDERS_UPDATE_REWARDS

```lua
CRAFTINGORDERS_UPDATE_REWARDS(npcOrderRewards: CraftingOrderRewardInfo[], orderID: BigUInteger)
```

`SynchronousEvent`

## Types

### CraftingOrderRequestInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `orderType` | `CraftingOrderType` |  |
| `selectedSkillLineAbility` | `number?` |  |
| `searchFavorites` | `bool` |  |
| `initialNonPublicSearch` | `bool` |  |
| `primarySort` | `CraftingOrderSortInfo` |  |
| `secondarySort` | `CraftingOrderSortInfo` |  |
| `forCrafter` | `bool` |  |
| `offset` | `number` |  |
| `callback` | `CraftingOrderRequestCallback` |  |
| `profession` | `Profession?` |  |

### CraftingOrderRequestMyOrdersInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `primarySort` | `CraftingOrderSortInfo` |  |
| `secondarySort` | `CraftingOrderSortInfo` |  |
| `offset` | `number` |  |
| `callback` | `CraftingOrderRequestMyOrdersCallback` |  |
