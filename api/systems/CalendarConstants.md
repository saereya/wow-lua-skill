# CalendarConstants

source `interface/addons/blizzard_apidocumentationgenerated/calendarconstantsdocumentation.lua` (FileDataID 4637041)

## Types

### CalendarCommandType

*Enumeration* · 12 values, 0..11

Access values as `Enum.CalendarCommandType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Create` | `CalendarCommandType` | = 0 |
| `Invite` | `CalendarCommandType` | = 1 |
| `Rsvp` | `CalendarCommandType` | = 2 |
| `RemoveInvite` | `CalendarCommandType` | = 3 |
| `RemoveEvent` | `CalendarCommandType` | = 4 |
| `Status` | `CalendarCommandType` | = 5 |
| `ModeratorStatus` | `CalendarCommandType` | = 6 |
| `GetCalendar` | `CalendarCommandType` | = 7 |
| `GetEvent` | `CalendarCommandType` | = 8 |
| `UpdateEvent` | `CalendarCommandType` | = 9 |
| `Complain` | `CalendarCommandType` | = 10 |
| `Notes` | `CalendarCommandType` | = 11 |

### CalendarErrorType

*Enumeration* · 51 values, 0..50

Access values as `Enum.CalendarErrorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `CalendarErrorType` | = 0 |
| `CommunityEventsExceeded` | `CalendarErrorType` | = 1 |
| `EventsExceeded` | `CalendarErrorType` | = 2 |
| `SelfInvitesExceeded` | `CalendarErrorType` | = 3 |
| `OtherInvitesExceeded` | `CalendarErrorType` | = 4 |
| `NoPermission` | `CalendarErrorType` | = 5 |
| `EventInvalid` | `CalendarErrorType` | = 6 |
| `NotInvited` | `CalendarErrorType` | = 7 |
| `UnknownError` | `CalendarErrorType` | = 8 |
| `NotInGuild` | `CalendarErrorType` | = 9 |
| `NotInCommunity` | `CalendarErrorType` | = 10 |
| `TargetAlreadyInvited` | `CalendarErrorType` | = 11 |
| `NameNotFound` | `CalendarErrorType` | = 12 |
| `WrongFaction` | `CalendarErrorType` | = 13 |
| `Ignored` | `CalendarErrorType` | = 14 |
| `InvitesExceeded` | `CalendarErrorType` | = 15 |
| `InvalidMaxSize` | `CalendarErrorType` | = 16 |
| `InvalidDate` | `CalendarErrorType` | = 17 |
| `InvalidTime` | `CalendarErrorType` | = 18 |
| `NoInvites` | `CalendarErrorType` | = 19 |
| `NeedsTitle` | `CalendarErrorType` | = 20 |
| `EventPassed` | `CalendarErrorType` | = 21 |
| `EventLocked` | `CalendarErrorType` | = 22 |
| `DeleteCreatorFailed` | `CalendarErrorType` | = 23 |
| `DataAlreadySet` | `CalendarErrorType` | = 24 |
| `CalendarDisabled` | `CalendarErrorType` | = 25 |
| `RestrictedAccount` | `CalendarErrorType` | = 26 |
| `ArenaEventsExceeded` | `CalendarErrorType` | = 27 |
| `RestrictedLevel` | `CalendarErrorType` | = 28 |
| `Squelched` | `CalendarErrorType` | = 29 |
| `NoInvite` | `CalendarErrorType` | = 30 |
| `ComplaintDisabled` | `CalendarErrorType` | = 31 |
| `ComplaintSelf` | `CalendarErrorType` | = 32 |
| `ComplaintSameGuild` | `CalendarErrorType` | = 33 |
| `ComplaintGm` | `CalendarErrorType` | = 34 |
| `ComplaintLimit` | `CalendarErrorType` | = 35 |
| `ComplaintNotFound` | `CalendarErrorType` | = 36 |
| `EventWrongServer` | `CalendarErrorType` | = 37 |
| `NoCommunityInvites` | `CalendarErrorType` | = 38 |
| `InvalidSignup` | `CalendarErrorType` | = 39 |
| `NoModerator` | `CalendarErrorType` | = 40 |
| `ModeratorRestricted` | `CalendarErrorType` | = 41 |
| `InvalidNotes` | `CalendarErrorType` | = 42 |
| `InvalidTitle` | `CalendarErrorType` | = 43 |
| `InvalidDescription` | `CalendarErrorType` | = 44 |
| `InvalidClub` | `CalendarErrorType` | = 45 |
| `CreatorNotFound` | `CalendarErrorType` | = 46 |
| `EventThrottled` | `CalendarErrorType` | = 47 |
| `InviteThrottled` | `CalendarErrorType` | = 48 |
| `Internal` | `CalendarErrorType` | = 49 |
| `ComplaintAdded` | `CalendarErrorType` | = 50 |

### CalendarEventBits

*Enumeration* · 15 values, 1..3788

Access values as `Enum.CalendarEventBits.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Player` | `CalendarEventBits` | = 1 |
| `GuildDeprecated` | `CalendarEventBits` | = 2 |
| `System` | `CalendarEventBits` | = 4 |
| `Holiday` | `CalendarEventBits` | = 8 |
| `Locked` | `CalendarEventBits` | = 16 |
| `AutoApprove` | `CalendarEventBits` | = 32 |
| `CommunityAnnouncement` | `CalendarEventBits` | = 64 |
| `RaidLockout` | `CalendarEventBits` | = 128 |
| `ArenaDeprecated` | `CalendarEventBits` | = 256 |
| `RaidResetDeprecated` | `CalendarEventBits` | = 512 |
| `CommunitySignup` | `CalendarEventBits` | = 1024 |
| `GuildSignup` | `CalendarEventBits` | = 2048 |
| `CommunityWide` | `CalendarEventBits` | = 3136 |
| `PlayerCreated` | `CalendarEventBits` | = 3395 |
| `CantComplain` | `CalendarEventBits` | = 3788 |

### CalendarEventRepeatOptions

*Enumeration* · 4 values, 0..3

Access values as `Enum.CalendarEventRepeatOptions.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Never` | `CalendarEventRepeatOptions` | = 0 |
| `Weekly` | `CalendarEventRepeatOptions` | = 1 |
| `Biweekly` | `CalendarEventRepeatOptions` | = 2 |
| `Monthly` | `CalendarEventRepeatOptions` | = 3 |

### CalendarEventType

*Enumeration* · 6 values, 0..5

Access values as `Enum.CalendarEventType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Raid` | `CalendarEventType` | = 0 |
| `Dungeon` | `CalendarEventType` | = 1 |
| `PvP` | `CalendarEventType` | = 2 |
| `Meeting` | `CalendarEventType` | = 3 |
| `Other` | `CalendarEventType` | = 4 |
| `HeroicDeprecated` | `CalendarEventType` | = 5 |

### CalendarFilterFlags

*Enumeration* · 5 values, 1..16

Access values as `Enum.CalendarFilterFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `WeeklyHoliday` | `CalendarFilterFlags` | = 1 |
| `Darkmoon` | `CalendarFilterFlags` | = 2 |
| `Battleground` | `CalendarFilterFlags` | = 4 |
| `RaidLockout` | `CalendarFilterFlags` | = 8 |
| `RaidReset` | `CalendarFilterFlags` | = 16 |

### CalendarGetEventType

*Enumeration* · 3 values, 0..2

Access values as `Enum.CalendarGetEventType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Get` | `CalendarGetEventType` | = 0 |
| `Add` | `CalendarGetEventType` | = 1 |
| `Copy` | `CalendarGetEventType` | = 2 |

### CalendarHolidayFilterType

*Enumeration* · 3 values, 0..2

Access values as `Enum.CalendarHolidayFilterType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Weekly` | `CalendarHolidayFilterType` | = 0 |
| `Darkmoon` | `CalendarHolidayFilterType` | = 1 |
| `Battleground` | `CalendarHolidayFilterType` | = 2 |

### CalendarInviteBits

*Enumeration* · 5 values, 0..8

Access values as `Enum.CalendarInviteBits.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CalendarInviteBits` | = 0 |
| `PendingInvite` | `CalendarInviteBits` | = 1 |
| `Moderator` | `CalendarInviteBits` | = 2 |
| `Creator` | `CalendarInviteBits` | = 4 |
| `Signup` | `CalendarInviteBits` | = 8 |

### CalendarInviteSortType

*Enumeration* · 6 values, 0..5

Access values as `Enum.CalendarInviteSortType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Name` | `CalendarInviteSortType` | = 0 |
| `Level` | `CalendarInviteSortType` | = 1 |
| `Class` | `CalendarInviteSortType` | = 2 |
| `Status` | `CalendarInviteSortType` | = 3 |
| `Party` | `CalendarInviteSortType` | = 4 |
| `Notes` | `CalendarInviteSortType` | = 5 |

### CalendarInviteType

*Enumeration* · 2 values, 0..1

Access values as `Enum.CalendarInviteType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Normal` | `CalendarInviteType` | = 0 |
| `Signup` | `CalendarInviteType` | = 1 |

### CalendarModeratorStatus

*Enumeration* · 3 values, 0..2

Access values as `Enum.CalendarModeratorStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `CalendarModeratorStatus` | = 0 |
| `Moderator` | `CalendarModeratorStatus` | = 1 |
| `Creator` | `CalendarModeratorStatus` | = 2 |

### CalendarStatus

*Enumeration* · 9 values, 0..8

Access values as `Enum.CalendarStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Invited` | `CalendarStatus` | = 0 |
| `Available` | `CalendarStatus` | = 1 |
| `Declined` | `CalendarStatus` | = 2 |
| `Confirmed` | `CalendarStatus` | = 3 |
| `Out` | `CalendarStatus` | = 4 |
| `Standby` | `CalendarStatus` | = 5 |
| `Signedup` | `CalendarStatus` | = 6 |
| `NotSignedup` | `CalendarStatus` | = 7 |
| `Tentative` | `CalendarStatus` | = 8 |

### CalendarTexturesType

*Enumeration* · 2 values, 0..1

Access values as `Enum.CalendarTexturesType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Dungeons` | `CalendarTexturesType` | = 0 |
| `Raid` | `CalendarTexturesType` | = 1 |

### CalendarType

*Enumeration* · 8 values, 0..7

Access values as `Enum.CalendarType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Player` | `CalendarType` | = 0 |
| `Community` | `CalendarType` | = 1 |
| `RaidLockout` | `CalendarType` | = 2 |
| `RaidResetDeprecated` | `CalendarType` | = 3 |
| `Holiday` | `CalendarType` | = 4 |
| `HolidayWeekly` | `CalendarType` | = 5 |
| `HolidayDarkmoon` | `CalendarType` | = 6 |
| `HolidayBattleground` | `CalendarType` | = 7 |

### CalendarWebActionType

*Enumeration* · 7 values, 0..6

Access values as `Enum.CalendarWebActionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Accept` | `CalendarWebActionType` | = 0 |
| `Decline` | `CalendarWebActionType` | = 1 |
| `Remove` | `CalendarWebActionType` | = 2 |
| `ReportSpam` | `CalendarWebActionType` | = 3 |
| `Signup` | `CalendarWebActionType` | = 4 |
| `Tentative` | `CalendarWebActionType` | = 5 |
| `TentativeSignup` | `CalendarWebActionType` | = 6 |

### HolidayCalendarFlags

*Enumeration* · 2 values, 1..2

Access values as `Enum.HolidayCalendarFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Alliance` | `HolidayCalendarFlags` | = 1 |
| `Horde` | `HolidayCalendarFlags` | = 2 |

### HolidayFlags

*Enumeration* · 8 values, 1..128

Access values as `Enum.HolidayFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `IsRegionwide` | `HolidayFlags` | = 1 |
| `DontShowInCalendar` | `HolidayFlags` | = 2 |
| `DontDisplayEnd` | `HolidayFlags` | = 4 |
| `DontDisplayBanner` | `HolidayFlags` | = 8 |
| `NotAvailableClientSide` | `HolidayFlags` | = 16 |
| `DurationUseMinutes` | `HolidayFlags` | = 32 |
| `BeginEventOnlyOnStageChange` | `HolidayFlags` | = 64 |
| `StagesUseDatetimes` | `HolidayFlags` | = 128 |

### CalendarGetEventTypeConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `DEFAULT_CALENDAR_GET_EVENT_TYPE` | `CalendarGetEventType` | = `Enum.CalendarGetEventType.Get` |
