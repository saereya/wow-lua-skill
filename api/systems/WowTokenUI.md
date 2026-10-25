# WowTokenUI

Namespace `C_WowTokenUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/wowtokenuidocumentation.lua` (FileDataID 4637305)

## Functions

### ShouldDisplayInAuctionHouse

```lua
C_WowTokenUI.ShouldDisplayInAuctionHouse() -> displayInAH: bool
```

### StartTokenSell

```lua
C_WowTokenUI.StartTokenSell(tokenGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### TOKEN_AUCTION_SOLD

```lua
TOKEN_AUCTION_SOLD()
```

`SynchronousEvent`

### TOKEN_BUY_CONFIRM_REQUIRED

```lua
TOKEN_BUY_CONFIRM_REQUIRED()
```

`SynchronousEvent`

### TOKEN_BUY_RESULT

```lua
TOKEN_BUY_RESULT(result: number)
```

`SynchronousEvent`

### TOKEN_CAN_VETERAN_BUY_UPDATE

```lua
TOKEN_CAN_VETERAN_BUY_UPDATE(result: number)
```

`SynchronousEvent`

### TOKEN_DISTRIBUTIONS_UPDATED

```lua
TOKEN_DISTRIBUTIONS_UPDATED(result: number)
```

`SynchronousEvent`

### TOKEN_MARKET_PRICE_UPDATED

```lua
TOKEN_MARKET_PRICE_UPDATED(result: number)
```

`SynchronousEvent`

### TOKEN_REDEEM_BALANCE_UPDATED

```lua
TOKEN_REDEEM_BALANCE_UPDATED()
```

`SynchronousEvent`

### TOKEN_REDEEM_CONFIRM_REQUIRED

```lua
TOKEN_REDEEM_CONFIRM_REQUIRED(choiceType: luaIndex)
```

`SynchronousEvent`

### TOKEN_REDEEM_FRAME_SHOW

```lua
TOKEN_REDEEM_FRAME_SHOW()
```

`SynchronousEvent`

### TOKEN_REDEEM_GAME_TIME_UPDATED

```lua
TOKEN_REDEEM_GAME_TIME_UPDATED()
```

`SynchronousEvent`

### TOKEN_REDEEM_RESULT

```lua
TOKEN_REDEEM_RESULT(result: luaIndex, choiceType: luaIndex)
```

`SynchronousEvent`

### TOKEN_SELL_CONFIRMED

```lua
TOKEN_SELL_CONFIRMED()
```

`SynchronousEvent`

### TOKEN_SELL_CONFIRM_REQUIRED

```lua
TOKEN_SELL_CONFIRM_REQUIRED()
```

`SynchronousEvent`

### TOKEN_SELL_RESULT

```lua
TOKEN_SELL_RESULT(result: number)
```

`SynchronousEvent`

### TOKEN_STATUS_CHANGED

```lua
TOKEN_STATUS_CHANGED()
```

`SynchronousEvent`
