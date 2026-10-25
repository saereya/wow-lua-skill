# AccountStore

Namespace `C_AccountStore` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/accountstoredocumentation.lua` (FileDataID 6177617)

## Functions

### BeginPurchase

```lua
C_AccountStore.BeginPurchase(itemID: number) -> purchaseStarted: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetCategories

```lua
C_AccountStore.GetCategories(storeFrontID: number) -> categories: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetCategoryInfo

```lua
C_AccountStore.GetCategoryInfo(categoryID: number) -> info: AccountStoreCategoryInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetCategoryItems

```lua
C_AccountStore.GetCategoryItems(categoryID: number) -> itemIDs: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyAvailable

```lua
C_AccountStore.GetCurrencyAvailable(currencyID: number) -> amount: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyIDForStore

```lua
C_AccountStore.GetCurrencyIDForStore(storeFrontID: number) -> currencyID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyInfo

```lua
C_AccountStore.GetCurrencyInfo(currencyID: number) -> info: AccountStoreCurrencyInfo
```

`SecretArguments=AllowedWhenUntainted`

### GetItemInfo

```lua
C_AccountStore.GetItemInfo(itemID: number) -> info: AccountStoreItemInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetStoreFrontState

```lua
C_AccountStore.GetStoreFrontState(storeFrontID: number) -> state: AccountStoreState
```

`SecretArguments=AllowedWhenUntainted`

### RefundItem

```lua
C_AccountStore.RefundItem(itemID: number) -> refundStarted: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestStoreFrontInfoUpdate

```lua
C_AccountStore.RequestStoreFrontInfoUpdate(storeFrontID: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACCOUNT_STORE_CURRENCY_AVAILABLE_UPDATED

```lua
ACCOUNT_STORE_CURRENCY_AVAILABLE_UPDATED(currencyID: number)
```

`SynchronousEvent`

### ACCOUNT_STORE_FRONT_UPDATED

```lua
ACCOUNT_STORE_FRONT_UPDATED(storeFrontID: number)
```

`SynchronousEvent`

### ACCOUNT_STORE_ITEM_INFO_UPDATED

```lua
ACCOUNT_STORE_ITEM_INFO_UPDATED(itemID: number)
```

`SynchronousEvent`

### ACCOUNT_STORE_TRANSACTION_ERROR

```lua
ACCOUNT_STORE_TRANSACTION_ERROR(result: AccountStoreTransactionResult)
```

`SynchronousEvent`

### STORE_FRONT_STATE_UPDATED

```lua
STORE_FRONT_STATE_UPDATED(storeFrontID: number)
```

`SynchronousEvent`

## Types

### AccountStoreCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `name` | `cstring` |  |
| `type` | `AccountStoreCategoryType` |  |
| `icon` | `fileID` |  |

### AccountStoreCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `amount` | `number` |  |
| `maxQuantity` | `number?` |  |
| `name` | `cstring` |  |
| `icon` | `fileID` |  |

### AccountStoreItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `number` |  |
| `status` | `AccountStoreItemStatus` |  |
| `mode` | `AccountStoreItemMode` |  |
| `currencyID` | `number` |  |
| `flags` | `AccountStoreItemFlag` |  |
| `customUIModelSceneID` | `number?` |  |
| `name` | `cstring` |  |
| `description` | `cstring?` |  |
| `price` | `number` |  |
| `nonrefundable` | `bool` |  |
| `creatureDisplayID` | `number?` |  |
| `transmogSetID` | `number?` |  |
| `displayIcon` | `fileID?` |  |
| `refundSecondsRemaining` | `time_t?` |  |
