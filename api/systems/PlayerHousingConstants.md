# PlayerHousingConstants

source `interface/addons/blizzard_apidocumentationgenerated/playerhousingconstantsdocumentation.lua` (FileDataID 5221196)

## Types

### HouseEditingContext

*Enumeration* · 4 values, 0..3

Access values as `Enum.HouseEditingContext.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseEditingContext` | = 0 |
| `Decor` | `HouseEditingContext` | = 1 |
| `Room` | `HouseEditingContext` | = 2 |
| `Fixture` | `HouseEditingContext` | = 3 |

### HouseEditorMode

*Enumeration* · 7 values, 0..6

Access values as `Enum.HouseEditorMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseEditorMode` | = 0 |
| `BasicDecor` | `HouseEditorMode` | = 1 |
| `ExpertDecor` | `HouseEditorMode` | = 2 |
| `Layout` | `HouseEditorMode` | = 3 |
| `Customize` | `HouseEditorMode` | = 4 |
| `Cleanup` | `HouseEditorMode` | = 5 |
| `ExteriorCustomization` | `HouseEditorMode` | = 6 |

### HouseExteriorWMODataFlags

*Enumeration* · 5 values, 0..8

Access values as `Enum.HouseExteriorWMODataFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseExteriorWMODataFlags` | = 0 |
| `UnlockedByDefault` | `HouseExteriorWMODataFlags` | = 1 |
| `AllowedInHordeNeighborhoods` | `HouseExteriorWMODataFlags` | = 2 |
| `AllowedInAllianceNeighborhoods` | `HouseExteriorWMODataFlags` | = 4 |
| `HiddenUnlessOwned` | `HouseExteriorWMODataFlags` | = 8 |

### HouseFinderSuggestionReason

*Enumeration* · 9 values, 0..128

Access values as `Enum.HouseFinderSuggestionReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseFinderSuggestionReason` | = 0 |
| `Owner` | `HouseFinderSuggestionReason` | = 1 |
| `CharterInvite` | `HouseFinderSuggestionReason` | = 2 |
| `Guild` | `HouseFinderSuggestionReason` | = 4 |
| `BNetFriends` | `HouseFinderSuggestionReason` | = 8 |
| `PartySync` | `HouseFinderSuggestionReason` | = 16 |
| `Random` | `HouseFinderSuggestionReason` | = 32 |
| `HomeOwner` | `HouseFinderSuggestionReason` | = 64 |
| `Relinquished` | `HouseFinderSuggestionReason` | = 128 |

### HouseOwnerError

*Enumeration* · 4 values, 0..3

Access values as `Enum.HouseOwnerError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HouseOwnerError` | = 0 |
| `Faction` | `HouseOwnerError` | = 1 |
| `Guild` | `HouseOwnerError` | = 2 |
| `GenericPermission` | `HouseOwnerError` | = 3 |

### HousingBlueprintFlag

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingBlueprintFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingBlueprintFlag` | = 0 |
| `AutomaticBackup` | `HousingBlueprintFlag` | = 1 |

### HousingBlueprintType

*Enumeration* · 5 values, 0..4

Access values as `Enum.HousingBlueprintType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingBlueprintType` | = 0 |
| `House` | `HousingBlueprintType` | = 1 |
| `Room` | `HousingBlueprintType` | = 2 |
| `Interior` | `HousingBlueprintType` | = 3 |
| `Exterior` | `HousingBlueprintType` | = 4 |

### HousingBudgetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingBudgetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RoomPlacement` | `HousingBudgetType` | = 0 |
| `DecorPlacement` | `HousingBudgetType` | = 1 |
| `PetDecor` | `HousingBudgetType` | = 2 |

### HousingDecorTheme

*Enumeration* · 6 values, 0..5

Access values as `Enum.HousingDecorTheme.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingDecorTheme` | = 0 |
| `Folk` | `HousingDecorTheme` | = 1 |
| `Rugged` | `HousingDecorTheme` | = 2 |
| `Generic` | `HousingDecorTheme` | = 3 |
| `NightElf` | `HousingDecorTheme` | = 4 |
| `BloodElf` | `HousingDecorTheme` | = 5 |

### HousingFixtureDecorAction

*Enumeration* · 2 values, 0..1

Kinds of actions that can be taken to deal with decor attached to an Exterior Fixture that is being removed or swapped

Access values as `Enum.HousingFixtureDecorAction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Store` | `HousingFixtureDecorAction` | = 0; Return any currently-attached decor back into storage |
| `Detach` | `HousingFixtureDecorAction` | = 1; Detach any currently-attached decor, and leave it floating in its current position; It will NOT be re-attached to the new Exterior Fixtures |

### HousingFixtureFlags

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingFixtureFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingFixtureFlags` | = 0 |
| `IsDefaultFixture` | `HousingFixtureFlags` | = 1 |
| `UnlockedByDefault` | `HousingFixtureFlags` | = 2 |

### HousingFixtureSize

*Enumeration* · 5 values, 0..4

Access values as `Enum.HousingFixtureSize.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingFixtureSize` | = 0 |
| `Any` | `HousingFixtureSize` | = 1 |
| `Small` | `HousingFixtureSize` | = 2 |
| `Medium` | `HousingFixtureSize` | = 3 |
| `Large` | `HousingFixtureSize` | = 4 |

### HousingFixtureType

*Enumeration* · 9 values, 0..16

Access values as `Enum.HousingFixtureType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingFixtureType` | = 0 |
| `Base` | `HousingFixtureType` | = 9 |
| `Roof` | `HousingFixtureType` | = 10 |
| `Door` | `HousingFixtureType` | = 11 |
| `Window` | `HousingFixtureType` | = 12 |
| `RoofDetail` | `HousingFixtureType` | = 13 |
| `RoofWindow` | `HousingFixtureType` | = 14 |
| `Tower` | `HousingFixtureType` | = 15 |
| `Chimney` | `HousingFixtureType` | = 16 |

### HousingHouseScope

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingHouseScope.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingHouseScope` | = 0 |
| `Interior` | `HousingHouseScope` | = 1 |
| `Exterior` | `HousingHouseScope` | = 2 |

### HousingLayoutRestriction

*Enumeration* · 10 values, 0..9

Access values as `Enum.HousingLayoutRestriction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingLayoutRestriction` | = 0 |
| `RoomNotFound` | `HousingLayoutRestriction` | = 1 |
| `NotInsideHouse` | `HousingLayoutRestriction` | = 2 |
| `NotHouseOwner` | `HousingLayoutRestriction` | = 3 |
| `IsBaseRoom` | `HousingLayoutRestriction` | = 4 |
| `RoomNotLeaf` | `HousingLayoutRestriction` | = 5 |
| `StairwellConnection` | `HousingLayoutRestriction` | = 6 |
| `LastRoom` | `HousingLayoutRestriction` | = 7 |
| `UnreachableRoom` | `HousingLayoutRestriction` | = 8 |
| `SingleDoor` | `HousingLayoutRestriction` | = 9 |

### HousingPetBehaviorType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingPetBehaviorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Stationary` | `HousingPetBehaviorType` | = 0 |
| `Wander` | `HousingPetBehaviorType` | = 1 |

### HousingPlotOwnerType

*Enumeration* · 4 values, 0..3

Access values as `Enum.HousingPlotOwnerType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingPlotOwnerType` | = 0 |
| `Stranger` | `HousingPlotOwnerType` | = 1 |
| `Friend` | `HousingPlotOwnerType` | = 2 |
| `Self` | `HousingPlotOwnerType` | = 3 |

### HousingResult

*Enumeration* · 113 values, 0..112

Access values as `Enum.HousingResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `HousingResult` | = 0 |
| `AccountBanned` | `HousingResult` | = 1 |
| `ActionLockedByCombat` | `HousingResult` | = 2 |
| `BlueprintCodeInvalid` | `HousingResult` | = 3 |
| `BlueprintDyeFailed` | `HousingResult` | = 4 |
| `BlueprintGenericExportError` | `HousingResult` | = 5 |
| `BlueprintGenericImportError` | `HousingResult` | = 6 |
| `BlueprintLocationInvalid` | `HousingResult` | = 7 |
| `BlueprintNameInvalid` | `HousingResult` | = 8 |
| `BlueprintNotFound` | `HousingResult` | = 9 |
| `BlueprintRequirementsUnmet` | `HousingResult` | = 10 |
| `BlueprintRoomPlacementRequired` | `HousingResult` | = 11 |
| `BlueprintTypeInvalid` | `HousingResult` | = 12 |
| `BlueprintTypeLocationInvalid` | `HousingResult` | = 13 |
| `BlueprintStorageLimit` | `HousingResult` | = 14 |
| `BlueprintVersionInvalid` | `HousingResult` | = 15 |
| `BoundsFailureChildren` | `HousingResult` | = 16 |
| `BoundsFailurePlot` | `HousingResult` | = 17 |
| `BoundsFailureRoom` | `HousingResult` | = 18 |
| `BoundToStartingArea` | `HousingResult` | = 19 |
| `CannotAfford` | `HousingResult` | = 20 |
| `CharterComplete` | `HousingResult` | = 21 |
| `CollisionInvalid` | `HousingResult` | = 22 |
| `DbError` | `HousingResult` | = 23 |
| `DecorCannotBeRedeemed` | `HousingResult` | = 24 |
| `DecorItemNotDestroyable` | `HousingResult` | = 25 |
| `DecorNotFound` | `HousingResult` | = 26 |
| `DecorNotFoundInStorage` | `HousingResult` | = 27 |
| `DuplicateCharterSignature` | `HousingResult` | = 28 |
| `FilterRejected` | `HousingResult` | = 29 |
| `FixtureCantDeleteDoor` | `HousingResult` | = 30 |
| `FixtureHookEmpty` | `HousingResult` | = 31 |
| `FixtureHookOccupied` | `HousingResult` | = 32 |
| `FixtureHouseTypeMismatch` | `HousingResult` | = 33 |
| `FixtureNotFound` | `HousingResult` | = 34 |
| `FixtureSizeMismatch` | `HousingResult` | = 35 |
| `FixtureTypeMismatch` | `HousingResult` | = 36 |
| `GenericFailure` | `HousingResult` | = 37 |
| `GuildMoreAccountsNeeded` | `HousingResult` | = 38 |
| `GuildMoreActivePlayersNeeded` | `HousingResult` | = 39 |
| `GuildNotLoaded` | `HousingResult` | = 40 |
| `HouseEditLockFailed` | `HousingResult` | = 41 |
| `HouseExteriorAlreadyThatSize` | `HousingResult` | = 42 |
| `HouseExteriorAlreadyThatType` | `HousingResult` | = 43 |
| `HouseExteriorRootNotFound` | `HousingResult` | = 44 |
| `HouseExteriorTypeNeighborhoodMismatch` | `HousingResult` | = 45 |
| `HouseExteriorTypeNotFound` | `HousingResult` | = 46 |
| `HouseExteriorTypeSizeMismatch` | `HousingResult` | = 47 |
| `HouseExteriorSizeNotAvailable` | `HousingResult` | = 48 |
| `HookNotChildOfFixture` | `HousingResult` | = 49 |
| `HouseNotFound` | `HousingResult` | = 50 |
| `IncorrectFaction` | `HousingResult` | = 51 |
| `InvalidDecorItem` | `HousingResult` | = 52 |
| `InvalidDistance` | `HousingResult` | = 53 |
| `InvalidExteriorDocument` | `HousingResult` | = 54 |
| `InvalidGuild` | `HousingResult` | = 55 |
| `InvalidHouse` | `HousingResult` | = 56 |
| `InvalidInstance` | `HousingResult` | = 57 |
| `InvalidInteraction` | `HousingResult` | = 58 |
| `InvalidInteriorDocument` | `HousingResult` | = 59 |
| `InvalidLightOverlap` | `HousingResult` | = 60 |
| `InvalidMap` | `HousingResult` | = 61 |
| `InvalidNeighborhoodName` | `HousingResult` | = 62 |
| `InvalidRoomLayout` | `HousingResult` | = 63 |
| `InsufficientRoomBudget` | `HousingResult` | = 64 |
| `LockedByOtherPlayer` | `HousingResult` | = 65 |
| `LockOperationFailed` | `HousingResult` | = 66 |
| `MaxPlacedDecorReached` | `HousingResult` | = 67 |
| `MaxPetDecorReached` | `HousingResult` | = 68 |
| `MaxPreviewDecorReached` | `HousingResult` | = 69 |
| `MaxStorageDecorReached` | `HousingResult` | = 70 |
| `MessageTooLong` | `HousingResult` | = 71 |
| `MissingCoreFixture` | `HousingResult` | = 72 |
| `MissingDye` | `HousingResult` | = 73 |
| `MissingExpansionAccess` | `HousingResult` | = 74 |
| `MissingFactionMap` | `HousingResult` | = 75 |
| `MissingPrivateNeighborhoodInvite` | `HousingResult` | = 76 |
| `MoreHouseSlotsNeeded` | `HousingResult` | = 77 |
| `MoreSignaturesNeeded` | `HousingResult` | = 78 |
| `NeighborhoodNotFound` | `HousingResult` | = 79 |
| `NoNeighborhoodOwnershipRequests` | `HousingResult` | = 80 |
| `NotInDecorEditMode` | `HousingResult` | = 81 |
| `NotInFixtureEditMode` | `HousingResult` | = 82 |
| `NotInLayoutEditMode` | `HousingResult` | = 83 |
| `NotInsideHouse` | `HousingResult` | = 84 |
| `NotOnOwnedPlot` | `HousingResult` | = 85 |
| `OperationAborted` | `HousingResult` | = 86 |
| `OwnerNotInGuild` | `HousingResult` | = 87 |
| `PermissionDenied` | `HousingResult` | = 88 |
| `PlacementTargetInvalid` | `HousingResult` | = 89 |
| `PlayerNotFound` | `HousingResult` | = 90 |
| `PlayerNotInInstance` | `HousingResult` | = 91 |
| `PlotNotFound` | `HousingResult` | = 92 |
| `PlotNotVacant` | `HousingResult` | = 93 |
| `PlotReservationCooldown` | `HousingResult` | = 94 |
| `PlotReserved` | `HousingResult` | = 95 |
| `RoomNotFound` | `HousingResult` | = 96 |
| `RoomPlacementOutOfBounds` | `HousingResult` | = 97 |
| `RoomUpdateFailed` | `HousingResult` | = 98 |
| `RpcFailure` | `HousingResult` | = 99 |
| `ServiceNotAvailable` | `HousingResult` | = 100 |
| `StaticDataNotFound` | `HousingResult` | = 101 |
| `TimeoutLimit` | `HousingResult` | = 102 |
| `TimerunningNotAllowed` | `HousingResult` | = 103 |
| `TokenRequired` | `HousingResult` | = 104 |
| `TooManyRequests` | `HousingResult` | = 105 |
| `TransactionFailure` | `HousingResult` | = 106 |
| `UncollectedExteriorFixture` | `HousingResult` | = 107 |
| `UncollectedHouseType` | `HousingResult` | = 108 |
| `UncollectedRoom` | `HousingResult` | = 109 |
| `UncollectedRoomMaterial` | `HousingResult` | = 110 |
| `UncollectedRoomTheme` | `HousingResult` | = 111 |
| `UnlockOperationFailed` | `HousingResult` | = 112 |

### HousingRoomComponentCeilingType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingRoomComponentCeilingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Flat` | `HousingRoomComponentCeilingType` | = 0 |
| `Vaulted` | `HousingRoomComponentCeilingType` | = 1 |

### HousingRoomComponentDoorType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingRoomComponentDoorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentDoorType` | = 0 |
| `Doorway` | `HousingRoomComponentDoorType` | = 1 |
| `Threshold` | `HousingRoomComponentDoorType` | = 2 |

### HousingRoomComponentFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingRoomComponentFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentFlags` | = 0 |
| `HiddenInLayoutMode` | `HousingRoomComponentFlags` | = 1 |

### HousingRoomComponentFloorType

*Enumeration* · 1 values, 0..0

Access values as `Enum.HousingRoomComponentFloorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Floor` | `HousingRoomComponentFloorType` | = 0 |

### HousingRoomComponentOptionFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingRoomComponentOptionFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentOptionFlags` | = 0 |
| `IsDefault` | `HousingRoomComponentOptionFlags` | = 1 |

### HousingRoomComponentOptionType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingRoomComponentOptionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Cosmetic` | `HousingRoomComponentOptionType` | = 0 |
| `DoorwayWall` | `HousingRoomComponentOptionType` | = 1 |
| `Doorway` | `HousingRoomComponentOptionType` | = 2 |

### HousingRoomComponentStairType

*Enumeration* · 5 values, 0..4

Access values as `Enum.HousingRoomComponentStairType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentStairType` | = 0 |
| `StartToEnd` | `HousingRoomComponentStairType` | = 1 |
| `StartToMiddle` | `HousingRoomComponentStairType` | = 2 |
| `MiddleToMiddle` | `HousingRoomComponentStairType` | = 3 |
| `MiddleToEnd` | `HousingRoomComponentStairType` | = 4 |

### HousingRoomComponentTextureFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingRoomComponentTextureFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentTextureFlags` | = 0 |
| `UnlockedByDefault` | `HousingRoomComponentTextureFlags` | = 1 |

### HousingRoomComponentType

*Enumeration* · 8 values, 0..7

Access values as `Enum.HousingRoomComponentType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomComponentType` | = 0 |
| `Wall` | `HousingRoomComponentType` | = 1 |
| `Floor` | `HousingRoomComponentType` | = 2 |
| `Ceiling` | `HousingRoomComponentType` | = 3 |
| `Stairs` | `HousingRoomComponentType` | = 4 |
| `Pillar` | `HousingRoomComponentType` | = 5 |
| `DoorwayWall` | `HousingRoomComponentType` | = 6 |
| `Doorway` | `HousingRoomComponentType` | = 7 |

### HousingRoomFlags

*Enumeration* · 5 values, 0..8

Access values as `Enum.HousingRoomFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingRoomFlags` | = 0 |
| `BaseRoom` | `HousingRoomFlags` | = 1 |
| `HasStairs` | `HousingRoomFlags` | = 2 |
| `UnlockedByDefault` | `HousingRoomFlags` | = 4 |
| `HasCustomGeometry` | `HousingRoomFlags` | = 8 |

### HousingThemeFlags

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingThemeFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingThemeFlags` | = 0 |
| `UnlockedByDefault` | `HousingThemeFlags` | = 1 |
| `ShowInStyleSelector` | `HousingThemeFlags` | = 2 |

### HousingThrottleType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingThrottleType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `General` | `HousingThrottleType` | = 0 |
| `Decoration` | `HousingThrottleType` | = 1 |

### NeighborhoodFlags

*Enumeration* · 3 values, 0..2

Access values as `Enum.NeighborhoodFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `NeighborhoodFlags` | = 0 |
| `PoolParent` | `NeighborhoodFlags` | = 1 |
| `OpenToPublic` | `NeighborhoodFlags` | = 2 |

### NeighborhoodInviteResult

*Enumeration* · 12 values, 0..11

Access values as `Enum.NeighborhoodInviteResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `NeighborhoodInviteResult` | = 0 |
| `DbError` | `NeighborhoodInviteResult` | = 1 |
| `RpcFailure` | `NeighborhoodInviteResult` | = 2 |
| `GenericFailure` | `NeighborhoodInviteResult` | = 3 |
| `Permission` | `NeighborhoodInviteResult` | = 4 |
| `Faction` | `NeighborhoodInviteResult` | = 5 |
| `PendingInvitation` | `NeighborhoodInviteResult` | = 6 |
| `InviteLimit` | `NeighborhoodInviteResult` | = 7 |
| `NotEnoughPlots` | `NeighborhoodInviteResult` | = 8 |
| `NotFound` | `NeighborhoodInviteResult` | = 9 |
| `TooManyRequests` | `NeighborhoodInviteResult` | = 10 |
| `AlreadyInNeighborhood` | `NeighborhoodInviteResult` | = 11 |

### NeighborhoodMapFlags

*Enumeration* · 4 values, 0..4

Access values as `Enum.NeighborhoodMapFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `NeighborhoodMapFlags` | = 0 |
| `AlliancePurchasable` | `NeighborhoodMapFlags` | = 1 |
| `HordePurchasable` | `NeighborhoodMapFlags` | = 2 |
| `CanSystemGenerate` | `NeighborhoodMapFlags` | = 4 |

### RetroactiveDecorRewardFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.RetroactiveDecorRewardFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `RetroactiveDecorRewardFlags` | = 0 |
| `AllCriteriaRequired` | `RetroactiveDecorRewardFlags` | = 1 |

### RoomConnectionType

*Enumeration* · 2 values, 0..1

Access values as `Enum.RoomConnectionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `RoomConnectionType` | = 0 |
| `All` | `RoomConnectionType` | = 1 |

### HousingConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `NeighborhoodNameMaxCharacters` | `number` | = `0` |
| `NeighborhoodNameMinCharacters` | `number` | = `0` |
| `BlueprintNameMaxCharacters` | `number` | = `0` |
| `BlueprintNameMinCharacters` | `number` | = `0` |
| `HOUSING_BLUEPRINTS_MAX_PER_BNET_ACCOUNT` | `number` | = `50` |
| `HOUSING_BLUEPRINTS_MAX_BACKUPS_PER_BNET_ACCOUNT` | `number` | = `10` |
