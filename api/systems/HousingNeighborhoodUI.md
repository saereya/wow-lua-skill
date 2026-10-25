# HousingNeighborhoodUI

Namespace `C_HousingNeighborhood` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingneighborhooduidocumentation.lua` (FileDataID 6152783)

## Functions

### CancelInviteToNeighborhood

```lua
C_HousingNeighborhood.CancelInviteToNeighborhood(playerName: cstring)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### CanReturnAfterVisitingHouse

```lua
C_HousingNeighborhood.CanReturnAfterVisitingHouse() -> canReturn: bool
```

### DemoteToResident

```lua
C_HousingNeighborhood.DemoteToResident(playerGUID: WOWGUID)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### GetCornerstoneHouseInfo

```lua
C_HousingNeighborhood.GetCornerstoneHouseInfo() -> houseInfo: HouseInfo
```

Only available when interacting with a cornerstone game object

### GetCornerstoneNeighborhoodInfo

```lua
C_HousingNeighborhood.GetCornerstoneNeighborhoodInfo() -> neighborhoodInfo: NeighborhoodInfo
```

Only available when interacting with a cornerstone game object

### GetCornerstonePurchaseMode

```lua
C_HousingNeighborhood.GetCornerstonePurchaseMode() -> purchaseMode: CornerstonePurchaseMode
```

Only available when interacting with a cornerstone game object

### GetCurrentNeighborhoodTextureSuffix

```lua
C_HousingNeighborhood.GetCurrentNeighborhoodTextureSuffix() -> neighborhoodTextureSuffix: cstring
```

### GetDiscountedMovePrice

```lua
C_HousingNeighborhood.GetDiscountedMovePrice() -> movePrice: number
```

Only available when interacting with a cornerstone game object

Returns:

| Name | Type | Notes |
|---|---|---|
| `movePrice` | `number` | Can be negative if the refund from moving is more than the cost of the new house |

### GetMoveCooldownTime

```lua
C_HousingNeighborhood.GetMoveCooldownTime() -> movecooldownTime: number
```

Only available when interacting with a cornerstone game object

### GetNeighborhoodMapData

```lua
C_HousingNeighborhood.GetNeighborhoodMapData() -> neighborhoodPlots: NeighborhoodPlotMapInfo[]
```

### GetNeighborhoodName

```lua
C_HousingNeighborhood.GetNeighborhoodName() -> neighborhoodName: string
```

### GetNeighborhoodPlotName

```lua
C_HousingNeighborhood.GetNeighborhoodPlotName(plotIndex: number) -> neighborhoodName: string
```

`SecretArguments=AllowedWhenUntainted`

### GetPreviousHouseIdentifier

```lua
C_HousingNeighborhood.GetPreviousHouseIdentifier() -> previousHouseIdentifier: string
```

Only available when interacting with a cornerstone game object

### HasPermissionToPurchase

```lua
C_HousingNeighborhood.HasPermissionToPurchase() -> cantPurchaseReason: PurchaseHouseDisabledReason
```

Only available when interacting with a cornerstone game object

### InvitePlayerToNeighborhood

```lua
C_HousingNeighborhood.InvitePlayerToNeighborhood(playerName: cstring)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### IsNeighborhoodManager

```lua
C_HousingNeighborhood.IsNeighborhoodManager() -> isManager: bool
```

### IsNeighborhoodOwner

```lua
C_HousingNeighborhood.IsNeighborhoodOwner() -> isOwner: bool
```

### IsPlayerInOtherPlayersPlot

```lua
C_HousingNeighborhood.IsPlayerInOtherPlayersPlot() -> isInUnownedPlot: bool
```

This returns true if the player is in a plot that is owned by another player

### IsPlotAvailableForPurchase

```lua
C_HousingNeighborhood.IsPlotAvailableForPurchase() -> isAvailable: bool
```

Only available when interacting with a cornerstone game object

### IsPlotOwnedByPlayer

```lua
C_HousingNeighborhood.IsPlotOwnedByPlayer() -> isPlayerOwned: bool
```

Only available when interacting with a cornerstone game object

### OnBulletinBoardClosed

```lua
C_HousingNeighborhood.OnBulletinBoardClosed()
```

### OnCornerstoneClosed

```lua
C_HousingNeighborhood.OnCornerstoneClosed()
```

### PromoteToManager

```lua
C_HousingNeighborhood.PromoteToManager(playerGUID: WOWGUID)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### RequestNeighborhoodInfo

```lua
C_HousingNeighborhood.RequestNeighborhoodInfo()
```

### RequestNeighborhoodRoster

```lua
C_HousingNeighborhood.RequestNeighborhoodRoster()
```

Only available when interacting with a bulletin board game object

### RequestPendingNeighborhoodInvites

```lua
C_HousingNeighborhood.RequestPendingNeighborhoodInvites()
```

Only available when interacting with a bulletin board game object

### TransferNeighborhoodOwnership

```lua
C_HousingNeighborhood.TransferNeighborhoodOwnership(playerGUID: WOWGUID)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### TryEvictPlayer

```lua
C_HousingNeighborhood.TryEvictPlayer(plotID: number)
```

Only available when interacting with a bulletin board game object

`SecretArguments=AllowedWhenUntainted`

### TryMoveHouse

```lua
C_HousingNeighborhood.TryMoveHouse()
```

Only available when interacting with a cornerstone game object

### TryPurchasePlot

```lua
C_HousingNeighborhood.TryPurchasePlot()
```

Only available when interacting with a cornerstone game object

## Events

### CANCEL_NEIGHBORHOOD_INVITE_RESPONSE

```lua
CANCEL_NEIGHBORHOOD_INVITE_RESPONSE(result: NeighborhoodInviteResult, playerName: cstring?)
```

`SynchronousEvent`

### CLOSE_PLOT_CORNERSTONE

```lua
CLOSE_PLOT_CORNERSTONE()
```

`SynchronousEvent`

### NEIGHBORHOOD_INFO_UPDATED

```lua
NEIGHBORHOOD_INFO_UPDATED(neighborhoodInfo: NeighborhoodInfo)
```

`SynchronousEvent`

### NEIGHBORHOOD_INVITE_RESPONSE

```lua
NEIGHBORHOOD_INVITE_RESPONSE(result: NeighborhoodInviteResult)
```

`SynchronousEvent`

### NEIGHBORHOOD_MAP_DATA_UPDATED

```lua
NEIGHBORHOOD_MAP_DATA_UPDATED()
```

`UniqueEvent`

### NEIGHBORHOOD_NAME_UPDATED

```lua
NEIGHBORHOOD_NAME_UPDATED(neighborhoodGuid: WOWGUID, neighborhoodName: cstring)
```

`UniqueEvent`

### OPEN_PLOT_CORNERSTONE

```lua
OPEN_PLOT_CORNERSTONE()
```

`SynchronousEvent`

### PENDING_NEIGHBORHOOD_INVITES_RECIEVED

```lua
PENDING_NEIGHBORHOOD_INVITES_RECIEVED(result: NeighborhoodInviteResult, pendingInviteList: string[]?)
```

`SynchronousEvent`

### PURCHASE_PLOT_RESULT

```lua
PURCHASE_PLOT_RESULT(result: number)
```

`SynchronousEvent`

### SHOW_PLAYER_EVICTED_DIALOG

```lua
SHOW_PLAYER_EVICTED_DIALOG()
```

`SynchronousEvent`

### UPDATE_BULLETIN_BOARD_MEMBER_TYPE

```lua
UPDATE_BULLETIN_BOARD_MEMBER_TYPE(player: WOWGUID, residentType: ResidentType)
```

`SynchronousEvent`

### UPDATE_BULLETIN_BOARD_ROSTER

```lua
UPDATE_BULLETIN_BOARD_ROSTER(neighborhoodInfo: NeighborhoodInfo, rosterMemberList: NeighborhoodRosterMemberInfo[])
```

`SynchronousEvent`

### UPDATE_BULLETIN_BOARD_ROSTER_STATUSES

```lua
UPDATE_BULLETIN_BOARD_ROSTER_STATUSES(rosterMemberList: NeighborhoodRosterMemberUpdateInfo[])
```

`SynchronousEvent`

## Types

### CornerstonePurchaseMode

*Enumeration* · 3 values, 0..2

Access values as `Enum.CornerstonePurchaseMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Basic` | `CornerstonePurchaseMode` | = 0 |
| `Import` | `CornerstonePurchaseMode` | = 1 |
| `Move` | `CornerstonePurchaseMode` | = 2 |
