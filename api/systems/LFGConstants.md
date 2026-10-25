# LFGConstants

source `interface/addons/blizzard_apidocumentationgenerated/lfgconstantsdocumentation.lua` (FileDataID 4637134)

## Types

### LFGEntryGeneralPlaystyle

*Enumeration* · 5 values, 0..4

Access values as `Enum.LFGEntryGeneralPlaystyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `LFGEntryGeneralPlaystyle` | = 0 |
| `Learning` | `LFGEntryGeneralPlaystyle` | = 1 |
| `FunRelaxed` | `LFGEntryGeneralPlaystyle` | = 2 |
| `FunSerious` | `LFGEntryGeneralPlaystyle` | = 3 |
| `Expert` | `LFGEntryGeneralPlaystyle` | = 4 |

### LFGEntryPlaystyle

*Enumeration* · 4 values, 0..3

Access values as `Enum.LFGEntryPlaystyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `LFGEntryPlaystyle` | = 0 |
| `Standard` | `LFGEntryPlaystyle` | = 1 |
| `Casual` | `LFGEntryPlaystyle` | = 2 |
| `Hardcore` | `LFGEntryPlaystyle` | = 3 |

### LFGEntryVoiceMode

*Enumeration* · 4 values, 0..3

Access values as `Enum.LFGEntryVoiceMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `LFGEntryVoiceMode` | = 0 |
| `Legacy` | `LFGEntryVoiceMode` | = 1 |
| `Discord` | `LFGEntryVoiceMode` | = 2 |
| `Custom` | `LFGEntryVoiceMode` | = 3 |

### LFGListDisplayType

*Enumeration* · 6 values, 0..5

Access values as `Enum.LFGListDisplayType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RoleCount` | `LFGListDisplayType` | = 0 |
| `RoleEnumerate` | `LFGListDisplayType` | = 1 |
| `ClassEnumerate` | `LFGListDisplayType` | = 2 |
| `HideAll` | `LFGListDisplayType` | = 3 |
| `PlayerCount` | `LFGListDisplayType` | = 4 |
| `Comment` | `LFGListDisplayType` | = 5 |

### LFGListFilter

*Enumeration* · 8 values, 1..128

Access values as `Enum.LFGListFilter.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Recommended` | `LFGListFilter` | = 1 |
| `NotRecommended` | `LFGListFilter` | = 2 |
| `PvE` | `LFGListFilter` | = 4 |
| `PvP` | `LFGListFilter` | = 8 |
| `Timerunning` | `LFGListFilter` | = 16 |
| `CurrentExpansion` | `LFGListFilter` | = 32 |
| `CurrentSeason` | `LFGListFilter` | = 64 |
| `NotCurrentSeason` | `LFGListFilter` | = 128 |

### LFGRole

*Enumeration* · 3 values, 0..2

Access values as `Enum.LFGRole.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Tank` | `LFGRole` | = 0 |
| `Healer` | `LFGRole` | = 1 |
| `Damage` | `LFGRole` | = 2 |

### LFGSlotInvalidReason

*Enumeration* · 20 values, 0..19

Access values as `Enum.LFGSlotInvalidReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `LFGSlotInvalidReason` | = 0 |
| `ExpansionTooLow` | `LFGSlotInvalidReason` | = 1 |
| `LevelTooLow` | `LFGSlotInvalidReason` | = 2 |
| `LevelTooHigh` | `LFGSlotInvalidReason` | = 3 |
| `GearTooLow` | `LFGSlotInvalidReason` | = 4 |
| `GearTooHigh` | `LFGSlotInvalidReason` | = 5 |
| `RaidLocked` | `LFGSlotInvalidReason` | = 6 |
| `LevelTargetTooLow` | `LFGSlotInvalidReason` | = 7 |
| `LevelTargetTooHigh` | `LFGSlotInvalidReason` | = 8 |
| `AreaNotExplored` | `LFGSlotInvalidReason` | = 9 |
| `WrongFaction` | `LFGSlotInvalidReason` | = 10 |
| `NoValidRoles` | `LFGSlotInvalidReason` | = 11 |
| `EngagedInPvP` | `LFGSlotInvalidReason` | = 12 |
| `NoSpec` | `LFGSlotInvalidReason` | = 13 |
| `CannotRunAnyChildDungeon` | `LFGSlotInvalidReason` | = 14 |
| `Restricted` | `LFGSlotInvalidReason` | = 15 |
| `ChromieTime` | `LFGSlotInvalidReason` | = 16 |
| `Npe` | `LFGSlotInvalidReason` | = 17 |
| `Timerunning` | `LFGSlotInvalidReason` | = 18 |
| `PlayerConditionFailed` | `LFGSlotInvalidReason` | = 19 |

### PremadeGroupFinderStyle

*Enumeration* · 3 values, 0..2

Access values as `Enum.PremadeGroupFinderStyle.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Disabled` | `PremadeGroupFinderStyle` | = 0 |
| `Mainline` | `PremadeGroupFinderStyle` | = 1 |
| `Vanilla` | `PremadeGroupFinderStyle` | = 2 |

### LFGConstsExposed

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `GROUP_FINDER_MAX_ACTIVITY_CAPACITY` | `number` | = `16` |

### LFG_ROLEConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `LFG_ROLE_NO_ROLE` | `LFGRole` | = `-1` |
| `LFG_ROLE_ANY` | `LFGRole` | = `Enum.LFGRoleMeta.NumValues` |

### LFGRoles

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `tank` | `bool` |  |
| `healer` | `bool` |  |
| `dps` | `bool` |  |
