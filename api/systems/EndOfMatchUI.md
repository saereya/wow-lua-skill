# EndOfMatchUI

Namespace `C_EndOfMatchUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/endofmatchuidocumentation.lua` (FileDataID 6225371)

## Functions

### GetEndOfMatchDetails

```lua
C_EndOfMatchUI.GetEndOfMatchDetails() -> matchDetails: MatchDetails?
```

## Events

### SHOW_END_OF_MATCH_UI

```lua
SHOW_END_OF_MATCH_UI()
```

`SynchronousEvent`

## Types

### EndOfMatchType

*Enumeration* · 2 values, 0..1

Access values as `Enum.EndOfMatchType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `EndOfMatchType` | = 0 |
| `Plunderstorm` | `EndOfMatchType` | = 1 |

### MatchDetailType

*Enumeration* · 3 values, 0..2

Access values as `Enum.MatchDetailType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Placement` | `MatchDetailType` | = 0 |
| `Kills` | `MatchDetailType` | = 1 |
| `PlunderAcquired` | `MatchDetailType` | = 2 |

### MatchDetail

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `MatchDetailType` |  |
| `value` | `number` |  |

### MatchDetails

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `matchType` | `EndOfMatchType` |  |
| `matchEnded` | `bool` |  |
| `detailsList` | `MatchDetail[]` |  |
