# BattlepayConstants

source `interface/addons/blizzard_apidocumentationgenerated/battlepayconstantsdocumentation.lua` (FileDataID 7335139)

## Types

### BulkPurchaseResult

*Enumeration* · 8 values, 0..7

Access values as `Enum.BulkPurchaseResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ResultOk` | `BulkPurchaseResult` | = 0 |
| `ResultInProgress` | `BulkPurchaseResult` | = 1 |
| `ResultPartialSuccess` | `BulkPurchaseResult` | = 2 |
| `ResultFailed` | `BulkPurchaseResult` | = 3 |
| `ResultTooManyProducts` | `BulkPurchaseResult` | = 4 |
| `ResultSystemDisabled` | `BulkPurchaseResult` | = 5 |
| `ResultInsufficientFunds` | `BulkPurchaseResult` | = 6 |
| `ResultPurchaseTimeout` | `BulkPurchaseResult` | = 7 |

### BulkPurchaseStatus

*Enumeration* · 5 values, 0..4

Access values as `Enum.BulkPurchaseStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `PlacingOrders` | `BulkPurchaseStatus` | = 0 |
| `PurchasesPending` | `BulkPurchaseStatus` | = 1 |
| `FetchEntitlements` | `BulkPurchaseStatus` | = 2 |
| `Done` | `BulkPurchaseStatus` | = 3 |
| `Failed` | `BulkPurchaseStatus` | = 4 |

### BulkRefundResult

*Enumeration* · 6 values, 0..5

Access values as `Enum.BulkRefundResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ResultOk` | `BulkRefundResult` | = 0 |
| `ResultFailed` | `BulkRefundResult` | = 1 |
| `ResultInvalidRequest` | `BulkRefundResult` | = 2 |
| `ResultRefundWindowExpired` | `BulkRefundResult` | = 3 |
| `ResultSystemDisabled` | `BulkRefundResult` | = 4 |
| `ResultTimeout` | `BulkRefundResult` | = 5 |

### CanRedeemTokenForBalanceResult

*Enumeration* · 2 values, 0..1

Access values as `Enum.CanRedeemTokenForBalanceResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `CanRedeemTokenForBalanceResult` | = 0 |
| `FailureCap` | `CanRedeemTokenForBalanceResult` | = 1 |

### LoginTicketLicenses

*Enumeration* · 1 values, 11486..11486

Access values as `Enum.LoginTicketLicenses.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `GmLicense` | `LoginTicketLicenses` | = 11486 |

### PurchaseResult

*Enumeration* · 72 values, 0..71

Access values as `Enum.PurchaseResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `PurchaseResult` | = 0 |
| `ErrorRiskDenied` | `PurchaseResult` | = 1 |
| `ErrorOrderFailed` | `PurchaseResult` | = 2 |
| `ErrorClientTimeout` | `PurchaseResult` | = 3 |
| `ErrorClientDeclined` | `PurchaseResult` | = 4 |
| `ErrorFailedToCreatePurchaseRecord` | `PurchaseResult` | = 5 |
| `ErrorFailedToGetPurchaseID` | `PurchaseResult` | = 6 |
| `ErrorFailedToSaveMopAndRiskStatus` | `PurchaseResult` | = 7 |
| `ErrorFailedToSaveMopAndRiskResponse` | `PurchaseResult` | = 8 |
| `ErrorClientGone` | `PurchaseResult` | = 9 |
| `ErrorFailedToSavePlaceOrderStatus` | `PurchaseResult` | = 10 |
| `ErrorBattlepayTimeoutMopAndRisk` | `PurchaseResult` | = 11 |
| `ErrorCurrencyInvalidInRegion` | `PurchaseResult` | = 12 |
| `ErrorBattlepayTemporarilyUnavailable` | `PurchaseResult` | = 13 |
| `ErrorBattlepayDisabled` | `PurchaseResult` | = 14 |
| `ErrorServerRestarted` | `PurchaseResult` | = 15 |
| `ErrorInvalidProduct` | `PurchaseResult` | = 16 |
| `ErrorInvalidRegionGroupMask` | `PurchaseResult` | = 17 |
| `ErrorProductInvalidInRegion` | `PurchaseResult` | = 18 |
| `ErrorDistributionObjectNotFound` | `PurchaseResult` | = 19 |
| `ErrorDistributionObjectAlreadyAssigned` | `PurchaseResult` | = 20 |
| `ErrorRiskResponseMissingScore` | `PurchaseResult` | = 21 |
| `ErrorMopAndRiskAmqpRpcFailed` | `PurchaseResult` | = 22 |
| `ErrorMopAndRiskRpcErrorFromBattlepay` | `PurchaseResult` | = 23 |
| `ErrorMopAndRiskUnexpectedResponseFromBattlepay` | `PurchaseResult` | = 24 |
| `ErrorMopAndRiskNoValidPaymentMethods` | `PurchaseResult` | = 25 |
| `ErrorOrderCanceledPriceChange` | `PurchaseResult` | = 26 |
| `ErrorBuyingProductNotAllowedInGlueScreen` | `PurchaseResult` | = 27 |
| `ErrorMopAndRiskNotEnoughBalance` | `PurchaseResult` | = 28 |
| `ErrorPlaceOrderNotEnoughBalance` | `PurchaseResult` | = 29 |
| `ErrorProgrammerManualFail` | `PurchaseResult` | = 30 |
| `ErrorThrottledByUserServer` | `PurchaseResult` | = 31 |
| `ErrorBuyingProductNotAllowedInWorld` | `PurchaseResult` | = 32 |
| `ErrorBlockedByParentalControls` | `PurchaseResult` | = 33 |
| `ErrorNoStorePurchaseFlagIsSet` | `PurchaseResult` | = 34 |
| `ErrorDistributionObjectInvalidChoice` | `PurchaseResult` | = 35 |
| `ErrorInvalidCreditCardExpiryDate` | `PurchaseResult` | = 36 |
| `ErrorAuthorizingPayment` | `PurchaseResult` | = 37 |
| `ErrorPaymentProviderDeniedPayment` | `PurchaseResult` | = 38 |
| `ErrorOverSpendingLimit` | `PurchaseResult` | = 39 |
| `ErrorClientTimeoutChallenge` | `PurchaseResult` | = 40 |
| `ErrorClientDeclinedChallenge` | `PurchaseResult` | = 41 |
| `ErrorDistributionObjectInvalidTarget` | `PurchaseResult` | = 42 |
| `ErrorFixedLicenseProductAlreadyExists` | `PurchaseResult` | = 43 |
| `ErrorDistributionObjectTrialBlocked` | `PurchaseResult` | = 44 |
| `ErrorDistributionObjectExpansionBlocked` | `PurchaseResult` | = 45 |
| `ErrorOwnsConsumableToken` | `PurchaseResult` | = 46 |
| `ErrorTooManyTokens` | `PurchaseResult` | = 47 |
| `ErrorCommerceServerDisabled` | `PurchaseResult` | = 48 |
| `ErrorFailedToWriteVasPurchaseID` | `PurchaseResult` | = 49 |
| `ErrorFailedToWriteVasLicenseID` | `PurchaseResult` | = 50 |
| `ErrorCharacterUpgradeOperationInProgress` | `PurchaseResult` | = 51 |
| `ErrorInvalidPlatform` | `PurchaseResult` | = 52 |
| `ErrorInvalidDeviceID` | `PurchaseResult` | = 53 |
| `ErrorFailedToSaveValidatePurchaseStatus` | `PurchaseResult` | = 54 |
| `ErrorFailedToSaveValidatePurchaseResponse` | `PurchaseResult` | = 55 |
| `ErrorBattlepayTimeoutValidatePurchase` | `PurchaseResult` | = 56 |
| `ErrorProductNotPurchasable` | `PurchaseResult` | = 57 |
| `ErrorFailedToSaveClientCheckoutStatus` | `PurchaseResult` | = 58 |
| `ErrorFailedOldPurchaseFlow` | `PurchaseResult` | = 59 |
| `ErrorClientCheckoutTimeout` | `PurchaseResult` | = 60 |
| `ErrorFailedToSaveValidationHashStatus` | `PurchaseResult` | = 61 |
| `ErrorBattlepayTimeoutValidationHash` | `PurchaseResult` | = 62 |
| `ErrorClientCheckoutCanceledOrFailed` | `PurchaseResult` | = 63 |
| `ErrorCouldNotGetValidationHash` | `PurchaseResult` | = 64 |
| `ErrorDistributionObjectWrongGameAccount` | `PurchaseResult` | = 65 |
| `ErrorClientRestricted` | `PurchaseResult` | = 66 |
| `ErrorFailedToSaveRedeemTokenStatus` | `PurchaseResult` | = 67 |
| `ErrorInvalidPurchaseID` | `PurchaseResult` | = 68 |
| `ErrorTokenRedemptionOrderFailed` | `PurchaseResult` | = 69 |
| `ErrorVasTransactionCreateFailed` | `PurchaseResult` | = 70 |
| `ErrorInManualReview` | `PurchaseResult` | = 71 |

### SimpleOrderStatus

*Enumeration* · 5 values, 0..4

Access values as `Enum.SimpleOrderStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `SimpleOrderStatus` | = 0 |
| `Creating` | `SimpleOrderStatus` | = 1 |
| `InProgress` | `SimpleOrderStatus` | = 2 |
| `Success` | `SimpleOrderStatus` | = 3 |
| `Failed` | `SimpleOrderStatus` | = 4 |

### VasTransactionPurchaseResult

*Enumeration* · 145 values, 0..20097

Access values as `Enum.VasTransactionPurchaseResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `VasTransactionPurchaseResult` | = 0 |
| `VasPurchaseDisabled` | `VasTransactionPurchaseResult` | = 1 |
| `NoneCharacter` | `VasTransactionPurchaseResult` | = 2 |
| `NoneProduct` | `VasTransactionPurchaseResult` | = 3 |
| `OnlyOneVasAtATime` | `VasTransactionPurchaseResult` | = 4 |
| `InvalidDestinationRealm` | `VasTransactionPurchaseResult` | = 5 |
| `InvalidDestinationAccount` | `VasTransactionPurchaseResult` | = 6 |
| `InvalidSourceAccount` | `VasTransactionPurchaseResult` | = 7 |
| `DisallowedSourceAccount` | `VasTransactionPurchaseResult` | = 8 |
| `DisallowedDestinationAccount` | `VasTransactionPurchaseResult` | = 9 |
| `UnknownError` | `VasTransactionPurchaseResult` | = 10 |
| `LowerBoxLevel` | `VasTransactionPurchaseResult` | = 11 |
| `InvalidDistribution` | `VasTransactionPurchaseResult` | = 12 |
| `InvalidBpayProductID` | `VasTransactionPurchaseResult` | = 13 |
| `InvalidBpayDeliverableID` | `VasTransactionPurchaseResult` | = 14 |
| `InvalidBpayProductType` | `VasTransactionPurchaseResult` | = 15 |
| `EndServerErrors` | `VasTransactionPurchaseResult` | = 16 |
| `BeginProxyErrors` | `VasTransactionPurchaseResult` | = 17 |
| `ProxyBadObjType` | `VasTransactionPurchaseResult` | = 18 |
| `ProxyObjNotInDb` | `VasTransactionPurchaseResult` | = 19 |
| `ProxyUniqueKey` | `VasTransactionPurchaseResult` | = 20 |
| `ProxyDbError` | `VasTransactionPurchaseResult` | = 21 |
| `ProxyDataInvalid` | `VasTransactionPurchaseResult` | = 22 |
| `ProxyLostProxyConnection` | `VasTransactionPurchaseResult` | = 23 |
| `ProxyLocksFailed` | `VasTransactionPurchaseResult` | = 24 |
| `ProxyMissingResultsPtr` | `VasTransactionPurchaseResult` | = 25 |
| `ProxyLockedForTransfer` | `VasTransactionPurchaseResult` | = 26 |
| `ProxyNoReturnValue` | `VasTransactionPurchaseResult` | = 27 |
| `ProxyDeleteNotSupported` | `VasTransactionPurchaseResult` | = 28 |
| `ProxyObjDropped` | `VasTransactionPurchaseResult` | = 29 |
| `ProxyCannotDeleteGuildLeader` | `VasTransactionPurchaseResult` | = 30 |
| `ProxyCannotDeleteArenaCaptain` | `VasTransactionPurchaseResult` | = 31 |
| `ProxyMoneyLimitExceeded` | `VasTransactionPurchaseResult` | = 32 |
| `ProxyBadRequestContained` | `VasTransactionPurchaseResult` | = 33 |
| `ProxyIsReadonly` | `VasTransactionPurchaseResult` | = 34 |
| `ProxyBadDbType` | `VasTransactionPurchaseResult` | = 35 |
| `ProxyOperationAlreadyInProgress` | `VasTransactionPurchaseResult` | = 36 |
| `ProxyExternalUpdateDetected` | `VasTransactionPurchaseResult` | = 37 |
| `ProxyCharacterLevelTooHigh` | `VasTransactionPurchaseResult` | = 38 |
| `ProxyCharacterTransferred` | `VasTransactionPurchaseResult` | = 39 |
| `ProxyCharacterTransferredNoBoostInProgress` | `VasTransactionPurchaseResult` | = 40 |
| `ProxyLockedForUpgrade` | `VasTransactionPurchaseResult` | = 41 |
| `ProxyLockedForToken` | `VasTransactionPurchaseResult` | = 42 |
| `ProxyLockedForVas` | `VasTransactionPurchaseResult` | = 43 |
| `ProxyGenericError` | `VasTransactionPurchaseResult` | = 44 |
| `ProxyCannotInsertNull` | `VasTransactionPurchaseResult` | = 45 |
| `ProxyCannotUndeleteTrialBoostCharacter` | `VasTransactionPurchaseResult` | = 46 |
| `ProxyPredicateFailed` | `VasTransactionPurchaseResult` | = 47 |
| `ProxyWeeklyRewardNotFound` | `VasTransactionPurchaseResult` | = 48 |
| `ProxyInsertRequestContainedNoData` | `VasTransactionPurchaseResult` | = 49 |
| `ProxyInvalidKey` | `VasTransactionPurchaseResult` | = 50 |
| `ProxyBindFailed` | `VasTransactionPurchaseResult` | = 51 |
| `ProxyTooManyRows` | `VasTransactionPurchaseResult` | = 52 |
| `ProxyCharacterHasWoWToken` | `VasTransactionPurchaseResult` | = 53 |
| `ProxyTooBusyBackOff` | `VasTransactionPurchaseResult` | = 54 |
| `ProxyAccountDataTooBig` | `VasTransactionPurchaseResult` | = 55 |
| `EndProxyErrors` | `VasTransactionPurchaseResult` | = 56 |
| `BeginDbErrors` | `VasTransactionPurchaseResult` | = 20010 |
| `DbRealmNotEligible` | `VasTransactionPurchaseResult` | = 20011 |
| `DbCannotMoveGuildmaster` | `VasTransactionPurchaseResult` | = 20012 |
| `DbMaxCharactersOnServer` | `VasTransactionPurchaseResult` | = 20013 |
| `DbNoMixedAlliance` | `VasTransactionPurchaseResult` | = 20014 |
| `DbDuplicateCharacterName` | `VasTransactionPurchaseResult` | = 20015 |
| `DbHasMail` | `VasTransactionPurchaseResult` | = 20016 |
| `DbAccountDoesNotOwnCharacter` | `VasTransactionPurchaseResult` | = 20017 |
| `DbMoveInProgress` | `VasTransactionPurchaseResult` | = 20018 |
| `DbCharacterDoesNotExist` | `VasTransactionPurchaseResult` | = 20019 |
| `DbNoCopiesAvailable` | `VasTransactionPurchaseResult` | = 20020 |
| `DbUnderMinLevelReq` | `VasTransactionPurchaseResult` | = 20021 |
| `DbIneligibleTargetRealm` | `VasTransactionPurchaseResult` | = 20022 |
| `DbTransferDateTooSoon` | `VasTransactionPurchaseResult` | = 20023 |
| `DbNewNameTooLong` | `VasTransactionPurchaseResult` | = 20024 |
| `DbCharNotLocked` | `VasTransactionPurchaseResult` | = 20025 |
| `DbCharLocked` | `VasTransactionPurchaseResult` | = 20026 |
| `DbAllianceNotEligible` | `VasTransactionPurchaseResult` | = 20027 |
| `DbBatchProcessingDisabled` | `VasTransactionPurchaseResult` | = 20028 |
| `DbNoneBatchQueueID` | `VasTransactionPurchaseResult` | = 20029 |
| `DbTransferNotFinalized` | `VasTransactionPurchaseResult` | = 20030 |
| `DbTransferNotCancellable` | `VasTransactionPurchaseResult` | = 20031 |
| `DbTooMuchMoneyForLevel` | `VasTransactionPurchaseResult` | = 20032 |
| `DbHasAuctions` | `VasTransactionPurchaseResult` | = 20033 |
| `DbLastSaveTooRecent` | `VasTransactionPurchaseResult` | = 20034 |
| `DbTransferNotLockable` | `VasTransactionPurchaseResult` | = 20035 |
| `DbTransferNotUnlockable` | `VasTransactionPurchaseResult` | = 20036 |
| `DbNoneRealmForEvent` | `VasTransactionPurchaseResult` | = 20037 |
| `DbEventRealmClosed` | `VasTransactionPurchaseResult` | = 20038 |
| `DbNoneTemplateForEvent` | `VasTransactionPurchaseResult` | = 20039 |
| `DbInventoryCorrupt` | `VasTransactionPurchaseResult` | = 20040 |
| `DbCouldNotObtainCharLock` | `VasTransactionPurchaseResult` | = 20041 |
| `DbNoneLockID` | `VasTransactionPurchaseResult` | = 20042 |
| `DbLockNotAcknowledged` | `VasTransactionPurchaseResult` | = 20043 |
| `DbLockAlreadyRequested` | `VasTransactionPurchaseResult` | = 20044 |
| `DbNoneSupportQueueID` | `VasTransactionPurchaseResult` | = 20045 |
| `DbNoneSupportActionID` | `VasTransactionPurchaseResult` | = 20046 |
| `DbNotRollbackable` | `VasTransactionPurchaseResult` | = 20047 |
| `DbNotMovebackable` | `VasTransactionPurchaseResult` | = 20048 |
| `DbRenameAlreadyRequested` | `VasTransactionPurchaseResult` | = 20049 |
| `DbReservationExpired` | `VasTransactionPurchaseResult` | = 20050 |
| `DbNameNotAvailable` | `VasTransactionPurchaseResult` | = 20051 |
| `DbLastRenameTooRecent` | `VasTransactionPurchaseResult` | = 20052 |
| `DbReservationDoesNotMatch` | `VasTransactionPurchaseResult` | = 20053 |
| `DbLastRequestTooSoon` | `VasTransactionPurchaseResult` | = 20054 |
| `DbAlreadyRenameFlagged` | `VasTransactionPurchaseResult` | = 20055 |
| `DbMultipleTransferCn` | `VasTransactionPurchaseResult` | = 20056 |
| `DbCustomizeAlreadyRequested` | `VasTransactionPurchaseResult` | = 20057 |
| `DbLastCustomizeTooSoon` | `VasTransactionPurchaseResult` | = 20058 |
| `DbWaitingForPayment` | `VasTransactionPurchaseResult` | = 20059 |
| `DbUnableToCustomize` | `VasTransactionPurchaseResult` | = 20060 |
| `DbFactionChangeTooSoon` | `VasTransactionPurchaseResult` | = 20061 |
| `DbRaceClassComboIneligible` | `VasTransactionPurchaseResult` | = 20062 |
| `DbDuplicateSupportRequest` | `VasTransactionPurchaseResult` | = 20063 |
| `DbCannotMoveArenaCaptn` | `VasTransactionPurchaseResult` | = 20064 |
| `DbNoCsiFound` | `VasTransactionPurchaseResult` | = 20065 |
| `DbPendingItemAudit` | `VasTransactionPurchaseResult` | = 20066 |
| `DbBatchStateInvalid` | `VasTransactionPurchaseResult` | = 20067 |
| `DbEventNotActive` | `VasTransactionPurchaseResult` | = 20068 |
| `DbGuildRankInsufficient` | `VasTransactionPurchaseResult` | = 20069 |
| `DbCharacterWithoutGuild` | `VasTransactionPurchaseResult` | = 20070 |
| `DbDeletedGuild` | `VasTransactionPurchaseResult` | = 20071 |
| `DbGmSenorityInsufficient` | `VasTransactionPurchaseResult` | = 20072 |
| `DbAuthenticatorInsufficient` | `VasTransactionPurchaseResult` | = 20073 |
| `DbGuildLevelInsufficient` | `VasTransactionPurchaseResult` | = 20074 |
| `DbRegionalDbNotFound` | `VasTransactionPurchaseResult` | = 20075 |
| `DbIneligibleMapID` | `VasTransactionPurchaseResult` | = 20076 |
| `DbBnetAccountNotProvided` | `VasTransactionPurchaseResult` | = 20077 |
| `DbBpayDeliveryPending` | `VasTransactionPurchaseResult` | = 20078 |
| `DbHasBpayToken` | `VasTransactionPurchaseResult` | = 20079 |
| `DbHasHeirloomItem` | `VasTransactionPurchaseResult` | = 20080 |
| `DbResultSourceAccountBanned` | `VasTransactionPurchaseResult` | = 20081 |
| `DbResultAccountRestricted` | `VasTransactionPurchaseResult` | = 20082 |
| `DbLastSaveTooDistant` | `VasTransactionPurchaseResult` | = 20083 |
| `DbCagedPetInInventory` | `VasTransactionPurchaseResult` | = 20084 |
| `DbOnBoostCooldown` | `VasTransactionPurchaseResult` | = 20085 |
| `DbNewLeaderInvalid` | `VasTransactionPurchaseResult` | = 20086 |
| `DbPvEPvPTransferNotAllowed` | `VasTransactionPurchaseResult` | = 20087 |
| `DbNeedsLevelSquish` | `VasTransactionPurchaseResult` | = 20088 |
| `DbHasUnclaimedCacheRewards` | `VasTransactionPurchaseResult` | = 20089 |
| `DbNeedsEraChoice` | `VasTransactionPurchaseResult` | = 20090 |
| `DbHasNewPlayerExperienceRestriction` | `VasTransactionPurchaseResult` | = 20091 |
| `DbHasCraftingOrders` | `VasTransactionPurchaseResult` | = 20092 |
| `DbNameChangeSkipped` | `VasTransactionPurchaseResult` | = 20093 |
| `DbInvalidName` | `VasTransactionPurchaseResult` | = 20094 |
| `DbBoostProcessingDisabled` | `VasTransactionPurchaseResult` | = 20095 |
| `DbHouseOwnerRestriction` | `VasTransactionPurchaseResult` | = 20096 |
| `EndDbErrors` | `VasTransactionPurchaseResult` | = 20097 |
