# SecureTransfer

Namespace `C_SecureTransfer` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/securetransferdocumentation.lua` (FileDataID 4637197)

## Functions

### AcceptTrade

```lua
C_SecureTransfer.AcceptTrade()
```

`HasRestrictions`

### Cancel

```lua
C_SecureTransfer.Cancel()
```

`HasRestrictions`

### CompleteHousingPurchase

```lua
C_SecureTransfer.CompleteHousingPurchase()
```

`HasRestrictions`

### CompleteHousingVCPurchase

```lua
C_SecureTransfer.CompleteHousingVCPurchase()
```

`HasRestrictions`

### GetHousingPurchaseCost

```lua
C_SecureTransfer.GetHousingPurchaseCost() -> totalCost: number
```

`HasRestrictions`

### GetHousingPurchaseQuantity

```lua
C_SecureTransfer.GetHousingPurchaseQuantity() -> quantity: number
```

`HasRestrictions`

### GetHousingVCPurchaseProductID

```lua
C_SecureTransfer.GetHousingVCPurchaseProductID() -> productID: number
```

`HasRestrictions`

### GetMailReceiveInfo

```lua
C_SecureTransfer.GetMailReceiveInfo() -> mailInfo: MailReceiveInfo
```

`HasRestrictions`

### GetMailSendInfo

```lua
C_SecureTransfer.GetMailSendInfo() -> mailInfo: MailSendInfo
```

`HasRestrictions`

### GetTradePartner

```lua
C_SecureTransfer.GetTradePartner() -> name: string?
```

`HasRestrictions`

### SendMail

```lua
C_SecureTransfer.SendMail()
```

`HasRestrictions`

### ShouldShowTradeOfferWarning

```lua
C_SecureTransfer.ShouldShowTradeOfferWarning() -> shouldShow: bool
```

`HasRestrictions`

### ShouldShowTradeRMTWarning

```lua
C_SecureTransfer.ShouldShowTradeRMTWarning() -> shouldShow: bool
```

`HasRestrictions`

### TakeMailMoney

```lua
C_SecureTransfer.TakeMailMoney()
```

`HasRestrictions`

## Events

### SECURE_TRANSFER_CANCEL

```lua
SECURE_TRANSFER_CANCEL()
```

`SynchronousEvent`

### SECURE_TRANSFER_CONFIRM_HOUSING_PURCHASE

```lua
SECURE_TRANSFER_CONFIRM_HOUSING_PURCHASE()
```

`SynchronousEvent`

### SECURE_TRANSFER_CONFIRM_SEND_MAIL

```lua
SECURE_TRANSFER_CONFIRM_SEND_MAIL()
```

`SynchronousEvent`

### SECURE_TRANSFER_CONFIRM_TAKE_MAIL_MONEY

```lua
SECURE_TRANSFER_CONFIRM_TAKE_MAIL_MONEY()
```

`SynchronousEvent`

### SECURE_TRANSFER_CONFIRM_TRADE_ACCEPT

```lua
SECURE_TRANSFER_CONFIRM_TRADE_ACCEPT()
```

`SynchronousEvent`

### SECURE_TRANSFER_HOUSING_CURRENCY_PURCHASE_CONFIRMATION

```lua
SECURE_TRANSFER_HOUSING_CURRENCY_PURCHASE_CONFIRMATION()
```

`SynchronousEvent`

## Types

### MailReceiveInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `sender` | `string` |  |
| `money` | `number` |  |

### MailSendInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `target` | `string` |  |
| `sendMoney` | `number` |  |
