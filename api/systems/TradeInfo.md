# TradeInfo

Namespace `C_TradeInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/tradeinfodocumentation.lua` (FileDataID 4637266)

## Functions

### AddTradeMoney

```lua
C_TradeInfo.AddTradeMoney()
```

Adds any cursor-held money to the current trade offer.

`HasRestrictions`

### PickupTradeMoney

```lua
C_TradeInfo.PickupTradeMoney(amount: WOWMONEY)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetTradeMoney

```lua
C_TradeInfo.SetTradeMoney(amount: WOWMONEY)
```

Sets the amount of money in the current trade offer.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ShouldShowTradeOfferWarning

```lua
C_TradeInfo.ShouldShowTradeOfferWarning() -> shouldShow: bool
```

## Events

### PLAYER_TRADE_CURRENCY

```lua
PLAYER_TRADE_CURRENCY()
```

`SynchronousEvent`

### PLAYER_TRADE_MONEY

```lua
PLAYER_TRADE_MONEY()
```

`SynchronousEvent`

### TRADE_ACCEPT_UPDATE

```lua
TRADE_ACCEPT_UPDATE(playerAccepted: number, targetAccepted: number)
```

`SynchronousEvent`

### TRADE_CLOSED

```lua
TRADE_CLOSED()
```

`SynchronousEvent`

### TRADE_CURRENCY_CHANGED

```lua
TRADE_CURRENCY_CHANGED()
```

`SynchronousEvent`

### TRADE_MONEY_CHANGED

```lua
TRADE_MONEY_CHANGED()
```

`SynchronousEvent`

### TRADE_PLAYER_ITEM_CHANGED

```lua
TRADE_PLAYER_ITEM_CHANGED(tradeSlotIndex: number)
```

`SynchronousEvent`

### TRADE_POTENTIAL_BIND_ENCHANT

```lua
TRADE_POTENTIAL_BIND_ENCHANT(canBecomeBoundForTrade: bool)
```

`SynchronousEvent`

### TRADE_POTENTIAL_REMOVE_TRANSMOG

```lua
TRADE_POTENTIAL_REMOVE_TRANSMOG(itemLink: cstring, tradeSlotIndex: number)
```

`SynchronousEvent`

### TRADE_REQUEST

```lua
TRADE_REQUEST(name: cstring)
```

`SynchronousEvent`

### TRADE_REQUEST_CANCEL

```lua
TRADE_REQUEST_CANCEL()
```

`SynchronousEvent`

### TRADE_SHOW

```lua
TRADE_SHOW()
```

`SynchronousEvent`

### TRADE_TARGET_ITEM_CHANGED

```lua
TRADE_TARGET_ITEM_CHANGED(tradeSlotIndex: number)
```

`SynchronousEvent`

### TRADE_UPDATE

```lua
TRADE_UPDATE()
```

`SynchronousEvent`

### TRADE_UPDATE_WARNINGS

```lua
TRADE_UPDATE_WARNINGS()
```

`SynchronousEvent`
