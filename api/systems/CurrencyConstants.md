# CurrencyConstants

source `interface/addons/blizzard_apidocumentationgenerated/currencyconstantsdocumentation.lua` (FileDataID 4637084)

## Types

### AccountCurrencyTransferResult

*Enumeration* · 11 values, 0..10

Access values as `Enum.AccountCurrencyTransferResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `AccountCurrencyTransferResult` | = 0 |
| `InvalidCharacter` | `AccountCurrencyTransferResult` | = 1 |
| `CharacterLoggedIn` | `AccountCurrencyTransferResult` | = 2 |
| `InsufficientCurrency` | `AccountCurrencyTransferResult` | = 3 |
| `MaxQuantity` | `AccountCurrencyTransferResult` | = 4 |
| `InvalidCurrency` | `AccountCurrencyTransferResult` | = 5 |
| `NoValidSourceCharacter` | `AccountCurrencyTransferResult` | = 6 |
| `ServerError` | `AccountCurrencyTransferResult` | = 7 |
| `CannotUseCurrency` | `AccountCurrencyTransferResult` | = 8 |
| `TransactionInProgress` | `AccountCurrencyTransferResult` | = 9 |
| `CurrencyTransferDisabled` | `AccountCurrencyTransferResult` | = 10 |

### CurrencyConversionResult

*Enumeration* · 3 values, 0..2

Access values as `Enum.CurrencyConversionResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NoConversion` | `CurrencyConversionResult` | = 0 |
| `Conversion` | `CurrencyConversionResult` | = 1 |
| `SkippedAccountCurrency` | `CurrencyConversionResult` | = 2 |

### CurrencyFilterType

*Enumeration* · 3 values, 0..2

Access values as `Enum.CurrencyFilterType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CurrencyFilterType` | = 0 |
| `DiscoveredOnly` | `CurrencyFilterType` | = 1 |
| `DiscoveredAndAllAccountTransferable` | `CurrencyFilterType` | = 2 |

### CurrencyFlags

*Enumeration* · 32 values, 1..2147483648

Access values as `Enum.CurrencyFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CurrencyTradable` | `CurrencyFlags` | = 1 |
| `CurrencyAppearsInLootWindow` | `CurrencyFlags` | = 2 |
| `CurrencyComputedWeeklyMaximum` | `CurrencyFlags` | = 4 |
| `Currency_100_Scaler` | `CurrencyFlags` | = 8 |
| `CurrencyNoLowLevelDrop` | `CurrencyFlags` | = 16 |
| `CurrencyIgnoreMaxQtyOnLoad` | `CurrencyFlags` | = 32 |
| `CurrencyLogOnWorldChange` | `CurrencyFlags` | = 64 |
| `CurrencyTrackQuantity` | `CurrencyFlags` | = 128 |
| `CurrencyResetTrackedQuantity` | `CurrencyFlags` | = 256 |
| `CurrencyUpdateVersionIgnoreMax` | `CurrencyFlags` | = 512 |
| `CurrencySuppressChatMessageOnVersionChange` | `CurrencyFlags` | = 1024 |
| `CurrencySingleDropInLoot` | `CurrencyFlags` | = 2048 |
| `CurrencyHasWeeklyCatchup` | `CurrencyFlags` | = 4096 |
| `CurrencyDoNotCompressChat` | `CurrencyFlags` | = 8192 |
| `CurrencyDoNotLogAcquisitionToBi` | `CurrencyFlags` | = 16384 |
| `CurrencyNoRaidDrop` | `CurrencyFlags` | = 32768 |
| `CurrencyNotPersistent` | `CurrencyFlags` | = 65536 |
| `CurrencyDeprecated` | `CurrencyFlags` | = 131072 |
| `CurrencyDynamicMaximum` | `CurrencyFlags` | = 262144 |
| `CurrencySuppressChatMessages` | `CurrencyFlags` | = 524288 |
| `CurrencyDoNotToast` | `CurrencyFlags` | = 1048576 |
| `CurrencyDestroyExtraOnLoot` | `CurrencyFlags` | = 2097152 |
| `CurrencyDontShowTotalInTooltip` | `CurrencyFlags` | = 4194304 |
| `CurrencyDontCoalesceInLootWindow` | `CurrencyFlags` | = 8388608 |
| `CurrencyAccountWide` | `CurrencyFlags` | = 16777216 |
| `CurrencyAllowOverflowMailer` | `CurrencyFlags` | = 33554432 |
| `CurrencyHideAsReward` | `CurrencyFlags` | = 67108864 |
| `CurrencyHasWarmodeBonus` | `CurrencyFlags` | = 134217728 |
| `CurrencyIsAllianceOnly` | `CurrencyFlags` | = 268435456 |
| `CurrencyIsHordeOnly` | `CurrencyFlags` | = 536870912 |
| `CurrencyLimitWarmodeBonusOncePerTooltip` | `CurrencyFlags` | = 1073741824 |
| `CurrencyUsesLedgerBalance` | `CurrencyFlags` | = 2147483648 |

### CurrencyFlagsB

*Enumeration* · 12 values, 1..2048

Access values as `Enum.CurrencyFlagsB.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CurrencyBUseTotalEarnedForEarned` | `CurrencyFlagsB` | = 1 |
| `CurrencyBShowQuestXPGainInTooltip` | `CurrencyFlagsB` | = 2 |
| `CurrencyBNoNotificationMailOnOfflineProgress` | `CurrencyFlagsB` | = 4 |
| `CurrencyBBattlenetVirtualCurrency` | `CurrencyFlagsB` | = 8 |
| `FutureCurrencyFlag` | `CurrencyFlagsB` | = 16 |
| `CurrencyBDontDisplayIfZero` | `CurrencyFlagsB` | = 32 |
| `CurrencyBScaleMaxQuantityBySeasonWeeks` | `CurrencyFlagsB` | = 64 |
| `CurrencyBScaleMaxQuantityByWeeksSinceStart` | `CurrencyFlagsB` | = 128 |
| `CurrencyBForceMaxQuantityOnConversion` | `CurrencyFlagsB` | = 256 |
| `CurrencyBUnearnableBeforeMaxQuantityStart` | `CurrencyFlagsB` | = 512 |
| `CurrencyBAllowReductionByResourcefulness` | `CurrencyFlagsB` | = 1024 |
| `CurrencyBNoBonusXP` | `CurrencyFlagsB` | = 2048 |

### CurrencyGainFlags

*Enumeration* · 5 values, 0..8

Access values as `Enum.CurrencyGainFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CurrencyGainFlags` | = 0 |
| `BonusAward` | `CurrencyGainFlags` | = 1 |
| `DroppedFromDeath` | `CurrencyGainFlags` | = 2 |
| `FromAccountServer` | `CurrencyGainFlags` | = 4 |
| `Autotracking` | `CurrencyGainFlags` | = 8 |

### CurrencyTokenCategoryFlags

*Enumeration* · 5 values, 1..16

Access values as `Enum.CurrencyTokenCategoryFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FlagSortLast` | `CurrencyTokenCategoryFlags` | = 1 |
| `FlagPlayerItemAssignment` | `CurrencyTokenCategoryFlags` | = 2 |
| `Hidden` | `CurrencyTokenCategoryFlags` | = 4 |
| `Virtual` | `CurrencyTokenCategoryFlags` | = 8 |
| `StartsCollapsed` | `CurrencyTokenCategoryFlags` | = 16 |

### CurrencyWeeksFromStartOption

*Enumeration* · 2 values, 1..2

Access values as `Enum.CurrencyWeeksFromStartOption.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DebugLogging` | `CurrencyWeeksFromStartOption` | = 1 |
| `IgnoreTimeBeforeStart` | `CurrencyWeeksFromStartOption` | = 2 |

### LinkedCurrencyFlags

*Enumeration* · 4 values, 1..8

Access values as `Enum.LinkedCurrencyFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IgnoreAdd` | `LinkedCurrencyFlags` | = 1 |
| `IgnoreSubtract` | `LinkedCurrencyFlags` | = 2 |
| `SuppressChatLog` | `LinkedCurrencyFlags` | = 4 |
| `AddIgnoresMax` | `LinkedCurrencyFlags` | = 8 |

### PlayerCurrencyFlags

*Enumeration* · 2 values, 1..2

Access values as `Enum.PlayerCurrencyFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Incremented` | `PlayerCurrencyFlags` | = 1 |
| `Loading` | `PlayerCurrencyFlags` | = 2 |

### PlayerCurrencyFlagsDbFlags

*Enumeration* · 5 values, 1..16

Access values as `Enum.PlayerCurrencyFlagsDbFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IgnoreMaxQtyOnload` | `PlayerCurrencyFlagsDbFlags` | = 1 |
| `Reuse1` | `PlayerCurrencyFlagsDbFlags` | = 2 |
| `InBackpack` | `PlayerCurrencyFlagsDbFlags` | = 4 |
| `UnusedInUI` | `PlayerCurrencyFlagsDbFlags` | = 8 |
| `Reuse2` | `PlayerCurrencyFlagsDbFlags` | = 16 |

### CurrencyConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `PLAYER_CURRENCY_CLIENT_FLAGS` | `PlayerCurrencyFlagsDbFlags` | = `Enum.PlayerCurrencyFlagsDbFlags.InBackpack + Enum.PlayerCurrencyFlagsDbFlags.UnusedInUI` |
| `MAX_CURRENCY_QUANTITY` | `number` | = `100000000` |
| `CONQUEST_ARENA_AND_BG_META_CURRENCY_ID` | `number` | = `483` |
| `CONQUEST_RATED_BG_META_CURRENCY_ID` | `number` | = `484` |
| `CONQUEST_ASHRAN_META_CURRENCY_ID` | `number` | = `692` |
| `ACCOUNT_WIDE_HONOR_CURRENCY_ID` | `number` | = `1585` |
| `ACCOUNT_WIDE_HONOR_LEVEL_CURRENCY_ID` | `number` | = `1586` |
| `CONQUEST_CURRENCY_ID` | `number` | = `1602` |
| `CONQUEST_POINTS_CURRENCY_ID` | `number` | = `390` |
| `CONQUEST_ARENA_META_CURRENCY_ID` | `number` | = `483` |
| `CONQUEST_BG_META_CURRENCY_ID` | `number` | = `484` |
| `HONOR_CURRENCY_ID` | `number` | = `1792` |
| `CLASSIC_HONOR_CURRENCY_ID` | `number` | = `1901` |
| `ARTIFACT_KNOWLEDGE_CURRENCY_ID` | `number` | = `1171` |
| `WAR_RESOURCES_CURRENCY_ID` | `number` | = `1560` |
| `ECHOES_OF_NYALOTHA_CURRENCY_ID` | `number` | = `1803` |
| `DRAGON_ISLES_SUPPLIES_CURRENCY_ID` | `number` | = `2003` |
| `QUESTIONMARK_INV_ICON` | `number` | = `134400` |
| `PVP_CURRENCY_CONQUEST_ALLIANCE_INV_ICON` | `number` | = `463448` |
| `PVP_CURRENCY_CONQUEST_HORDE_INV_ICON` | `number` | = `463449` |
| `PVP_CURRENCY_HONOR_ALLIANCE_INV_ICON` | `number` | = `463450` |
| `PVP_CURRENCY_HONOR_HORDE_INV_ICON` | `number` | = `463451` |
| `CURRENCY_ID_RENOWN` | `number` | = `1822` |
| `CURRENCY_ID_RENOWN_KYRIAN` | `number` | = `1829` |
| `CURRENCY_ID_RENOWN_VENTHYR` | `number` | = `1830` |
| `CURRENCY_ID_RENOWN_NIGHT_FAE` | `number` | = `1831` |
| `CURRENCY_ID_RENOWN_NECROLORD` | `number` | = `1832` |
| `CURRENCY_ID_WILLING_SOUL` | `number` | = `1810` |
| `CURRENCY_ID_RESERVOIR_ANIMA` | `number` | = `1813` |
| `CURRENCY_ID_PERKS_PROGRAM_DISPLAY_INFO` | `number` | = `2032` |
| `CURRENCY_ID_RENOWN_PVP_RANK` | `number` | = `3473` |
| `CURRENCY_ID_RENOWN_LEGACY` | `number` | = `3485` |
| `IMMEDIATE_CURRENCY_WALLET_ITEM_ID` | `number` | = `276637` |
| `CURRENCY_WALLET_TYPE_WOWMONEY` | `number` | = `0` |
