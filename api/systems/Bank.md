# Bank

Namespace `C_Bank` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/bankdocumentation.lua` (FileDataID 4637026)

## Functions

### AreAnyBankTypesViewable

```lua
C_Bank.AreAnyBankTypesViewable() -> areAnyBankTypesViewable: bool
```

### AutoDepositItemsIntoBank

```lua
C_Bank.AutoDepositItemsIntoBank(bankType: BankType)
```

`SecretArguments=AllowedWhenUntainted`

### BankBagTypeAndIDToInvSlot

```lua
C_Bank.BankBagTypeAndIDToInvSlot(bankType: BankType, slotIndex: luaIndex) -> slot: number?
```

`SecretArguments=AllowedWhenUntainted`

### CanDepositMoney

```lua
C_Bank.CanDepositMoney(bankType: BankType) -> canDepositMoney: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanPurchaseBankTab

```lua
C_Bank.CanPurchaseBankTab(bankType: BankType) -> canPurchaseBankTab: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanUseBank

```lua
C_Bank.CanUseBank(bankType: BankType) -> canUseBank: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanViewBank

```lua
C_Bank.CanViewBank(bankType: BankType) -> canViewBank: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanWithdrawMoney

```lua
C_Bank.CanWithdrawMoney(bankType: BankType) -> canWithdrawMoney: bool
```

`SecretArguments=AllowedWhenUntainted`

### CloseBankFrame

```lua
C_Bank.CloseBankFrame()
```

### DepositMoney

```lua
C_Bank.DepositMoney(bankType: BankType, amount: WOWMONEY)
```

`SecretArguments=AllowedWhenUntainted`

### DoesBankTypeSupportAutoDeposit

```lua
C_Bank.DoesBankTypeSupportAutoDeposit(bankType: BankType) -> doesBankTypeSupportAutoDeposit: bool
```

`SecretArguments=AllowedWhenUntainted`

### DoesBankTypeSupportMoneyTransfer

```lua
C_Bank.DoesBankTypeSupportMoneyTransfer(bankType: BankType) -> doesBankTypeSupportMoneyTransfer: bool
```

`SecretArguments=AllowedWhenUntainted`

### FetchBankLockedReason

```lua
C_Bank.FetchBankLockedReason(bankType: BankType) -> reason: BankLockedReason?
```

`SecretArguments=AllowedWhenUntainted`

### FetchDepositedMoney

```lua
C_Bank.FetchDepositedMoney(bankType: BankType) -> amount: WOWMONEY
```

`SecretArguments=AllowedWhenUntainted`

### FetchMaxNumBankTabs

```lua
C_Bank.FetchMaxNumBankTabs(bankType: BankType) -> numPurchasedBankTabs: number
```

`SecretArguments=AllowedWhenUntainted`

### FetchNextPurchasableBankTabData

```lua
C_Bank.FetchNextPurchasableBankTabData(bankType: BankType) -> nextPurchasableTabData: PurchasableBankTabData?
```

`SecretArguments=AllowedWhenUntainted`

### FetchNumPurchasedBankTabs

```lua
C_Bank.FetchNumPurchasedBankTabs(bankType: BankType) -> numPurchasedBankTabs: number
```

`SecretArguments=AllowedWhenUntainted`

### FetchPurchasedBankTabData

```lua
C_Bank.FetchPurchasedBankTabData(bankType: BankType) -> purchasedBankTabData: BankTabData[]
```

`SecretArguments=AllowedWhenUntainted`

### FetchPurchasedBankTabIDs

```lua
C_Bank.FetchPurchasedBankTabIDs(bankType: BankType) -> purchasedBankTabIDs: BagIndex[]
```

`SecretArguments=AllowedWhenUntainted`

### FetchViewableBankTypes

```lua
C_Bank.FetchViewableBankTypes() -> viewableBankTypes: BankType[]
```

### HasMaxBankTabs

```lua
C_Bank.HasMaxBankTabs(bankType: BankType) -> hasMaxBankTabs: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsItemAllowedInBankType

```lua
C_Bank.IsItemAllowedInBankType(bankType: BankType, itemLocation: ItemLocation) -> isItemAllowedInBankType: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `bankType` | `BankType` |  |
| `itemLocation` | `ItemLocation` | `Mixin=ItemLocationMixin` |

### PurchaseBankTab

```lua
C_Bank.PurchaseBankTab(bankType: BankType)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ShouldUsePlayerBagsInBank

```lua
C_Bank.ShouldUsePlayerBagsInBank() -> shouldUsePlayerBagsInBank: bool
```

### UpdateBankTabSettings

```lua
C_Bank.UpdateBankTabSettings(bankType: BankType, tabID: BagIndex, tabName: cstring, tabIcon: cstring, depositFlags: BagSlotFlags)
```

`SecretArguments=AllowedWhenUntainted`

### WithdrawMoney

```lua
C_Bank.WithdrawMoney(bankType: BankType, amount: WOWMONEY)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### BANK_BAG_SLOT_FLAGS_UPDATED

```lua
BANK_BAG_SLOT_FLAGS_UPDATED(slot: number)
```

`SynchronousEvent`

### BANKFRAME_CLOSED

```lua
BANKFRAME_CLOSED()
```

`SynchronousEvent`

### BANKFRAME_OPENED

```lua
BANKFRAME_OPENED()
```

`SynchronousEvent`

### BANK_TABS_CHANGED

```lua
BANK_TABS_CHANGED(bankType: BankType)
```

`SynchronousEvent`

### BANK_TAB_SETTINGS_UPDATED

```lua
BANK_TAB_SETTINGS_UPDATED(bankType: BankType)
```

`SynchronousEvent`

### PLAYER_ACCOUNT_BANK_TAB_SLOTS_CHANGED

```lua
PLAYER_ACCOUNT_BANK_TAB_SLOTS_CHANGED(slot: number)
```

`SynchronousEvent`

### PLAYERBANKSLOTS_CHANGED

```lua
PLAYERBANKSLOTS_CHANGED(slot: number)
```

`SynchronousEvent`

## Types

### BankLockedReason

*Enumeration* · 4 values, 0..3

Access values as `Enum.BankLockedReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `BankLockedReason` | = 0 |
| `NoAccountInventoryLock` | `BankLockedReason` | = 1 |
| `BankDisabled` | `BankLockedReason` | = 2 |
| `BankConversionFailed` | `BankLockedReason` | = 3 |

### BankTabData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `bankType` | `BankType` |  |
| `name` | `cstring` |  |
| `icon` | `fileID` |  |
| `depositFlags` | `BagSlotFlags` |  |
| `tabCleanupConfirmation` | `cstring` |  |
| `tabNameEditBoxHeader` | `cstring` |  |

### PurchasableBankTabData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tabCost` | `BigUInteger` |  |
| `canAfford` | `bool` |  |
| `purchasePromptTitle` | `cstring` |  |
| `purchasePromptBody` | `cstring` |  |
| `purchasePromptConfirmation` | `cstring` |  |
