# TransmogOutfitConstants

source `interface/addons/blizzard_apidocumentationgenerated/transmogoutfitconstantsdocumentation.lua` (FileDataID 7240887)

## Types

### TransmogOutfitCostModifiersApplied

*Enumeration* · 4 values, 1..8

Access values as `Enum.TransmogOutfitCostModifiersApplied.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DebugOnlyFreeDiscountApplied` | `TransmogOutfitCostModifiersApplied` | = 1 |
| `VoidRacialDiscountApplied` | `TransmogOutfitCostModifiersApplied` | = 2 |
| `OutfitCostModifierApplied` | `TransmogOutfitCostModifiersApplied` | = 4 |
| `AuraDiscountApplied` | `TransmogOutfitCostModifiersApplied` | = 8 |

### TransmogOutfitDataFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.TransmogOutfitDataFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsCachedLocally` | `TransmogOutfitDataFlags` | = 1 |

### TransmogOutfitDisplayType

*Enumeration* · 5 values, 0..4

Access values as `Enum.TransmogOutfitDisplayType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unassigned` | `TransmogOutfitDisplayType` | = 0 |
| `Assigned` | `TransmogOutfitDisplayType` | = 1 |
| `Equipped` | `TransmogOutfitDisplayType` | = 2 |
| `Hidden` | `TransmogOutfitDisplayType` | = 3 |
| `Disabled` | `TransmogOutfitDisplayType` | = 4 |

### TransmogOutfitEntryFlags

*Enumeration* · 6 values, 1..32

Access values as `Enum.TransmogOutfitEntryFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AutomaticallyAwardedOnLogin` | `TransmogOutfitEntryFlags` | = 1 |
| `UseOverrideName` | `TransmogOutfitEntryFlags` | = 2 |
| `OnlyAvailableDuringEvent` | `TransmogOutfitEntryFlags` | = 4 |
| `SortedToTopOfList` | `TransmogOutfitEntryFlags` | = 8 |
| `UseOverrideCostModifier` | `TransmogOutfitEntryFlags` | = 16 |
| `IsDefaultEquipped` | `TransmogOutfitEntryFlags` | = 32 |

### TransmogOutfitEntrySource

*Enumeration* · 3 values, 0..2

Access values as `Enum.TransmogOutfitEntrySource.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `StampedSource` | `TransmogOutfitEntrySource` | = 0 |
| `AutomaticallyAwarded` | `TransmogOutfitEntrySource` | = 1 |
| `PlayerPurchased` | `TransmogOutfitEntrySource` | = 2 |

### TransmogOutfitEquipAction

*Enumeration* · 6 values, 0..5

Access values as `Enum.TransmogOutfitEquipAction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Equip` | `TransmogOutfitEquipAction` | = 0 |
| `EquipAndLock` | `TransmogOutfitEquipAction` | = 1 |
| `Remove` | `TransmogOutfitEquipAction` | = 2 |
| `RemoveAndLock` | `TransmogOutfitEquipAction` | = 3 |
| `Unlock` | `TransmogOutfitEquipAction` | = 4 |
| `Lock` | `TransmogOutfitEquipAction` | = 5 |

### TransmogOutfitSetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.TransmogOutfitSetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Equipped` | `TransmogOutfitSetType` | = 0 |
| `Outfit` | `TransmogOutfitSetType` | = 1 |
| `CustomSet` | `TransmogOutfitSetType` | = 2 |

### TransmogOutfitSlot

*Enumeration* · 15 values, 0..14

Access values as `Enum.TransmogOutfitSlot.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Head` | `TransmogOutfitSlot` | = 0 |
| `ShoulderRight` | `TransmogOutfitSlot` | = 1 |
| `ShoulderLeft` | `TransmogOutfitSlot` | = 2 |
| `Back` | `TransmogOutfitSlot` | = 3 |
| `Chest` | `TransmogOutfitSlot` | = 4 |
| `Tabard` | `TransmogOutfitSlot` | = 5 |
| `Body` | `TransmogOutfitSlot` | = 6 |
| `Wrist` | `TransmogOutfitSlot` | = 7 |
| `Hand` | `TransmogOutfitSlot` | = 8 |
| `Waist` | `TransmogOutfitSlot` | = 9 |
| `Legs` | `TransmogOutfitSlot` | = 10 |
| `Feet` | `TransmogOutfitSlot` | = 11 |
| `WeaponMainHand` | `TransmogOutfitSlot` | = 12 |
| `WeaponOffHand` | `TransmogOutfitSlot` | = 13 |
| `WeaponRanged` | `TransmogOutfitSlot` | = 14 |

### TransmogOutfitSlotError

*Enumeration* · 15 values, 0..14

Access values as `Enum.TransmogOutfitSlotError.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `TransmogOutfitSlotError` | = 0 |
| `NoItem` | `TransmogOutfitSlotError` | = 1 |
| `NotSoulbound` | `TransmogOutfitSlotError` | = 2 |
| `Legendary` | `TransmogOutfitSlotError` | = 3 |
| `InvalidItemType` | `TransmogOutfitSlotError` | = 4 |
| `InvalidDestination` | `TransmogOutfitSlotError` | = 5 |
| `Mismatch` | `TransmogOutfitSlotError` | = 6 |
| `SameItem` | `TransmogOutfitSlotError` | = 7 |
| `InvalidSource` | `TransmogOutfitSlotError` | = 8 |
| `InvalidSourceQuality` | `TransmogOutfitSlotError` | = 9 |
| `CannotUseItem` | `TransmogOutfitSlotError` | = 10 |
| `InvalidSlotForRace` | `TransmogOutfitSlotError` | = 11 |
| `NoIllusion` | `TransmogOutfitSlotError` | = 12 |
| `InvalidSlotForForm` | `TransmogOutfitSlotError` | = 13 |
| `IncompatibleWithMainHand` | `TransmogOutfitSlotError` | = 14 |

### TransmogOutfitSlotFlags

*Enumeration* · 3 values, 1..4

Access values as `Enum.TransmogOutfitSlotFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CannotBeHidden` | `TransmogOutfitSlotFlags` | = 1 |
| `CanHaveIllusions` | `TransmogOutfitSlotFlags` | = 2 |
| `IsSecondarySlot` | `TransmogOutfitSlotFlags` | = 4 |

### TransmogOutfitSlotOption

*Enumeration* · 16 values, 0..15

Access values as `Enum.TransmogOutfitSlotOption.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TransmogOutfitSlotOption` | = 0 |
| `OneHandedWeapon` | `TransmogOutfitSlotOption` | = 1 |
| `TwoHandedWeapon` | `TransmogOutfitSlotOption` | = 2 |
| `RangedWeapon` | `TransmogOutfitSlotOption` | = 3 |
| `OffHand` | `TransmogOutfitSlotOption` | = 4 |
| `Shield` | `TransmogOutfitSlotOption` | = 5 |
| `DeprecatedReuseMe` | `TransmogOutfitSlotOption` | = 6 |
| `FuryTwoHandedWeapon` | `TransmogOutfitSlotOption` | = 7 |
| `ArtifactSpecOne` | `TransmogOutfitSlotOption` | = 8 |
| `ArtifactSpecTwo` | `TransmogOutfitSlotOption` | = 9 |
| `ArtifactSpecThree` | `TransmogOutfitSlotOption` | = 10 |
| `ArtifactSpecFour` | `TransmogOutfitSlotOption` | = 11 |
| `ArmorCloth` | `TransmogOutfitSlotOption` | = 12 |
| `ArmorLeather` | `TransmogOutfitSlotOption` | = 13 |
| `ArmorMail` | `TransmogOutfitSlotOption` | = 14 |
| `ArmorPlate` | `TransmogOutfitSlotOption` | = 15 |

### TransmogOutfitSlotOptionFlags

*Enumeration* · 3 values, 1..4

Access values as `Enum.TransmogOutfitSlotOptionFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IllusionNotAllowed` | `TransmogOutfitSlotOptionFlags` | = 1 |
| `DynamicOptionName` | `TransmogOutfitSlotOptionFlags` | = 2 |
| `DisablesOffhandSlot` | `TransmogOutfitSlotOptionFlags` | = 4 |

### TransmogOutfitSlotOptionSheatheCategory

*Enumeration* · 4 values, 0..3

Access values as `Enum.TransmogOutfitSlotOptionSheatheCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `TransmogOutfitSlotOptionSheatheCategory` | = 0 |
| `Back` | `TransmogOutfitSlotOptionSheatheCategory` | = 1 |
| `Side` | `TransmogOutfitSlotOptionSheatheCategory` | = 2 |
| `Hide` | `TransmogOutfitSlotOptionSheatheCategory` | = 3 |

### TransmogOutfitSlotPosition

*Enumeration* · 3 values, 0..2

Access values as `Enum.TransmogOutfitSlotPosition.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Left` | `TransmogOutfitSlotPosition` | = 0 |
| `Right` | `TransmogOutfitSlotPosition` | = 1 |
| `Bottom` | `TransmogOutfitSlotPosition` | = 2 |

### TransmogOutfitSlotSaveFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.TransmogOutfitSlotSaveFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AppearanceIsNotValid` | `TransmogOutfitSlotSaveFlags` | = 1 |

### TransmogOutfitSlotWarning

*Enumeration* · 8 values, 0..7

Access values as `Enum.TransmogOutfitSlotWarning.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ok` | `TransmogOutfitSlotWarning` | = 0 |
| `InvalidEquippedDestinationItem` | `TransmogOutfitSlotWarning` | = 1 |
| `WrongWeaponCategoryEquipped` | `TransmogOutfitSlotWarning` | = 2 |
| `WrongArmorTypeEquipped` | `TransmogOutfitSlotWarning` | = 3 |
| `EquippedItemLowLevel` | `TransmogOutfitSlotWarning` | = 4 |
| `PendingWeaponChanges` | `TransmogOutfitSlotWarning` | = 5 |
| `WeaponDoesNotSupportIllusions` | `TransmogOutfitSlotWarning` | = 6 |
| `NothingEquipped` | `TransmogOutfitSlotWarning` | = 7 |

### TransmogOutfitTransactionFlags

*Enumeration* · 10 values, 1..28

Access values as `Enum.TransmogOutfitTransactionFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UpdateMetadata` | `TransmogOutfitTransactionFlags` | = 1 |
| `UpdateOutfitInfo` | `TransmogOutfitTransactionFlags` | = 2 |
| `CreateOutfitInfo` | `TransmogOutfitTransactionFlags` | = 4 |
| `UpdateSlots` | `TransmogOutfitTransactionFlags` | = 8 |
| `UpdateSituations` | `TransmogOutfitTransactionFlags` | = 16 |
| `AddNewOutfitMask` | `TransmogOutfitTransactionFlags` | = 20 |
| `UpdateSituationsMask` | `TransmogOutfitTransactionFlags` | = 18 |
| `AddOutfitAndUpdateSlots` | `TransmogOutfitTransactionFlags` | = 28 |
| `FullOutfitUpdateMask` | `TransmogOutfitTransactionFlags` | = 27 |
| `CreateAndUpdateOutfitInfoMask` | `TransmogOutfitTransactionFlags` | = 6 |

### TransmogOutfitTransactionType

*Enumeration* · 5 values, 0..4

Access values as `Enum.TransmogOutfitTransactionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `UpdateMetadata` | `TransmogOutfitTransactionType` | = 0 |
| `UpdateOutfitInfo` | `TransmogOutfitTransactionType` | = 1 |
| `CreateOutfitInfo` | `TransmogOutfitTransactionType` | = 2 |
| `UpdateSlots` | `TransmogOutfitTransactionType` | = 3 |
| `UpdateSituations` | `TransmogOutfitTransactionType` | = 4 |

### TransmogSettingsUpdateType

*Enumeration* · 2 values, 0..1

Access values as `Enum.TransmogSettingsUpdateType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TransmogSettingsUpdateType` | = 0 |
| `OptOut` | `TransmogSettingsUpdateType` | = 1 |

### TransmogSituation

*Enumeration* · 32 values, 0..31

Access values as `Enum.TransmogSituation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AllSpecs` | `TransmogSituation` | = 0 |
| `Spec` | `TransmogSituation` | = 1 |
| `AllLocations` | `TransmogSituation` | = 2 |
| `LocationRested` | `TransmogSituation` | = 3 |
| `LocationHouse` | `TransmogSituation` | = 4 |
| `LocationCharacterSelect` | `TransmogSituation` | = 5 |
| `LocationWorld` | `TransmogSituation` | = 6 |
| `LocationDelves` | `TransmogSituation` | = 7 |
| `LocationDungeons` | `TransmogSituation` | = 8 |
| `LocationRaids` | `TransmogSituation` | = 9 |
| `LocationArenas` | `TransmogSituation` | = 10 |
| `LocationBattlegrounds` | `TransmogSituation` | = 11 |
| `AllMovement` | `TransmogSituation` | = 12 |
| `MovementUnmounted` | `TransmogSituation` | = 13 |
| `MovementSwimming` | `TransmogSituation` | = 14 |
| `MovementGroundMount` | `TransmogSituation` | = 15 |
| `MovementFlyingMount` | `TransmogSituation` | = 16 |
| `AllEquipmentSets` | `TransmogSituation` | = 17 |
| `EquipmentSets` | `TransmogSituation` | = 18 |
| `AllRacialForms` | `TransmogSituation` | = 19 |
| `FormNative` | `TransmogSituation` | = 20 |
| `FormNonNative` | `TransmogSituation` | = 21 |
| `AllWeather` | `TransmogSituation` | = 22 |
| `WeatherClear` | `TransmogSituation` | = 23 |
| `WeatherRain` | `TransmogSituation` | = 24 |
| `WeatherSnow` | `TransmogSituation` | = 25 |
| `WeatherSand` | `TransmogSituation` | = 26 |
| `AllTime` | `TransmogSituation` | = 27 |
| `TimeMorning` | `TransmogSituation` | = 28 |
| `TimeDay` | `TransmogSituation` | = 29 |
| `TimeEvening` | `TransmogSituation` | = 30 |
| `TimeNight` | `TransmogSituation` | = 31 |

### TransmogSituationFlags

*Enumeration* · 7 values, 1..64

Access values as `Enum.TransmogSituationFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsPlayerFacing` | `TransmogSituationFlags` | = 1 |
| `SpecUseTalentLoadout` | `TransmogSituationFlags` | = 2 |
| `AllSituation` | `TransmogSituationFlags` | = 4 |
| `DefaultsToOn` | `TransmogSituationFlags` | = 8 |
| `DynamicallyNamed` | `TransmogSituationFlags` | = 16 |
| `NoneSituation` | `TransmogSituationFlags` | = 32 |
| `DisabledSituation` | `TransmogSituationFlags` | = 64 |

### TransmogSituationGroupFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.TransmogSituationGroupFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DynamicallyCreatesGroups` | `TransmogSituationGroupFlags` | = 1 |

### TransmogSituationTrigger

*Enumeration* · 12 values, 0..11

Access values as `Enum.TransmogSituationTrigger.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TransmogSituationTrigger` | = 0 |
| `Manual` | `TransmogSituationTrigger` | = 1 |
| `TransmogUpdate` | `TransmogSituationTrigger` | = 2 |
| `Location` | `TransmogSituationTrigger` | = 3 |
| `Movement` | `TransmogSituationTrigger` | = 4 |
| `Specialization` | `TransmogSituationTrigger` | = 5 |
| `EquipmentSet` | `TransmogSituationTrigger` | = 6 |
| `Forms` | `TransmogSituationTrigger` | = 7 |
| `EventOutfit` | `TransmogSituationTrigger` | = 8 |
| `Weather` | `TransmogSituationTrigger` | = 9 |
| `TimeOfDay` | `TransmogSituationTrigger` | = 10 |
| `SettingsUpdate` | `TransmogSituationTrigger` | = 11 |

### TransmogSituationTriggerFlags

*Enumeration* · 5 values, 1..16

Access values as `Enum.TransmogSituationTriggerFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CanLockOutfit` | `TransmogSituationTriggerFlags` | = 1 |
| `CanChangeLockedOutfit` | `TransmogSituationTriggerFlags` | = 2 |
| `IsPlayerFacing` | `TransmogSituationTriggerFlags` | = 4 |
| `SituationsAreExclusive` | `TransmogSituationTriggerFlags` | = 8 |
| `DisabledTrigger` | `TransmogSituationTriggerFlags` | = 16 |

### TransmogSituationTriggerType

*Enumeration* · 4 values, 0..3

Access values as `Enum.TransmogSituationTriggerType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TransmogSituationTriggerType` | = 0 |
| `Manual` | `TransmogSituationTriggerType` | = 1 |
| `Automatic` | `TransmogSituationTriggerType` | = 2 |
| `TransmogUpdate` | `TransmogSituationTriggerType` | = 3 |

### TransmogTimeOfDayCategory

*Enumeration* · 4 values, 0..3

Access values as `Enum.TransmogTimeOfDayCategory.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Morning` | `TransmogTimeOfDayCategory` | = 0 |
| `Midday` | `TransmogTimeOfDayCategory` | = 1 |
| `Evening` | `TransmogTimeOfDayCategory` | = 2 |
| `Night` | `TransmogTimeOfDayCategory` | = 3 |

### TransmogOutfitDataConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `EQUIP_TRANSMOG_OUTFIT_MANUAL_SPELL_ID` | `number` | = `1247613` |
| `CLEAR_TRANSMOG_OUTFIT_MANUAL_SPELL_ID` | `number` | = `1247917` |
| `TRANSMOG_OUTFIT_SLOT_NONE` | `TransmogOutfitSlot` | = `-1` |
