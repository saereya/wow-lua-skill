# MerchantFrame

Namespace `C_MerchantFrame` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/merchantframedocumentation.lua` (FileDataID 4637139)

## Functions

### GetBuybackItemID

```lua
C_MerchantFrame.GetBuybackItemID(buybackSlotIndex: luaIndex) -> buybackItemID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetItemInfo

```lua
C_MerchantFrame.GetItemInfo(index: luaIndex) -> info: MerchantItemInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMerchantCurrencies

```lua
C_MerchantFrame.GetMerchantCurrencies() -> currencies: number[]
```

`MayReturnNothing`

### GetNumJunkItems

```lua
C_MerchantFrame.GetNumJunkItems() -> numJunkItems: number
```

### IsMerchantItemRefundable

```lua
C_MerchantFrame.IsMerchantItemRefundable(index: luaIndex) -> refundable: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSellAllJunkEnabled

```lua
C_MerchantFrame.IsSellAllJunkEnabled() -> enabled: bool
```

### SellAllJunkItems

```lua
C_MerchantFrame.SellAllJunkItems()
```

## Events

### MERCHANT_CLOSED

```lua
MERCHANT_CLOSED()
```

`SynchronousEvent`

### MERCHANT_FILTER_ITEM_UPDATE

```lua
MERCHANT_FILTER_ITEM_UPDATE(itemID: number)
```

`SynchronousEvent`

### MERCHANT_SHOW

```lua
MERCHANT_SHOW()
```

`SynchronousEvent`

### MERCHANT_UPDATE

```lua
MERCHANT_UPDATE()
```

`SynchronousEvent`

## Types

### MerchantItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `texture` | `fileID` |  |
| `price` | `number` | default `0` |
| `stackCount` | `number` | default `0` |
| `numAvailable` | `number` | default `0` |
| `isPurchasable` | `bool` | default `false` |
| `isUsable` | `bool` | default `false` |
| `hasExtendedCost` | `bool` | default `false` |
| `currencyID` | `number?` |  |
| `spellID` | `number?` |  |
| `isQuestStartItem` | `bool` | default `false` |
