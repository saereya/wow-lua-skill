# HousingUI

Namespace `C_Housing` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housinguidocumentation.lua` (FileDataID 5222393)

## Functions

### AcceptNeighborhoodOwnership

```lua
C_Housing.AcceptNeighborhoodOwnership()
```

### CanEditCharter

```lua
C_Housing.CanEditCharter() -> canEditCharter: bool
```

### CanTakeReportScreenshot

```lua
C_Housing.CanTakeReportScreenshot(plotIndex: number) -> reason: InvalidPlotScreenshotReason
```

`SecretArguments=AllowedWhenUntainted`

### CreateGuildNeighborhood

```lua
C_Housing.CreateGuildNeighborhood(neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### CreateNeighborhoodCharter

```lua
C_Housing.CreateNeighborhoodCharter(neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### DeclineNeighborhoodOwnership

```lua
C_Housing.DeclineNeighborhoodOwnership()
```

### DoesFactionMatchNeighborhood

```lua
C_Housing.DoesFactionMatchNeighborhood(neighborhoodGUID: WOWGUID) -> factionMatches: bool
```

`SecretArguments=AllowedWhenUntainted`

### EditNeighborhoodCharter

```lua
C_Housing.EditNeighborhoodCharter(neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentHouseInfo

```lua
C_Housing.GetCurrentHouseInfo() -> houseInfo: HouseInfo?
```

### GetCurrentHouseLevelFavor

```lua
C_Housing.GetCurrentHouseLevelFavor(houseGuid: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentHouseRefundAmount

```lua
C_Housing.GetCurrentHouseRefundAmount() -> refundAmount: number
```

### GetCurrentNeighborhoodGUID

```lua
C_Housing.GetCurrentNeighborhoodGUID() -> neighborhoodGUID: WOWGUID?
```

### GetHouseLevelFavorForLevel

```lua
C_Housing.GetHouseLevelFavorForLevel(level: number) -> houseFavor: number
```

`SecretArguments=AllowedWhenUntainted`

### GetHouseLevelRewardsForLevel

```lua
C_Housing.GetHouseLevelRewardsForLevel(level: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetHousingAccessFlags

```lua
C_Housing.GetHousingAccessFlags() -> accessFlags: HouseSettingFlags
```

### GetMaxHouseLevel

```lua
C_Housing.GetMaxHouseLevel() -> level: number
```

### GetNeighborhoodTextureSuffix

```lua
C_Housing.GetNeighborhoodTextureSuffix(neighborhoodGUID: WOWGUID) -> neighborhoodTextureSuffix: cstring
```

`SecretArguments=AllowedWhenUntainted`

### GetOthersOwnedHouses

```lua
C_Housing.GetOthersOwnedHouses(playerGUID: WOWGUID?, bnetID: number?, isInPlayersGuild: bool)
```

`SecretArguments=AllowedWhenUntainted`

### GetPlayerOwnedHouses

```lua
C_Housing.GetPlayerOwnedHouses()
```

### GetTrackedHouseGuid

```lua
C_Housing.GetTrackedHouseGuid() -> trackedHouse: WOWGUID?
```

### GetUIMapIDForNeighborhood

```lua
C_Housing.GetUIMapIDForNeighborhood(neighborhoodGuid: WOWGUID) -> uiMapID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetVisitCooldownInfo

```lua
C_Housing.GetVisitCooldownInfo() -> spellCooldownInfo: SpellCooldownInfo
```

`MayReturnNothing`

### HasHousingExpansionAccess

```lua
C_Housing.HasHousingExpansionAccess() -> hasAccess: bool
```

### HouseFinderDeclineNeighborhoodInvitation

```lua
C_Housing.HouseFinderDeclineNeighborhoodInvitation()
```

### HouseFinderIgnoreNeighborhood

```lua
C_Housing.HouseFinderIgnoreNeighborhood(neighborhoodGuid: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### HouseFinderRequestNeighborhoods

```lua
C_Housing.HouseFinderRequestNeighborhoods()
```

### HouseFinderRequestReservationAndPort

```lua
C_Housing.HouseFinderRequestReservationAndPort(neighborhoodGuid: WOWGUID, plotID: number)
```

`SecretArguments=AllowedWhenUntainted`

### IsHousingMarketCartFullRemoveEnabled

```lua
C_Housing.IsHousingMarketCartFullRemoveEnabled() -> isHousingMarketCartFullRemoveEnabled: bool
```

### IsHousingMarketEnabled

```lua
C_Housing.IsHousingMarketEnabled() -> isHousingMarketEnabled: bool
```

### IsHousingMarketShopEnabled

```lua
C_Housing.IsHousingMarketShopEnabled() -> isHousingMarketShopEnabled: bool
```

### IsHousingServiceEnabled

```lua
C_Housing.IsHousingServiceEnabled() -> isAvailable: bool
```

### IsInsideHouse

```lua
C_Housing.IsInsideHouse() -> isInside: bool
```

### IsInsideHouseOrPlot

```lua
C_Housing.IsInsideHouseOrPlot() -> isInside: bool
```

### IsInsideOwnedHouse

```lua
C_Housing.IsInsideOwnedHouse() -> isInsideOwnedHouse: bool
```

### IsInsideOwnedHouseOrPlot

```lua
C_Housing.IsInsideOwnedHouseOrPlot() -> isInsideOwnedHouseOrPlot: bool
```

### IsInsideOwnedPlot

```lua
C_Housing.IsInsideOwnedPlot() -> isInside: bool
```

### IsInsidePlot

```lua
C_Housing.IsInsidePlot() -> isInside: bool
```

### IsOnNeighborhoodMap

```lua
C_Housing.IsOnNeighborhoodMap() -> isOnNeighborhoodMap: bool
```

### LeaveHouse

```lua
C_Housing.LeaveHouse()
```

### OnCharterConfirmationAccepted

```lua
C_Housing.OnCharterConfirmationAccepted()
```

### OnCharterConfirmationClosed

```lua
C_Housing.OnCharterConfirmationClosed()
```

### OnCreateCharterNeighborhoodClosed

```lua
C_Housing.OnCreateCharterNeighborhoodClosed()
```

### OnCreateGuildNeighborhoodClosed

```lua
C_Housing.OnCreateGuildNeighborhoodClosed()
```

### OnHouseFinderClickPlot

```lua
C_Housing.OnHouseFinderClickPlot(plotID: number)
```

`SecretArguments=AllowedWhenUntainted`

### OnRequestSignatureClicked

```lua
C_Housing.OnRequestSignatureClicked()
```

### OnSignCharterClicked

```lua
C_Housing.OnSignCharterClicked(charterOwnerGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### RelinquishHouse

```lua
C_Housing.RelinquishHouse(houseGuid: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### RequestCurrentHouseInfo

```lua
C_Housing.RequestCurrentHouseInfo()
```

### RequestHouseFinderNeighborhoodData

```lua
C_Housing.RequestHouseFinderNeighborhoodData(neighborhoodGuid: WOWGUID, neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### RequestPlayerCharacterList

```lua
C_Housing.RequestPlayerCharacterList()
```

### ResetHouse

```lua
C_Housing.ResetHouse(resetScope: HousingHouseScope)
```

Resets all contents of the house, based on the provided scope; API restricted to ensure this can't be triggered without the player getting ample notice and confirmation

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ReturnAfterVisitingHouse

```lua
C_Housing.ReturnAfterVisitingHouse()
```

`HasRestrictions`

### SaveHouseSettings

```lua
C_Housing.SaveHouseSettings(playerGUID: WOWGUID, accessFlags: HouseSettingFlags)
```

`SecretArguments=AllowedWhenUntainted`

### SearchBNetFriendNeighborhoods

```lua
C_Housing.SearchBNetFriendNeighborhoods(bnetName: cstring) -> isValidBnetFriend: bool
```

`SecretArguments=AllowedWhenUntainted`

### SearchBNetFriendNeighborhoodsByID

```lua
C_Housing.SearchBNetFriendNeighborhoodsByID(bnetID: number) -> isValidBnetFriend: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetTrackedHouseGuid

```lua
C_Housing.SetTrackedHouseGuid(trackedHouse: WOWGUID?)
```

`SecretArguments=AllowedWhenUntainted`

### StartTutorial

```lua
C_Housing.StartTutorial()
```

### TeleportHome

```lua
C_Housing.TeleportHome(neighborhoodGUID: WOWGUID, houseGUID: WOWGUID, plotID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### TryRenameNeighborhood

```lua
C_Housing.TryRenameNeighborhood(neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### ValidateCreateGuildNeighborhoodSize

```lua
C_Housing.ValidateCreateGuildNeighborhoodSize()
```

### ValidateNeighborhoodName

```lua
C_Housing.ValidateNeighborhoodName(neighborhoodName: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### VisitHouse

```lua
C_Housing.VisitHouse(neighborhoodGUID: WOWGUID, houseGUID: WOWGUID, plotID: number)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### ADD_NEIGHBORHOOD_CHARTER_SIGNATURE

```lua
ADD_NEIGHBORHOOD_CHARTER_SIGNATURE(signature: cstring)
```

`SynchronousEvent`

### B_NET_NEIGHBORHOOD_LIST_UPDATED

```lua
B_NET_NEIGHBORHOOD_LIST_UPDATED(result: HousingResult, neighborhoodInfos: NeighborhoodInfo[]?)
```

`SynchronousEvent`

### CLOSE_CHARTER_CONFIRMATION_UI

```lua
CLOSE_CHARTER_CONFIRMATION_UI()
```

`SynchronousEvent`

### CLOSE_CREATE_CHARTER_NEIGHBORHOOD_UI

```lua
CLOSE_CREATE_CHARTER_NEIGHBORHOOD_UI()
```

`SynchronousEvent`

### CLOSE_CREATE_GUILD_NEIGHBORHOOD_UI

```lua
CLOSE_CREATE_GUILD_NEIGHBORHOOD_UI()
```

`SynchronousEvent`

### CREATE_NEIGHBORHOOD_RESULT

```lua
CREATE_NEIGHBORHOOD_RESULT(result: HousingResult, neighborhoodName: cstring?)
```

`SynchronousEvent`

### CURRENT_HOUSE_INFO_RECIEVED

```lua
CURRENT_HOUSE_INFO_RECIEVED(houseInfo: HouseInfo)
```

`SynchronousEvent`

### CURRENT_HOUSE_INFO_UPDATED

```lua
CURRENT_HOUSE_INFO_UPDATED(houseInfo: HouseInfo)
```

`SynchronousEvent`

### DECLINE_NEIGHBORHOOD_INVITATION_RESPONSE

```lua
DECLINE_NEIGHBORHOOD_INVITATION_RESPONSE(success: bool)
```

`SynchronousEvent`

### FORCE_REFRESH_HOUSE_FINDER

```lua
FORCE_REFRESH_HOUSE_FINDER()
```

`SynchronousEvent`

### HOUSE_FINDER_NEIGHBORHOOD_DATA_RECIEVED

```lua
HOUSE_FINDER_NEIGHBORHOOD_DATA_RECIEVED(neighborhoodPlots: NeighborhoodPlotMapInfo[])
```

`SynchronousEvent`

### HOUSE_INFO_UPDATED

```lua
HOUSE_INFO_UPDATED()
```

`SynchronousEvent`

### HOUSE_LEVEL_CHANGED

```lua
HOUSE_LEVEL_CHANGED(newHouseLevelInfo: HouseLevelInfo?)
```

`SynchronousEvent`

### HOUSE_LEVEL_FAVOR_UPDATED

```lua
HOUSE_LEVEL_FAVOR_UPDATED(houseLevelFavor: HouseLevelFavor)
```

`SynchronousEvent`

### HOUSE_PLOT_ENTERED

```lua
HOUSE_PLOT_ENTERED()
```

`SynchronousEvent`

### HOUSE_PLOT_EXITED

```lua
HOUSE_PLOT_EXITED()
```

`SynchronousEvent`

### HOUSE_RESERVATION_RESPONSE_RECIEVED

```lua
HOUSE_RESERVATION_RESPONSE_RECIEVED(result: HousingResult)
```

`SynchronousEvent`

### HOUSE_RESET_COMPLETED

```lua
HOUSE_RESET_COMPLETED()
```

`SynchronousEvent`

### HOUSE_RESET_FAILED

```lua
HOUSE_RESET_FAILED(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_MARKET_AVAILABILITY_UPDATED

```lua
HOUSING_MARKET_AVAILABILITY_UPDATED()
```

`SynchronousEvent`

### HOUSING_SERVICES_AVAILABILITY_UPDATED

```lua
HOUSING_SERVICES_AVAILABILITY_UPDATED()
```

`SynchronousEvent`

### IGNORE_NEIGHBORHOOD_RESPONSE

```lua
IGNORE_NEIGHBORHOOD_RESPONSE(success: bool, neighborhoodGuid: WOWGUID)
```

`SynchronousEvent`

### MOVE_OUT_RESERVATION_UPDATED

```lua
MOVE_OUT_RESERVATION_UPDATED()
```

`SynchronousEvent`

### NEIGHBORHOOD_GUILD_SIZE_VALIDATED

```lua
NEIGHBORHOOD_GUILD_SIZE_VALIDATED(approved: bool)
```

`SynchronousEvent`

### NEIGHBORHOOD_LIST_UPDATED

```lua
NEIGHBORHOOD_LIST_UPDATED(result: HousingResult, neighborhoodInfos: NeighborhoodInfo[]?)
```

`SynchronousEvent`

### NEIGHBORHOOD_NAME_VALIDATED

```lua
NEIGHBORHOOD_NAME_VALIDATED(approved: bool)
```

`SynchronousEvent`

### NEW_HOUSING_ITEM_ACQUIRED

```lua
NEW_HOUSING_ITEM_ACQUIRED(itemType: HousingItemToastType, itemName: cstring, icon: fileID?)
```

`SynchronousEvent`

### OPEN_CHARTER_CONFIRMATION_UI

```lua
OPEN_CHARTER_CONFIRMATION_UI(neighborhoodName: string, locationName: string)
```

`SynchronousEvent`

### OPEN_CREATE_CHARTER_NEIGHBORHOOD_UI

```lua
OPEN_CREATE_CHARTER_NEIGHBORHOOD_UI(locationName: cstring)
```

`SynchronousEvent`

### OPEN_CREATE_GUILD_NEIGHBORHOOD_UI

```lua
OPEN_CREATE_GUILD_NEIGHBORHOOD_UI(locationName: cstring)
```

`SynchronousEvent`

### OPEN_NEIGHBORHOOD_CHARTER

```lua
OPEN_NEIGHBORHOOD_CHARTER(neighborhoodInfo: NeighborhoodInfo, signatures: string[], requiredSignatures: number)
```

`SynchronousEvent`

### OPEN_NEIGHBORHOOD_CHARTER_SIGNATURE_REQUEST

```lua
OPEN_NEIGHBORHOOD_CHARTER_SIGNATURE_REQUEST(neighborhoodInfo: NeighborhoodInfo)
```

`SynchronousEvent`

### PLAYER_CHARACTER_LIST_UPDATED

```lua
PLAYER_CHARACTER_LIST_UPDATED(characterInfos: HouseOwnerCharacterInfo[], ownerListIndex: number)
```

`SynchronousEvent`

### PLAYER_HOUSE_LIST_UPDATED

```lua
PLAYER_HOUSE_LIST_UPDATED(houseInfos: HouseInfo[])
```

`SynchronousEvent`

### RECEIVED_HOUSE_LEVEL_REWARDS

```lua
RECEIVED_HOUSE_LEVEL_REWARDS(level: number, rewards: HouseLevelReward[])
```

`SynchronousEvent`

### REMOVE_NEIGHBORHOOD_CHARTER_SIGNATURE

```lua
REMOVE_NEIGHBORHOOD_CHARTER_SIGNATURE(signature: cstring)
```

`SynchronousEvent`

### SHOW_NEIGHBORHOOD_OWNERSHIP_TRANSFER_DIALOG

```lua
SHOW_NEIGHBORHOOD_OWNERSHIP_TRANSFER_DIALOG(neighborhoodName: cstring, cosmeticOwnerName: cstring)
```

`SynchronousEvent`

### TRACKED_HOUSE_CHANGED

```lua
TRACKED_HOUSE_CHANGED(trackedHouse: WOWGUID?)
```

`SynchronousEvent`

### VIEW_HOUSES_LIST_RECIEVED

```lua
VIEW_HOUSES_LIST_RECIEVED(houseInfos: HouseInfo[])
```

`SynchronousEvent`

## Types

### CreateNeighborhoodErrorType

*Enumeration* · 4 values, 0..3

Access values as `Enum.CreateNeighborhoodErrorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CreateNeighborhoodErrorType` | = 0 |
| `Profanity` | `CreateNeighborhoodErrorType` | = 1 |
| `UndersizedGuild` | `CreateNeighborhoodErrorType` | = 2 |
| `OversizedGuild` | `CreateNeighborhoodErrorType` | = 3 |

### HousingItemToastType

*Enumeration* · 5 values, 0..4

Access values as `Enum.HousingItemToastType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Room` | `HousingItemToastType` | = 0 |
| `Fixture` | `HousingItemToastType` | = 1 |
| `Customization` | `HousingItemToastType` | = 2 |
| `Decor` | `HousingItemToastType` | = 3 |
| `HouseType` | `HousingItemToastType` | = 4 |
