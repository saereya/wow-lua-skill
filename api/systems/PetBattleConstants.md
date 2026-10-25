# PetBattleConstants

source `interface/addons/blizzard_apidocumentationgenerated/petbattleconstantsdocumentation.lua` (FileDataID 4637150)

## Types

### PetBattleQueueStatus

*Enumeration* · 22 values, 0..21

Access values as `Enum.PetBattleQueueStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PetBattleQueueStatus` | = 0 |
| `Queued` | `PetBattleQueueStatus` | = 1 |
| `QueuedUpdate` | `PetBattleQueueStatus` | = 2 |
| `AlreadyQueued` | `PetBattleQueueStatus` | = 3 |
| `JoinFailed` | `PetBattleQueueStatus` | = 4 |
| `JoinFailedSlots` | `PetBattleQueueStatus` | = 5 |
| `JoinFailedJournalLock` | `PetBattleQueueStatus` | = 6 |
| `JoinFailedNeutral` | `PetBattleQueueStatus` | = 7 |
| `MatchAccepted` | `PetBattleQueueStatus` | = 8 |
| `MatchDeclined` | `PetBattleQueueStatus` | = 9 |
| `MatchOpponentDeclined` | `PetBattleQueueStatus` | = 10 |
| `ProposalTimedOut` | `PetBattleQueueStatus` | = 11 |
| `Removed` | `PetBattleQueueStatus` | = 12 |
| `RequeuedAfterInternalError` | `PetBattleQueueStatus` | = 13 |
| `RequeuedAfterOpponentRemoved` | `PetBattleQueueStatus` | = 14 |
| `Matchmaking` | `PetBattleQueueStatus` | = 15 |
| `LostConnection` | `PetBattleQueueStatus` | = 16 |
| `Shutdown` | `PetBattleQueueStatus` | = 17 |
| `Suspended` | `PetBattleQueueStatus` | = 18 |
| `Unsuspended` | `PetBattleQueueStatus` | = 19 |
| `InBattle` | `PetBattleQueueStatus` | = 20 |
| `NoBattlingHere` | `PetBattleQueueStatus` | = 21 |

### PetbattleSlot

*Enumeration* · 3 values, 0..2

Access values as `Enum.PetbattleSlot.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Slot_0` | `PetbattleSlot` | = 0 |
| `Slot_1` | `PetbattleSlot` | = 1 |
| `Slot_2` | `PetbattleSlot` | = 2 |

### PetbattleState

*Enumeration* · 7 values, 0..6

Access values as `Enum.PetbattleState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Created` | `PetbattleState` | = 0 |
| `WaitingPreBattle` | `PetbattleState` | = 1 |
| `RoundInProgress` | `PetbattleState` | = 2 |
| `WaitingForFrontPets` | `PetbattleState` | = 3 |
| `CreatedFailed` | `PetbattleState` | = 4 |
| `FinalRound` | `PetbattleState` | = 5 |
| `Finished` | `PetbattleState` | = 6 |

### PetBattleConsts

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `SUMMON_RANDOM_FAVORITE_BATTLEPET_SPELL_ID` | `number` | = `243819` |
