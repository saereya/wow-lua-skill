# BagConstants

source `interface/addons/blizzard_apidocumentationgenerated/bagconstantsdocumentation.lua` (FileDataID 4637035)

## Types

### BagFlag

*Enumeration* · 27 values, 1..134217728

Access values as `Enum.BagFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DontFindStack` | `BagFlag` | = 1 |
| `AlreadyOwner` | `BagFlag` | = 2 |
| `AlreadyBound` | `BagFlag` | = 4 |
| `Swap` | `BagFlag` | = 8 |
| `BagIsEmpty` | `BagFlag` | = 16 |
| `LookInInventory` | `BagFlag` | = 32 |
| `IgnoreBoundItemCheck` | `BagFlag` | = 64 |
| `StackOnly` | `BagFlag` | = 128 |
| `RecurseQuivers` | `BagFlag` | = 256 |
| `IgnoreBankcheck` | `BagFlag` | = 512 |
| `AllowBagsInNonBagSlots` | `BagFlag` | = 1024 |
| `PreferQuivers` | `BagFlag` | = 2048 |
| `SwapBags` | `BagFlag` | = 4096 |
| `IgnoreExisting` | `BagFlag` | = 8192 |
| `AllowPartialStack` | `BagFlag` | = 16384 |
| `LookInCharacterBankOnly` | `BagFlag` | = 32768 |
| `AllowBuyback` | `BagFlag` | = 65536 |
| `IgnorePetBankcheck` | `BagFlag` | = 131072 |
| `PreferPriorityBags` | `BagFlag` | = 262144 |
| `PreferNeutralPriorityBags` | `BagFlag` | = 524288 |
| `AsymmetricSwap` | `BagFlag` | = 1048576 |
| `PreferReagentBags` | `BagFlag` | = 2097152 |
| `IgnoreReagentBags` | `BagFlag` | = 8388608 |
| `LookInAccountBankOnly` | `BagFlag` | = 16777216 |
| `HasRefund` | `BagFlag` | = 33554432 |
| `SkipValidCountCheck` | `BagFlag` | = 67108864 |
| `AllowSoulboundItemInAccountBank` | `BagFlag` | = 134217728 |

### BagSlotFlags

*Enumeration* · 10 values, 1..512

Access values as `Enum.BagSlotFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DisableAutoSort` | `BagSlotFlags` | = 1 |
| `ClassEquipment` | `BagSlotFlags` | = 2 |
| `ClassConsumables` | `BagSlotFlags` | = 4 |
| `ClassProfessionGoods` | `BagSlotFlags` | = 8 |
| `ClassJunk` | `BagSlotFlags` | = 16 |
| `ClassQuestItems` | `BagSlotFlags` | = 32 |
| `ExcludeJunkSell` | `BagSlotFlags` | = 64 |
| `ClassReagents` | `BagSlotFlags` | = 128 |
| `ExpansionCurrent` | `BagSlotFlags` | = 256 |
| `ExpansionLegacy` | `BagSlotFlags` | = 512 |
