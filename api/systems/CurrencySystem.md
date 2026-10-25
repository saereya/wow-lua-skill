# CurrencySystem

Namespace `C_CurrencyInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/currencyinfodocumentation.lua` (FileDataID 4637087)

## Functions

### CanTransferCurrency

```lua
C_CurrencyInfo.CanTransferCurrency(currencyID: number) -> canTransferCurrency: bool, failureReason: AccountCurrencyTransferResult?
```

`SecretArguments=AllowedWhenUntainted`

### DoesCurrentFilterRequireAccountCurrencyData

```lua
C_CurrencyInfo.DoesCurrentFilterRequireAccountCurrencyData() -> doesCurrentFilterRequireAccountCurrencyData: bool
```

### DoesWarModeBonusApply

```lua
C_CurrencyInfo.DoesWarModeBonusApply(currencyID: number) -> warModeApplies: bool?, limitOncePerTooltip: bool?
```

`SecretArguments=AllowedWhenUntainted`

### ExpandCurrencyList

```lua
C_CurrencyInfo.ExpandCurrencyList(index: luaIndex, expand: bool)
```

`SecretArguments=AllowedWhenUntainted`

### FetchCurrencyDataFromAccountCharacters

```lua
C_CurrencyInfo.FetchCurrencyDataFromAccountCharacters(currencyID: number) -> accountCurrencyData: CharacterCurrencyData[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### FetchCurrencyTransferTransactions

```lua
C_CurrencyInfo.FetchCurrencyTransferTransactions() -> currencyTransferTransactions: CurrencyTransferTransaction[]
```

### GetAzeriteCurrencyID

```lua
C_CurrencyInfo.GetAzeriteCurrencyID() -> azeriteCurrencyID: number
```

### GetBackpackCurrencyInfo

```lua
C_CurrencyInfo.GetBackpackCurrencyInfo(index: luaIndex) -> info: BackpackCurrencyInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetBasicCurrencyInfo

```lua
C_CurrencyInfo.GetBasicCurrencyInfo(currencyType: number, quantity: number?) -> info: CurrencyDisplayInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCoinIcon

```lua
C_CurrencyInfo.GetCoinIcon(amount: WOWMONEY) -> result: fileID
```

`SecretArguments=AllowedWhenUntainted`

### GetCoinText

```lua
C_CurrencyInfo.GetCoinText(amount: WOWMONEY, separator: cstring) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `amount` | `WOWMONEY` |  |
| `separator` | `cstring` | default `", "` |

### GetCoinTextureString

```lua
C_CurrencyInfo.GetCoinTextureString(amount: WOWMONEY, fontHeight: number) -> result: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `amount` | `WOWMONEY` |  |
| `fontHeight` | `number` | default `14` |

### GetCostToTransferCurrency

```lua
C_CurrencyInfo.GetCostToTransferCurrency(currencyID: number, quantity: number) -> totalQuantityConsumed: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyContainerInfo

```lua
C_CurrencyInfo.GetCurrencyContainerInfo(currencyType: number, quantity: number) -> info: CurrencyDisplayInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyDescription

```lua
C_CurrencyInfo.GetCurrencyDescription(type: number) -> description: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyFilter

```lua
C_CurrencyInfo.GetCurrencyFilter() -> filterType: CurrencyFilterType
```

### GetCurrencyIDFromLink

```lua
C_CurrencyInfo.GetCurrencyIDFromLink(currencyLink: cstring) -> currencyID: number
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyInfo

```lua
C_CurrencyInfo.GetCurrencyInfo(type: number) -> info: CurrencyInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyInfoFromLink

```lua
C_CurrencyInfo.GetCurrencyInfoFromLink(link: string) -> info: CurrencyInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyLink

```lua
C_CurrencyInfo.GetCurrencyLink(type: number, amount: number?) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyListInfo

```lua
C_CurrencyInfo.GetCurrencyListInfo(index: luaIndex) -> info: CurrencyInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetCurrencyListLink

```lua
C_CurrencyInfo.GetCurrencyListLink(index: luaIndex) -> link: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrencyListSize

```lua
C_CurrencyInfo.GetCurrencyListSize() -> currencyListSize: number
```

### GetDragonIslesSuppliesCurrencyID

```lua
C_CurrencyInfo.GetDragonIslesSuppliesCurrencyID() -> dragonIslesSuppliesCurrencyID: number
```

### GetFactionGrantedByCurrency

```lua
C_CurrencyInfo.GetFactionGrantedByCurrency(currencyID: number) -> factionID: number?
```

Gets the faction ID for currency that is immediately converted into reputation with that faction instead.

`SecretArguments=AllowedWhenUntainted`

### GetMaxTransferableAmountFromQuantity

```lua
C_CurrencyInfo.GetMaxTransferableAmountFromQuantity(currencyID: number, requestedQuantity: number) -> maxTransferableAmount: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerCurrencyCategoryInfo

```lua
C_CurrencyInfo.GetPlayerCurrencyCategoryInfo(categoryID: number, includeAccountWide: bool) -> info: PlayerCurrencyCategoryInfo
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `categoryID` | `number` |  |
| `includeAccountWide` | `bool` | default `true` |

### GetWarResourcesCurrencyID

```lua
C_CurrencyInfo.GetWarResourcesCurrencyID() -> warResourceCurrencyID: number
```

### IsAccountCharacterCurrencyDataReady

```lua
C_CurrencyInfo.IsAccountCharacterCurrencyDataReady() -> isReady: bool
```

### IsAccountTransferableCurrency

```lua
C_CurrencyInfo.IsAccountTransferableCurrency(currencyID: number) -> isAccountTransferableCurrency: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsAccountWideCurrency

```lua
C_CurrencyInfo.IsAccountWideCurrency(currencyID: number) -> isAccountWideCurrency: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCurrencyContainer

```lua
C_CurrencyInfo.IsCurrencyContainer(currencyID: number, quantity: number) -> isCurrencyContainer: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsCurrencyTransferInProgress

```lua
C_CurrencyInfo.IsCurrencyTransferInProgress() -> currencyTransferInProgress: bool
```

### IsCurrencyTransferTransactionDataReady

```lua
C_CurrencyInfo.IsCurrencyTransferTransactionDataReady() -> isReady: bool
```

### PickupCurrency

```lua
C_CurrencyInfo.PickupCurrency(type: number)
```

`SecretArguments=AllowedWhenUntainted`

### PlayerHasMaxQuantity

```lua
C_CurrencyInfo.PlayerHasMaxQuantity(currencyID: number) -> hasMaxQuantity: bool
```

`SecretArguments=AllowedWhenUntainted`

### PlayerHasMaxWeeklyQuantity

```lua
C_CurrencyInfo.PlayerHasMaxWeeklyQuantity(currencyID: number) -> hasMaxWeeklyQuantity: bool
```

`SecretArguments=AllowedWhenUntainted`

### RequestCurrencyDataForAccountCharacters

```lua
C_CurrencyInfo.RequestCurrencyDataForAccountCharacters()
```

### RequestCurrencyFromAccountCharacter

```lua
C_CurrencyInfo.RequestCurrencyFromAccountCharacter(sourceCharacterGUID: WOWGUID, currencyID: number, quantity: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetCurrencyBackpack

```lua
C_CurrencyInfo.SetCurrencyBackpack(index: luaIndex, backpack: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCurrencyBackpackByID

```lua
C_CurrencyInfo.SetCurrencyBackpackByID(currencyType: number, backpack: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetCurrencyFilter

```lua
C_CurrencyInfo.SetCurrencyFilter(filterType: CurrencyFilterType)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetCurrencyUnused

```lua
C_CurrencyInfo.SetCurrencyUnused(index: luaIndex, unused: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACCOUNT_CHARACTER_CURRENCY_DATA_RECEIVED

```lua
ACCOUNT_CHARACTER_CURRENCY_DATA_RECEIVED()
```

`SynchronousEvent`

### ACCOUNT_MONEY

```lua
ACCOUNT_MONEY()
```

`SynchronousEvent`

### CURRENCY_DISPLAY_UPDATE

```lua
CURRENCY_DISPLAY_UPDATE(currencyType: number?, quantity: number?, quantityChange: number?, quantityGainSource: number?, destroyReason: number?)
```

`SynchronousEvent`

### CURRENCY_TRANSFER_FAILED

```lua
CURRENCY_TRANSFER_FAILED(failureReason: AccountCurrencyTransferResult)
```

`SynchronousEvent`

### CURRENCY_TRANSFER_INITIATED

```lua
CURRENCY_TRANSFER_INITIATED()
```

`SynchronousEvent`

### CURRENCY_TRANSFER_LOG_UPDATE

```lua
CURRENCY_TRANSFER_LOG_UPDATE()
```

`SynchronousEvent`

### CURRENCY_TRANSFER_SUCCESS

```lua
CURRENCY_TRANSFER_SUCCESS()
```

`SynchronousEvent`

### PLAYER_MONEY

```lua
PLAYER_MONEY()
```

`SynchronousEvent`

## Types

### BackpackCurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `quantity` | `number` |  |
| `iconFileID` | `fileID` |  |
| `currencyTypesID` | `number` |  |

### CharacterCurrencyData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `characterGUID` | `WOWGUID` |  |
| `characterName` | `string` |  |
| `fullCharacterName` | `string` |  |
| `currencyID` | `number` |  |
| `quantity` | `number` |  |

### CurrencyDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `description` | `string` |  |
| `icon` | `number` |  |
| `quality` | `number` |  |
| `displayAmount` | `number` |  |
| `actualAmount` | `number` |  |

### CurrencyInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `currencyID` | `number` |  |
| `isHeader` | `bool` |  |
| `isHeaderExpanded` | `bool` |  |
| `currencyListDepth` | `number` |  |
| `isTypeUnused` | `bool` |  |
| `isShowInBackpack` | `bool` |  |
| `quantity` | `number` |  |
| `trackedQuantity` | `number` |  |
| `iconFileID` | `fileID` |  |
| `maxQuantity` | `number` |  |
| `canEarnPerWeek` | `bool` |  |
| `quantityEarnedThisWeek` | `number` |  |
| `isTradeable` | `bool` |  |
| `quality` | `ItemQuality` |  |
| `maxWeeklyQuantity` | `number` |  |
| `totalEarned` | `number` |  |
| `discovered` | `bool` |  |
| `useTotalEarnedForMaxQty` | `bool` |  |
| `isAccountWide` | `bool` |  |
| `isAccountTransferable` | `bool` |  |
| `transferPercentage` | `number?` |  |
| `rechargingCycleDurationMS` | `number` |  |
| `rechargingAmountPerCycle` | `number` |  |

### CurrencyTransferTransaction

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `sourceCharacterGUID` | `WOWGUID` |  |
| `sourceCharacterName` | `string` | default `""` |
| `fullSourceCharacterName` | `string` | default `""` |
| `destinationCharacterGUID` | `WOWGUID` |  |
| `destinationCharacterName` | `string` | default `""` |
| `fullDestinationCharacterName` | `string` | default `""` |
| `currencyType` | `number` |  |
| `quantityTransferred` | `number` |  |
| `totalQuantityConsumed` | `number` |  |
| `timestamp` | `time_t` |  |

### PlayerCurrencyCategoryInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `categoryName` | `cstring` |  |
| `currencyTypes` | `number[]` |  |
| `childCategories` | `number[]` |  |
