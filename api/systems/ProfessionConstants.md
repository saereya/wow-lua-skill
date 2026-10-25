# ProfessionConstants

source `interface/addons/blizzard_apidocumentationgenerated/professionconstantsdocumentation.lua` (FileDataID 4637162)

## Types

### CraftingOrderDuration

*Enumeration* · 3 values, 0..2

Access values as `Enum.CraftingOrderDuration.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Short` | `CraftingOrderDuration` | = 0 |
| `Medium` | `CraftingOrderDuration` | = 1 |
| `Long` | `CraftingOrderDuration` | = 2 |

### CraftingOrderFlags

*Enumeration* · 6 values, 0..16

Access values as `Enum.CraftingOrderFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CraftingOrderFlags` | = 0 |
| `IsRecraft` | `CraftingOrderFlags` | = 1 |
| `HasNoneReagents` | `CraftingOrderFlags` | = 2 |
| `HasSomeReagents` | `CraftingOrderFlags` | = 4 |
| `HasAllReagents` | `CraftingOrderFlags` | = 8 |
| `IsFulfillable` | `CraftingOrderFlags` | = 16 |

### CraftingOrderItemFlags

*Enumeration* · 3 values, 0..2

Access values as `Enum.CraftingOrderItemFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CraftingOrderItemFlags` | = 0 |
| `NpcProvided` | `CraftingOrderItemFlags` | = 1 |
| `HasEnchantmentData` | `CraftingOrderItemFlags` | = 2 |

### CraftingOrderItemType

*Enumeration* · 6 values, 0..5

Access values as `Enum.CraftingOrderItemType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `CraftingOrderItemType` | = 0 |
| `Recraft` | `CraftingOrderItemType` | = 1 |
| `CraftedResult` | `CraftingOrderItemType` | = 2 |
| `RemoveReagent` | `CraftingOrderItemType` | = 3 |
| `Deprecated` | `CraftingOrderItemType` | = 4 |
| `Currency` | `CraftingOrderItemType` | = 5 |

### CraftingOrderReagentSource

*Enumeration* · 4 values, 0..3

Access values as `Enum.CraftingOrderReagentSource.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Any` | `CraftingOrderReagentSource` | = 0 |
| `Customer` | `CraftingOrderReagentSource` | = 1 |
| `Crafter` | `CraftingOrderReagentSource` | = 2 |
| `None` | `CraftingOrderReagentSource` | = 3 |

### CraftingOrderResult

*Enumeration* · 49 values, 0..48

Access values as `Enum.CraftingOrderResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `CraftingOrderResult` | = 0 |
| `Aborted` | `CraftingOrderResult` | = 1 |
| `AlreadyClaimed` | `CraftingOrderResult` | = 2 |
| `AlreadyCrafted` | `CraftingOrderResult` | = 3 |
| `CannotBeOrdered` | `CraftingOrderResult` | = 4 |
| `CannotCancel` | `CraftingOrderResult` | = 5 |
| `CannotClaim` | `CraftingOrderResult` | = 6 |
| `CannotClaimOwnOrder` | `CraftingOrderResult` | = 7 |
| `CannotCraft` | `CraftingOrderResult` | = 8 |
| `CannotCreate` | `CraftingOrderResult` | = 9 |
| `CannotFulfill` | `CraftingOrderResult` | = 10 |
| `CannotRecraft` | `CraftingOrderResult` | = 11 |
| `CannotReject` | `CraftingOrderResult` | = 12 |
| `CannotRelease` | `CraftingOrderResult` | = 13 |
| `CrafterIsIgnored` | `CraftingOrderResult` | = 14 |
| `DatabaseError` | `CraftingOrderResult` | = 15 |
| `Expired` | `CraftingOrderResult` | = 16 |
| `Locked` | `CraftingOrderResult` | = 17 |
| `InvalidDuration` | `CraftingOrderResult` | = 18 |
| `InvalidMinQuality` | `CraftingOrderResult` | = 19 |
| `InvalidNotes` | `CraftingOrderResult` | = 20 |
| `InvalidReagent` | `CraftingOrderResult` | = 21 |
| `InvalidRealm` | `CraftingOrderResult` | = 22 |
| `InvalidRecipe` | `CraftingOrderResult` | = 23 |
| `InvalidRecraftItem` | `CraftingOrderResult` | = 24 |
| `InvalidSort` | `CraftingOrderResult` | = 25 |
| `InvalidTarget` | `CraftingOrderResult` | = 26 |
| `InvalidType` | `CraftingOrderResult` | = 27 |
| `MaxOrdersReached` | `CraftingOrderResult` | = 28 |
| `MissingCraftingTable` | `CraftingOrderResult` | = 29 |
| `MissingCurrency` | `CraftingOrderResult` | = 30 |
| `MissingItem` | `CraftingOrderResult` | = 31 |
| `MissingNpc` | `CraftingOrderResult` | = 32 |
| `MissingOrder` | `CraftingOrderResult` | = 33 |
| `MissingRecraftItem` | `CraftingOrderResult` | = 34 |
| `NoAccountItems` | `CraftingOrderResult` | = 35 |
| `NotClaimed` | `CraftingOrderResult` | = 36 |
| `NotCrafted` | `CraftingOrderResult` | = 37 |
| `NotInGuild` | `CraftingOrderResult` | = 38 |
| `NotYetImplemented` | `CraftingOrderResult` | = 39 |
| `OutOfPublicOrderCapacity` | `CraftingOrderResult` | = 40 |
| `ServerIsNotAvailable` | `CraftingOrderResult` | = 41 |
| `ThrottleViolation` | `CraftingOrderResult` | = 42 |
| `TargetCannotCraft` | `CraftingOrderResult` | = 43 |
| `TargetLocked` | `CraftingOrderResult` | = 44 |
| `Timeout` | `CraftingOrderResult` | = 45 |
| `TooManyCurrencies` | `CraftingOrderResult` | = 46 |
| `TooManyItems` | `CraftingOrderResult` | = 47 |
| `WrongVersion` | `CraftingOrderResult` | = 48 |

### CraftingOrderSortType

*Enumeration* · 8 values, 0..7

Access values as `Enum.CraftingOrderSortType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ItemName` | `CraftingOrderSortType` | = 0 |
| `AveTip` | `CraftingOrderSortType` | = 1 |
| `MaxTip` | `CraftingOrderSortType` | = 2 |
| `Quantity` | `CraftingOrderSortType` | = 3 |
| `Reagents` | `CraftingOrderSortType` | = 4 |
| `Tip` | `CraftingOrderSortType` | = 5 |
| `TimeRemaining` | `CraftingOrderSortType` | = 6 |
| `Status` | `CraftingOrderSortType` | = 7 |

### CraftingOrderState

*Enumeration* · 16 values, 0..15

Access values as `Enum.CraftingOrderState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CraftingOrderState` | = 0 |
| `Creating` | `CraftingOrderState` | = 1 |
| `Created` | `CraftingOrderState` | = 2 |
| `Claiming` | `CraftingOrderState` | = 3 |
| `Claimed` | `CraftingOrderState` | = 4 |
| `Rejecting` | `CraftingOrderState` | = 5 |
| `Rejected` | `CraftingOrderState` | = 6 |
| `Releasing` | `CraftingOrderState` | = 7 |
| `Crafting` | `CraftingOrderState` | = 8 |
| `Recrafting` | `CraftingOrderState` | = 9 |
| `Fulfilling` | `CraftingOrderState` | = 10 |
| `Fulfilled` | `CraftingOrderState` | = 11 |
| `Canceling` | `CraftingOrderState` | = 12 |
| `Canceled` | `CraftingOrderState` | = 13 |
| `Expiring` | `CraftingOrderState` | = 14 |
| `Expired` | `CraftingOrderState` | = 15 |

### CraftingOrderType

*Enumeration* · 4 values, 0..3

Access values as `Enum.CraftingOrderType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Public` | `CraftingOrderType` | = 0 |
| `Guild` | `CraftingOrderType` | = 1 |
| `Personal` | `CraftingOrderType` | = 2 |
| `Npc` | `CraftingOrderType` | = 3 |

### CraftingReagentType

*Enumeration* · 4 values, 0..3

Access values as `Enum.CraftingReagentType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Modifying` | `CraftingReagentType` | = 0 |
| `Basic` | `CraftingReagentType` | = 1 |
| `Finishing` | `CraftingReagentType` | = 2 |
| `Automatic` | `CraftingReagentType` | = 3 |

### ItemRecraftFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.ItemRecraftFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `ItemRecraftFlags` | = 1 |

### NpcCraftingOrderSetFlags

*Enumeration* · 2 values, 1..2

Access values as `Enum.NpcCraftingOrderSetFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AllowMultiple` | `NpcCraftingOrderSetFlags` | = 1 |
| `AllowDuplicate` | `NpcCraftingOrderSetFlags` | = 2 |

### Profession

*Enumeration* · 15 values, 0..14

Access values as `Enum.Profession.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `FirstAid` | `Profession` | = 0 |
| `Blacksmithing` | `Profession` | = 1 |
| `Leatherworking` | `Profession` | = 2 |
| `Alchemy` | `Profession` | = 3 |
| `Herbalism` | `Profession` | = 4 |
| `Cooking` | `Profession` | = 5 |
| `Mining` | `Profession` | = 6 |
| `Tailoring` | `Profession` | = 7 |
| `Engineering` | `Profession` | = 8 |
| `Enchanting` | `Profession` | = 9 |
| `Fishing` | `Profession` | = 10 |
| `Skinning` | `Profession` | = 11 |
| `Jewelcrafting` | `Profession` | = 12 |
| `Inscription` | `Profession` | = 13 |
| `Archaeology` | `Profession` | = 14 |

### ProfessionActionType

*Enumeration* · 2 values, 0..1

Access values as `Enum.ProfessionActionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Craft` | `ProfessionActionType` | = 0 |
| `Gather` | `ProfessionActionType` | = 1 |

### ProfessionEffect

*Enumeration* · 31 values, 0..30

Access values as `Enum.ProfessionEffect.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Skill` | `ProfessionEffect` | = 0 |
| `StatInspiration` | `ProfessionEffect` | = 1 |
| `StatResourcefulness` | `ProfessionEffect` | = 2 |
| `StatFinesse` | `ProfessionEffect` | = 3 |
| `StatDeftness` | `ProfessionEffect` | = 4 |
| `StatPerception` | `ProfessionEffect` | = 5 |
| `StatCraftingSpeed` | `ProfessionEffect` | = 6 |
| `StatMulticraft` | `ProfessionEffect` | = 7 |
| `UnlockReagentSlot` | `ProfessionEffect` | = 8 |
| `ModInspiration` | `ProfessionEffect` | = 9 |
| `ModResourcefulness` | `ProfessionEffect` | = 10 |
| `ModFinesse` | `ProfessionEffect` | = 11 |
| `ModDeftness` | `ProfessionEffect` | = 12 |
| `ModPerception` | `ProfessionEffect` | = 13 |
| `ModCraftingSpeed` | `ProfessionEffect` | = 14 |
| `ModMulticraft` | `ProfessionEffect` | = 15 |
| `ModUnused_1` | `ProfessionEffect` | = 16 |
| `ModUnused_2` | `ProfessionEffect` | = 17 |
| `ModCraftExtraQuantity` | `ProfessionEffect` | = 18 |
| `ModGatherExtraQuantity` | `ProfessionEffect` | = 19 |
| `ModCraftCritSize` | `ProfessionEffect` | = 20 |
| `ModCraftReductionQuantity` | `ProfessionEffect` | = 21 |
| `DecreaseDifficulty` | `ProfessionEffect` | = 22 |
| `IncreaseDifficulty` | `ProfessionEffect` | = 23 |
| `ModSkillGain` | `ProfessionEffect` | = 24 |
| `AccumulateRanksByLabel` | `ProfessionEffect` | = 25 |
| `StatIngenuity` | `ProfessionEffect` | = 26 |
| `ModConcentration` | `ProfessionEffect` | = 27 |
| `Tokenizer` | `ProfessionEffect` | = 28 |
| `ModIngenuity` | `ProfessionEffect` | = 29 |
| `ConcentrationRefund` | `ProfessionEffect` | = 30 |

### ProfessionRating

*Enumeration* · 9 values, 0..8

Access values as `Enum.ProfessionRating.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Inspiration` | `ProfessionRating` | = 0 |
| `Resourcefulness` | `ProfessionRating` | = 1 |
| `Finesse` | `ProfessionRating` | = 2 |
| `Deftness` | `ProfessionRating` | = 3 |
| `Perception` | `ProfessionRating` | = 4 |
| `CraftingSpeed` | `ProfessionRating` | = 5 |
| `Multicraft` | `ProfessionRating` | = 6 |
| `Ingenuity` | `ProfessionRating` | = 7 |
| `Unused_2` | `ProfessionRating` | = 8 |

### ProfessionRatingType

*Enumeration* · 2 values, 0..1

Access values as `Enum.ProfessionRatingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Craft` | `ProfessionRatingType` | = 0 |
| `Gather` | `ProfessionRatingType` | = 1 |

### RcoCloseReason

*Enumeration* · 7 values, 0..6

Access values as `Enum.RcoCloseReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Fulfill` | `RcoCloseReason` | = 0 |
| `Expire` | `RcoCloseReason` | = 1 |
| `Cancel` | `RcoCloseReason` | = 2 |
| `Reject` | `RcoCloseReason` | = 3 |
| `GmCancel` | `RcoCloseReason` | = 4 |
| `CrafterFulfill` | `RcoCloseReason` | = 5 |
| `Invalid` | `RcoCloseReason` | = 6 |

### SkinningState

*Enumeration* · 5 values, 0..4

Access values as `Enum.SkinningState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `SkinningState` | = 0 |
| `Reserved` | `SkinningState` | = 1 |
| `Skinning` | `SkinningState` | = 2 |
| `Looting` | `SkinningState` | = 3 |
| `Skinned` | `SkinningState` | = 4 |

### ProfessionConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `NUM_PRIMARY_PROFESSIONS` | `number` | = `2` |
| `CLASSIC_PROFESSION_PARENT_TIER_INDEX` | `number` | = `4` |
| `RUNEFORGING_SKILL_LINE_ID` | `number` | = `960` |
| `RUNEFORGING_ROOT_CATEGORY_ID` | `number` | = `210` |
| `MAX_CRAFTING_REAGENT_SLOTS` | `number` | = `12` |
| `CRAFTING_ORDER_CLAIM_DURATION` | `number` | = `0` |
| `PUBLIC_CRAFTING_ORDER_STALE_THRESHOLD` | `number` | = `0` |
| `CRAFTING_ORDER_ITEM_RETENTION` | `number` | = `30` |
| `CRAFTING_ORDER_CURRENCY_WALLET_ITEM_ID` | `number` | = `262724` |
