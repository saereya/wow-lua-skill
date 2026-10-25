# TraitConstants

source `interface/addons/blizzard_apidocumentationgenerated/traitconstantsdocumentation.lua` (FileDataID 4637263)

## Types

### NodeOpFailureReason

*Enumeration* · 27 values, 0..26

Access values as `Enum.NodeOpFailureReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `NodeOpFailureReason` | = 0 |
| `MissingEdgeConnection` | `NodeOpFailureReason` | = 1 |
| `RequiredForEdge` | `NodeOpFailureReason` | = 2 |
| `MissingRequiredEdge` | `NodeOpFailureReason` | = 3 |
| `HasMutuallyExclusiveEdge` | `NodeOpFailureReason` | = 4 |
| `NotEnoughSourcedCurrencySpent` | `NodeOpFailureReason` | = 5 |
| `NotEnoughCurrencySpent` | `NodeOpFailureReason` | = 6 |
| `NotEnoughGoldSpent` | `NodeOpFailureReason` | = 7 |
| `MissingAchievement` | `NodeOpFailureReason` | = 8 |
| `MissingQuest` | `NodeOpFailureReason` | = 9 |
| `WrongSpec` | `NodeOpFailureReason` | = 10 |
| `WrongSelection` | `NodeOpFailureReason` | = 11 |
| `MaxRank` | `NodeOpFailureReason` | = 12 |
| `DataError` | `NodeOpFailureReason` | = 13 |
| `NotEnoughSourcedCurrency` | `NodeOpFailureReason` | = 14 |
| `NotEnoughCurrency` | `NodeOpFailureReason` | = 15 |
| `NotEnoughGold` | `NodeOpFailureReason` | = 16 |
| `SameSelection` | `NodeOpFailureReason` | = 17 |
| `NodeNotFound` | `NodeOpFailureReason` | = 18 |
| `EntryNotFound` | `NodeOpFailureReason` | = 19 |
| `RequiredForCondition` | `NodeOpFailureReason` | = 20 |
| `WrongTreeID` | `NodeOpFailureReason` | = 21 |
| `LevelTooLow` | `NodeOpFailureReason` | = 22 |
| `TreeFlaggedNoRefund` | `NodeOpFailureReason` | = 23 |
| `NodeNeverPurchasable` | `NodeOpFailureReason` | = 24 |
| `AccountDataNoMatch` | `NodeOpFailureReason` | = 25 |
| `NotEnoughRanksInEntry` | `NodeOpFailureReason` | = 26 |

### RespecType

*Enumeration* · 6 values, 0..5

Access values as `Enum.RespecType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Talents` | `RespecType` | = 0 |
| `Glyphs` | `RespecType` | = 1 |
| `SetPrimarySpecialization` | `RespecType` | = 2 |
| `PetTalents` | `RespecType` | = 3 |
| `Legacy` | `RespecType` | = 4 |
| `Specialization` | `RespecType` | = 5 |

### SharedStringFlag

*Enumeration* · 1 values, 1..1

Access values as `Enum.SharedStringFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InternalOnly` | `SharedStringFlag` | = 1 |

### TraitCombatConfigFlags

*Enumeration* · 4 values, 1..8

Access values as `Enum.TraitCombatConfigFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ActiveForSpec` | `TraitCombatConfigFlags` | = 1 |
| `StarterBuild` | `TraitCombatConfigFlags` | = 2 |
| `SharedActionBars` | `TraitCombatConfigFlags` | = 4 |
| `SecondarySpec` | `TraitCombatConfigFlags` | = 8 |

### TraitCondFlag

*Enumeration* · 3 values, 1..4

Access values as `Enum.TraitCondFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsGate` | `TraitCondFlag` | = 1 |
| `IsAlwaysMet` | `TraitCondFlag` | = 2 |
| `IsSufficient` | `TraitCondFlag` | = 4 |

### TraitConditionType

*Enumeration* · 6 values, 0..5

Access values as `Enum.TraitConditionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `TraitConditionType` | = 0 |
| `Visible` | `TraitConditionType` | = 1 |
| `Granted` | `TraitConditionType` | = 2 |
| `Increased` | `TraitConditionType` | = 3 |
| `DisplayError` | `TraitConditionType` | = 4 |
| `RanksAllowed` | `TraitConditionType` | = 5 |

### TraitConfigDbState

*Enumeration* · 4 values, 0..3

Access values as `Enum.TraitConfigDbState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Ready` | `TraitConfigDbState` | = 0 |
| `Created` | `TraitConfigDbState` | = 1 |
| `Removed` | `TraitConfigDbState` | = 2 |
| `Deleted` | `TraitConfigDbState` | = 3 |

### TraitConfigType

*Enumeration* · 5 values, 0..4

Access values as `Enum.TraitConfigType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `TraitConfigType` | = 0 |
| `Combat` | `TraitConfigType` | = 1 |
| `Profession` | `TraitConfigType` | = 2 |
| `Generic` | `TraitConfigType` | = 3 |
| `CamelotCombat` | `TraitConfigType` | = 4 |

### TraitCurrencyFlag

*Enumeration* · 4 values, 1..8

Access values as `Enum.TraitCurrencyFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ShowQuantityAsSpent` | `TraitCurrencyFlag` | = 1 |
| `TraitSourcedShowMax` | `TraitCurrencyFlag` | = 2 |
| `UseClassIcon` | `TraitCurrencyFlag` | = 4 |
| `UseSpecIcon` | `TraitCurrencyFlag` | = 8 |

### TraitCurrencyType

*Enumeration* · 4 values, 0..3

Access values as `Enum.TraitCurrencyType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Gold` | `TraitCurrencyType` | = 0 |
| `CurrencyTypesBased` | `TraitCurrencyType` | = 1 |
| `TraitSourced` | `TraitCurrencyType` | = 2 |
| `TraitSourcedPlayerDataElement` | `TraitCurrencyType` | = 3 |

### TraitDefinitionSubType

*Enumeration* · 5 values, 0..4

Access values as `Enum.TraitDefinitionSubType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DragonflightRed` | `TraitDefinitionSubType` | = 0 |
| `DragonflightBlue` | `TraitDefinitionSubType` | = 1 |
| `DragonflightGreen` | `TraitDefinitionSubType` | = 2 |
| `DragonflightBronze` | `TraitDefinitionSubType` | = 3 |
| `DragonflightBlack` | `TraitDefinitionSubType` | = 4 |

### TraitEdgeType

*Enumeration* · 6 values, 0..5

Access values as `Enum.TraitEdgeType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `VisualOnly` | `TraitEdgeType` | = 0 |
| `DeprecatedRankConnection` | `TraitEdgeType` | = 1 |
| `SufficientForAvailability` | `TraitEdgeType` | = 2 |
| `RequiredForAvailability` | `TraitEdgeType` | = 3 |
| `MutuallyExclusive` | `TraitEdgeType` | = 4 |
| `DeprecatedSelectionOption` | `TraitEdgeType` | = 5 |

### TraitEdgeVisualStyle

*Enumeration* · 2 values, 0..1

Access values as `Enum.TraitEdgeVisualStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TraitEdgeVisualStyle` | = 0 |
| `Straight` | `TraitEdgeVisualStyle` | = 1 |

### TraitNodeEntryType

*Enumeration* · 15 values, 0..14

Access values as `Enum.TraitNodeEntryType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `SpendHex` | `TraitNodeEntryType` | = 0 |
| `SpendSquare` | `TraitNodeEntryType` | = 1 |
| `SpendCircle` | `TraitNodeEntryType` | = 2 |
| `SpendSmallCircle` | `TraitNodeEntryType` | = 3 |
| `DeprecatedSelect` | `TraitNodeEntryType` | = 4 |
| `DragAndDrop` | `TraitNodeEntryType` | = 5 |
| `SpendDiamond` | `TraitNodeEntryType` | = 6 |
| `ProfPath` | `TraitNodeEntryType` | = 7 |
| `ProfPerk` | `TraitNodeEntryType` | = 8 |
| `ProfPathUnlock` | `TraitNodeEntryType` | = 9 |
| `RedButton` | `TraitNodeEntryType` | = 10 |
| `ArmorSet` | `TraitNodeEntryType` | = 11 |
| `SpendInfinite` | `TraitNodeEntryType` | = 12 |
| `SpendCapstoneCircle` | `TraitNodeEntryType` | = 13 |
| `SpendCapstoneSquare` | `TraitNodeEntryType` | = 14 |

### TraitNodeFlag

*Enumeration* · 9 values, 1..256

Access values as `Enum.TraitNodeFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ShowMultipleIcons` | `TraitNodeFlag` | = 1 |
| `NeverPurchasable` | `TraitNodeFlag` | = 2 |
| `TestPositionLocked` | `TraitNodeFlag` | = 4 |
| `TestGridPositioned` | `TraitNodeFlag` | = 8 |
| `ActiveAtFirstRank` | `TraitNodeFlag` | = 16 |
| `ShowExpandedSelection` | `TraitNodeFlag` | = 32 |
| `HideMaxRank` | `TraitNodeFlag` | = 64 |
| `HighestChosenRank` | `TraitNodeFlag` | = 128 |
| `ShowTierTrack` | `TraitNodeFlag` | = 256 |

### TraitNodeGroupFlag

*Enumeration* · 1 values, 1..1

Access values as `Enum.TraitNodeGroupFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AvailableByDefault` | `TraitNodeGroupFlag` | = 1 |

### TraitNodeType

*Enumeration* · 4 values, 0..3

Access values as `Enum.TraitNodeType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Single` | `TraitNodeType` | = 0 |
| `Tiered` | `TraitNodeType` | = 1 |
| `Selection` | `TraitNodeType` | = 2 |
| `SubTreeSelection` | `TraitNodeType` | = 3 |

### TraitPointsOperationType

*Enumeration* · 3 values, -1..1

Access values as `Enum.TraitPointsOperationType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TraitPointsOperationType` | = -1 |
| `Set` | `TraitPointsOperationType` | = 0 |
| `Multiply` | `TraitPointsOperationType` | = 1 |

### TraitSystemFlag

*Enumeration* · 4 values, 1..8

Access values as `Enum.TraitSystemFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `AllowMultipleLoadoutsPerTree` | `TraitSystemFlag` | = 1 |
| `ShowSpendConfirmation` | `TraitSystemFlag` | = 2 |
| `AllowEditInCombat` | `TraitSystemFlag` | = 4 |
| `AllowEditInChallengeMode` | `TraitSystemFlag` | = 8 |

### TraitSystemVariationType

*Enumeration* · 2 values, 0..1

Access values as `Enum.TraitSystemVariationType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TraitSystemVariationType` | = 0 |
| `Spec` | `TraitSystemVariationType` | = 1 |

### TraitTreeFlag

*Enumeration* · 2 values, 1..2

Access values as `Enum.TraitTreeFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `CannotRefund` | `TraitTreeFlag` | = 1 |
| `HideSingleRankNumbers` | `TraitTreeFlag` | = 2 |

### TraitVendorResetFailureReason

*Enumeration* · 3 values, 0..2

Access values as `Enum.TraitVendorResetFailureReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `TraitVendorResetFailureReason` | = 0 |
| `DataError` | `TraitVendorResetFailureReason` | = 1 |
| `ClassPointDeficit` | `TraitVendorResetFailureReason` | = 2 |

### TraitConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `MAX_COMBAT_TRAIT_CONFIGS` | `number` | = `40` |
| `COMMIT_COMBAT_TRAIT_CONFIG_CHANGES_SPELL_ID` | `number` | = `384255` |
| `INSPECT_TRAIT_CONFIG_ID` | `number` | = `-1` |
| `STARTER_BUILD_TRAIT_CONFIG_ID` | `number` | = `-2` |
| `VIEW_TRAIT_CONFIG_ID` | `number` | = `-3` |
