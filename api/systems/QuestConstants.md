# QuestConstants

source `interface/addons/blizzard_apidocumentationgenerated/questconstantsdocumentation.lua` (FileDataID 4637168)

## Types

### CombinedQuestLogStatus

*Enumeration* · 8 values, 0..7

Access values as `Enum.CombinedQuestLogStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `CombinedQuestLogStatus` | = 0 |
| `Complete` | `CombinedQuestLogStatus` | = 1 |
| `CompleteDaily` | `CombinedQuestLogStatus` | = 2 |
| `CompleteWeekly` | `CombinedQuestLogStatus` | = 3 |
| `CompleteMonthly` | `CombinedQuestLogStatus` | = 4 |
| `CompleteYearly` | `CombinedQuestLogStatus` | = 5 |
| `CompleteGameReset` | `CombinedQuestLogStatus` | = 6 |
| `Reset` | `CombinedQuestLogStatus` | = 7 |

### CombinedQuestStatus

*Enumeration* · 3 values, 0..2

Access values as `Enum.CombinedQuestStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invalid` | `CombinedQuestStatus` | = 0 |
| `Completed` | `CombinedQuestStatus` | = 1 |
| `NotCompleted` | `CombinedQuestStatus` | = 2 |

### QuestCompleteSpellType

*Enumeration* · 12 values, 0..11

Access values as `Enum.QuestCompleteSpellType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `LegacyBehavior` | `QuestCompleteSpellType` | = 0 |
| `Follower` | `QuestCompleteSpellType` | = 1 |
| `Tradeskill` | `QuestCompleteSpellType` | = 2 |
| `Ability` | `QuestCompleteSpellType` | = 3 |
| `Aura` | `QuestCompleteSpellType` | = 4 |
| `Spell` | `QuestCompleteSpellType` | = 5 |
| `Unlock` | `QuestCompleteSpellType` | = 6 |
| `Companion` | `QuestCompleteSpellType` | = 7 |
| `QuestlineUnlock` | `QuestCompleteSpellType` | = 8 |
| `QuestlineReward` | `QuestCompleteSpellType` | = 9 |
| `QuestlineUnlockPart` | `QuestCompleteSpellType` | = 10 |
| `PossibleReward` | `QuestCompleteSpellType` | = 11 |

### QuestRepeatability

*Enumeration* · 5 values, 0..4

Access values as `Enum.QuestRepeatability.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `QuestRepeatability` | = 0 |
| `Daily` | `QuestRepeatability` | = 1 |
| `Weekly` | `QuestRepeatability` | = 2 |
| `Turnin` | `QuestRepeatability` | = 3 |
| `World` | `QuestRepeatability` | = 4 |

### QuestRewardContextFlags

*Enumeration* · 3 values, 0..2

Access values as `Enum.QuestRewardContextFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `QuestRewardContextFlags` | = 0 |
| `FirstCompletionBonus` | `QuestRewardContextFlags` | = 1 |
| `RepeatCompletionBonus` | `QuestRewardContextFlags` | = 2 |

### QuestTagType

*Enumeration* · 20 values, 0..19

Access values as `Enum.QuestTagType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Tag` | `QuestTagType` | = 0 |
| `Profession` | `QuestTagType` | = 1 |
| `Normal` | `QuestTagType` | = 2 |
| `PvP` | `QuestTagType` | = 3 |
| `PetBattle` | `QuestTagType` | = 4 |
| `Bounty` | `QuestTagType` | = 5 |
| `Dungeon` | `QuestTagType` | = 6 |
| `Invasion` | `QuestTagType` | = 7 |
| `Raid` | `QuestTagType` | = 8 |
| `Contribution` | `QuestTagType` | = 9 |
| `RatedReward` | `QuestTagType` | = 10 |
| `InvasionWrapper` | `QuestTagType` | = 11 |
| `FactionAssault` | `QuestTagType` | = 12 |
| `Islands` | `QuestTagType` | = 13 |
| `Threat` | `QuestTagType` | = 14 |
| `CovenantCalling` | `QuestTagType` | = 15 |
| `DragonRiderRacing` | `QuestTagType` | = 16 |
| `Capstone` | `QuestTagType` | = 17 |
| `WorldBoss` | `QuestTagType` | = 18 |
| `Prey` | `QuestTagType` | = 19 |

### QuestTreasurePickerType

*Enumeration* · 3 values, 0..2

Access values as `Enum.QuestTreasurePickerType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Visible` | `QuestTreasurePickerType` | = 0 |
| `Hidden` | `QuestTreasurePickerType` | = 1 |
| `Select` | `QuestTreasurePickerType` | = 2 |

### RelativeContentDifficulty

*Enumeration* · 5 values, 0..4

Access values as `Enum.RelativeContentDifficulty.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Trivial` | `RelativeContentDifficulty` | = 0 |
| `Easy` | `RelativeContentDifficulty` | = 1 |
| `Fair` | `RelativeContentDifficulty` | = 2 |
| `Difficult` | `RelativeContentDifficulty` | = 3 |
| `Impossible` | `RelativeContentDifficulty` | = 4 |

### QuestInfoLuaConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `QUEST_INFO_ELITE_ID` | `number` | = `1` |
| `QUEST_INFO_DUNGEON_ID` | `number` | = `81` |
| `QUEST_INFO_PVP_ID` | `number` | = `41` |
| `QUEST_INFO_RAID_ID` | `number` | = `62` |

### QuestLogConstsMainlineCamelot

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `MAXIMUM_NUM_QUESTS_LOG_CAN_ACCEPT` | `number` | = `40` |

### QuestWatchConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `MAX_QUEST_WATCHES` | `number` | = `25` |
| `MAX_WORLD_QUEST_WATCHES_AUTOMATIC` | `number` | = `1` |
| `MAX_WORLD_QUEST_WATCHES_MANUAL` | `number` | = `5` |
