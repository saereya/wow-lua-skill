# AccountConstants

source `interface/addons/blizzard_apidocumentationgenerated/accountconstantsdocumentation.lua` (FileDataID 4954795)

## Types

### AccountData

*Enumeration* · 20 values, 0..19

Access values as `Enum.AccountData.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Config` | `AccountData` | = 0 |
| `Config2` | `AccountData` | = 1 |
| `Bindings` | `AccountData` | = 2 |
| `Bindings2` | `AccountData` | = 3 |
| `Macros` | `AccountData` | = 4 |
| `Macros2` | `AccountData` | = 5 |
| `UILayout` | `AccountData` | = 6 |
| `ChatSettings` | `AccountData` | = 7 |
| `TtsSettings` | `AccountData` | = 8 |
| `TtsSettings2` | `AccountData` | = 9 |
| `FlaggedIDs` | `AccountData` | = 10 |
| `FlaggedIDs2` | `AccountData` | = 11 |
| `ClickBindings` | `AccountData` | = 12 |
| `UIEditModeAccount` | `AccountData` | = 13 |
| `UIEditModeChar` | `AccountData` | = 14 |
| `FrontendChatSettings` | `AccountData` | = 15 |
| `CharacterListOrder` | `AccountData` | = 16 |
| `CooldownManager` | `AccountData` | = 17 |
| `CooldownManager2` | `AccountData` | = 18 |
| `Shop2PendingOrders` | `AccountData` | = 19 |

### AccountDataUpdateStatus

*Enumeration* · 4 values, 0..3

Access values as `Enum.AccountDataUpdateStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `AccountDataUpdateStatus` | = 0 |
| `Failed` | `AccountDataUpdateStatus` | = 1 |
| `Corrupt` | `AccountDataUpdateStatus` | = 2 |
| `Toobig` | `AccountDataUpdateStatus` | = 3 |

### AccountExportResult

*Enumeration* · 14 values, 0..13

Access values as `Enum.AccountExportResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `AccountExportResult` | = 0 |
| `UnknownError` | `AccountExportResult` | = 1 |
| `Cancelled` | `AccountExportResult` | = 2 |
| `ShuttingDown` | `AccountExportResult` | = 3 |
| `TimedOut` | `AccountExportResult` | = 4 |
| `NoAccountFound` | `AccountExportResult` | = 5 |
| `RequestedInvalidCharacter` | `AccountExportResult` | = 6 |
| `RpcError` | `AccountExportResult` | = 7 |
| `FileInvalid` | `AccountExportResult` | = 8 |
| `FileWriteFailed` | `AccountExportResult` | = 9 |
| `Unavailable` | `AccountExportResult` | = 10 |
| `AlreadyInProgress` | `AccountExportResult` | = 11 |
| `FailedToLockAccount` | `AccountExportResult` | = 12 |
| `FailedToGenerateFile` | `AccountExportResult` | = 13 |

### AccountGetListRequestType

*Enumeration* · 2 values, 0..1

Access values as `Enum.AccountGetListRequestType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `AccountGetListRequestType` | = 0 |
| `Battlepets` | `AccountGetListRequestType` | = 1 |

### AccountSequenceCacheType

*Enumeration* · 3 values, 0..2

Access values as `Enum.AccountSequenceCacheType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `AccountSequenceCacheType` | = 0 |
| `Local` | `AccountSequenceCacheType` | = 1 |
| `HouseDecor` | `AccountSequenceCacheType` | = 2 |

### AccountTransType

*Enumeration* · 67 values, 0..66

Access values as `Enum.AccountTransType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ProxyForwarder` | `AccountTransType` | = 0 |
| `Purchase` | `AccountTransType` | = 1 |
| `Distribution` | `AccountTransType` | = 2 |
| `Battlepet` | `AccountTransType` | = 3 |
| `Achievements` | `AccountTransType` | = 4 |
| `Criteria` | `AccountTransType` | = 5 |
| `Mounts` | `AccountTransType` | = 6 |
| `Characters` | `AccountTransType` | = 7 |
| `Purchases` | `AccountTransType` | = 8 |
| `ArchivedPurchases` | `AccountTransType` | = 9 |
| `Distributions` | `AccountTransType` | = 10 |
| `CurrencyCaps` | `AccountTransType` | = 11 |
| `QuestLog` | `AccountTransType` | = 12 |
| `CriteriaNotif` | `AccountTransType` | = 13 |
| `Settings` | `AccountTransType` | = 14 |
| `FixedLicense` | `AccountTransType` | = 15 |
| `AddLicense` | `AccountTransType` | = 16 |
| `ItemCollections` | `AccountTransType` | = 17 |
| `AuctionableToken` | `AccountTransType` | = 18 |
| `ConsumableToken` | `AccountTransType` | = 19 |
| `VasTransaction` | `AccountTransType` | = 20 |
| `Productitem` | `AccountTransType` | = 21 |
| `TrialBoostHistory` | `AccountTransType` | = 22 |
| `TrialBoostHistories` | `AccountTransType` | = 23 |
| `QuestCriteria` | `AccountTransType` | = 24 |
| `BattlenetAccount` | `AccountTransType` | = 25 |
| `AccountCurrencies` | `AccountTransType` | = 26 |
| `RafRecruiterAcceptances` | `AccountTransType` | = 27 |
| `RafFriendMonth` | `AccountTransType` | = 28 |
| `RafReward` | `AccountTransType` | = 29 |
| `DynamicCriteria` | `AccountTransType` | = 30 |
| `RafActivity` | `AccountTransType` | = 31 |
| `CreateOrderInfo` | `AccountTransType` | = 32 |
| `ProxyHonorInitialConversion` | `AccountTransType` | = 33 |
| `ProxyCreateAccountHonor` | `AccountTransType` | = 34 |
| `ProxyValidateAccountHonor` | `AccountTransType` | = 35 |
| `ProxyGmSetHonor` | `AccountTransType` | = 36 |
| `ProxyGenerateBpayID` | `AccountTransType` | = 37 |
| `AccountNotifications` | `AccountTransType` | = 38 |
| `PerkItemHold` | `AccountTransType` | = 39 |
| `PerkPendingRewards` | `AccountTransType` | = 40 |
| `PerkPastRewards` | `AccountTransType` | = 41 |
| `PerkTransaction` | `AccountTransType` | = 42 |
| `OutstandingRpc` | `AccountTransType` | = 43 |
| `LoadWowlabs` | `AccountTransType` | = 44 |
| `UpgradeAccount` | `AccountTransType` | = 45 |
| `GetOrderStatusByPurchaseID` | `AccountTransType` | = 46 |
| `Items` | `AccountTransType` | = 47 |
| `BankTab` | `AccountTransType` | = 48 |
| `Factions` | `AccountTransType` | = 49 |
| `BitVectors` | `AccountTransType` | = 50 |
| `CombinedQuestLog` | `AccountTransType` | = 51 |
| `PlayerDataElements` | `AccountTransType` | = 52 |
| `CharacterDataMerge` | `AccountTransType` | = 53 |
| `AccountStore` | `AccountTransType` | = 54 |
| `WarbandGroups` | `AccountTransType` | = 55 |
| `Mapping` | `AccountTransType` | = 56 |
| `CharacterItems` | `AccountTransType` | = 57 |
| `CurrencyTransferLog` | `AccountTransType` | = 58 |
| `LgVendorPurchase` | `AccountTransType` | = 59 |
| `SaveWarbandGroups` | `AccountTransType` | = 60 |
| `Profile` | `AccountTransType` | = 61 |
| `WarbandSceneCollection` | `AccountTransType` | = 62 |
| `EventRecords` | `AccountTransType` | = 63 |
| `HousingItem` | `AccountTransType` | = 64 |
| `TransmogOutfitCollection` | `AccountTransType` | = 65 |
| `HouseInitiativeFavor` | `AccountTransType` | = 66 |

### BnetAccountFlag

*Enumeration* · 23 values, 0..2097152

Access values as `Enum.BnetAccountFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `BnetAccountFlag` | = 0 |
| `BattlePetTrainer` | `BnetAccountFlag` | = 1 |
| `RafVeteranNotified` | `BnetAccountFlag` | = 2 |
| `TwitterLinked` | `BnetAccountFlag` | = 4 |
| `TwitterHasTempSecret` | `BnetAccountFlag` | = 8 |
| `Employee` | `BnetAccountFlag` | = 16 |
| `EmployeeFlagIsManual` | `BnetAccountFlag` | = 32 |
| `AccountQuestBitFixUp` | `BnetAccountFlag` | = 64 |
| `AchievementsToBi` | `BnetAccountFlag` | = 128 |
| `InvalidTransmogsFixUp` | `BnetAccountFlag` | = 256 |
| `InvalidTransmogsFixUp2` | `BnetAccountFlag` | = 512 |
| `GdprErased` | `BnetAccountFlag` | = 1024 |
| `DarkRealmLightCopy` | `BnetAccountFlag` | = 2048 |
| `QuestLogFlagsFixUp` | `BnetAccountFlag` | = 4096 |
| `WasSecured` | `BnetAccountFlag` | = 8192 |
| `LockedForExport` | `BnetAccountFlag` | = 16384 |
| `CanBuyAhGameTimeTokens` | `BnetAccountFlag` | = 32768 |
| `PetAchievementFixUp` | `BnetAccountFlag` | = 65536 |
| `IsLegacy` | `BnetAccountFlag` | = 131072 |
| `CataLegendaryMountChecked` | `BnetAccountFlag` | = 262144 |
| `CataLegendaryMountObtained` | `BnetAccountFlag` | = 524288 |
| `MopQuestLogFlagsFixUp` | `BnetAccountFlag` | = 1048576 |
| `Unused` | `BnetAccountFlag` | = 2097152 |

### ChallengeModeHistoryFlags

*Enumeration* · 2 values, 0..1

Access values as `Enum.ChallengeModeHistoryFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ChallengeModeHistoryFlags` | = 0 |
| `ConfirmedLeaver` | `ChallengeModeHistoryFlags` | = 1 |

### ChallengeModeHistoryResult

*Enumeration* · 2 values, 0..1

Access values as `Enum.ChallengeModeHistoryResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Successful` | `ChallengeModeHistoryResult` | = 0 |
| `Leaver` | `ChallengeModeHistoryResult` | = 1 |

### ChallengeModeHistoryStatus

*Enumeration* · 2 values, 0..1

Access values as `Enum.ChallengeModeHistoryStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Normal` | `ChallengeModeHistoryStatus` | = 0 |
| `Leaver` | `ChallengeModeHistoryStatus` | = 1 |

### DisableAccountProfilesFlags

*Enumeration* · 7 values, 0..32

Access values as `Enum.DisableAccountProfilesFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `DisableAccountProfilesFlags` | = 0 |
| `Document` | `DisableAccountProfilesFlags` | = 1 |
| `SharedCollections` | `DisableAccountProfilesFlags` | = 2 |
| `MountsCollections` | `DisableAccountProfilesFlags` | = 4 |
| `PetsCollections` | `DisableAccountProfilesFlags` | = 8 |
| `ItemsCollections` | `DisableAccountProfilesFlags` | = 16 |
| `DecorsCollections` | `DisableAccountProfilesFlags` | = 32 |

### ItemCollectionType

*Enumeration* · 14 values, 0..13

Access values as `Enum.ItemCollectionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ItemCollectionType` | = 0 |
| `Toy` | `ItemCollectionType` | = 1 |
| `Heirloom` | `ItemCollectionType` | = 2 |
| `Transmog` | `ItemCollectionType` | = 3 |
| `TransmogSetFavorite` | `ItemCollectionType` | = 4 |
| `RuneforgeLegendaryAbility` | `ItemCollectionType` | = 5 |
| `TransmogIllusion` | `ItemCollectionType` | = 6 |
| `WarbandScene` | `ItemCollectionType` | = 7 |
| `Room` | `ItemCollectionType` | = 8 |
| `ExteriorFixture` | `ItemCollectionType` | = 9 |
| `RoomTheme` | `ItemCollectionType` | = 10 |
| `RoomMaterial` | `ItemCollectionType` | = 11 |
| `TransmogOutfit` | `ItemCollectionType` | = 12 |
| `HouseType` | `ItemCollectionType` | = 13 |

### SdToggleUsageLocation

*Enumeration* · 4 values, 0..3

Access values as `Enum.SdToggleUsageLocation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `BeforeLogin` | `SdToggleUsageLocation` | = 0 |
| `CharacterCreation` | `SdToggleUsageLocation` | = 1 |
| `BarberShop` | `SdToggleUsageLocation` | = 2 |
| `OptionsMenu` | `SdToggleUsageLocation` | = 3 |
