# PlayerChoiceConstants

source `interface/addons/blizzard_apidocumentationgenerated/playerchoiceconstantsdocumentation.lua` (FileDataID 8169111)

## Types

### PlayerChoiceFlags

*Enumeration* · 9 values, 1..256

Access values as `Enum.PlayerChoiceFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `InfiniteRange` | `PlayerChoiceFlags` | = 1 |
| `HideWarboardHeader` | `PlayerChoiceFlags` | = 2 |
| `KeepOpenAfterChoice` | `PlayerChoiceFlags` | = 4 |
| `DoNotRefresh` | `PlayerChoiceFlags` | = 8 |
| `ShowChoicesAsList` | `PlayerChoiceFlags` | = 16 |
| `RequiresSelection` | `PlayerChoiceFlags` | = 32 |
| `ShowChoicesAsGrid` | `PlayerChoiceFlags` | = 64 |
| `HideAnswerArt` | `PlayerChoiceFlags` | = 128 |
| `ShowChoicesAsColumns` | `PlayerChoiceFlags` | = 256 |

### PlayerChoiceLayout

*Enumeration* · 4 values, 0..3

Access values as `Enum.PlayerChoiceLayout.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `PlayerChoiceLayout` | = 0 |
| `Grid` | `PlayerChoiceLayout` | = 1 |
| `List` | `PlayerChoiceLayout` | = 2 |
| `Columns` | `PlayerChoiceLayout` | = 3 |

### PlayerChoiceResponseFlags

*Enumeration* · 10 values, 0..256

Access values as `Enum.PlayerChoiceResponseFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PlayerChoiceResponseFlags` | = 0 |
| `ShowAnswerDisabled` | `PlayerChoiceResponseFlags` | = 1 |
| `ShowArtDesaturated` | `PlayerChoiceResponseFlags` | = 2 |
| `ShowOptionDisabled` | `PlayerChoiceResponseFlags` | = 4 |
| `InvertCondition` | `PlayerChoiceResponseFlags` | = 8 |
| `ShowAnswerDisabledWhenConditionFails` | `PlayerChoiceResponseFlags` | = 16 |
| `ConsolidateWidgets` | `PlayerChoiceResponseFlags` | = 32 |
| `CheckmarkOnlyButton` | `PlayerChoiceResponseFlags` | = 64 |
| `HideButton` | `PlayerChoiceResponseFlags` | = 128 |
| `ShowAnswerSelected` | `PlayerChoiceResponseFlags` | = 256 |
