# Calendar

Namespace `C_Calendar` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/calendardocumentation.lua` (FileDataID 4637052)

## Functions

### AddEvent

```lua
C_Calendar.AddEvent()
```

`HasRestrictions`

### AreNamesReady

```lua
C_Calendar.AreNamesReady() -> ready: bool
```

### CanAddEvent

```lua
C_Calendar.CanAddEvent() -> canAddEvent: bool
```

### CanSendInvite

```lua
C_Calendar.CanSendInvite() -> canSendInvite: bool
```

### CloseEvent

```lua
C_Calendar.CloseEvent()
```

### ContextMenuEventCanComplain

```lua
C_Calendar.ContextMenuEventCanComplain(offsetMonths: number, monthDay: luaIndex, eventIndex: luaIndex) -> canComplain: bool
```

`SecretArguments=AllowedWhenUntainted`

### ContextMenuEventCanEdit

```lua
C_Calendar.ContextMenuEventCanEdit(offsetMonths: number, monthDay: luaIndex, eventIndex: luaIndex) -> canEdit: bool
```

`SecretArguments=AllowedWhenUntainted`

### ContextMenuEventCanRemove

```lua
C_Calendar.ContextMenuEventCanRemove(offsetMonths: number, monthDay: luaIndex, eventIndex: luaIndex) -> canRemove: bool
```

`SecretArguments=AllowedWhenUntainted`

### ContextMenuEventClipboard

```lua
C_Calendar.ContextMenuEventClipboard() -> exists: bool
```

### ContextMenuEventCopy

```lua
C_Calendar.ContextMenuEventCopy()
```

### ContextMenuEventGetCalendarType

```lua
C_Calendar.ContextMenuEventGetCalendarType() -> calendarType: string?
```

### ContextMenuEventPaste

```lua
C_Calendar.ContextMenuEventPaste(offsetMonths: number, monthDay: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### ContextMenuEventRemove

```lua
C_Calendar.ContextMenuEventRemove()
```

### ContextMenuEventSignUp

```lua
C_Calendar.ContextMenuEventSignUp()
```

### ContextMenuGetEventIndex

```lua
C_Calendar.ContextMenuGetEventIndex() -> info: CalendarEventIndexInfo
```

`MayReturnNothing`

### ContextMenuInviteAvailable

```lua
C_Calendar.ContextMenuInviteAvailable()
```

### ContextMenuInviteDecline

```lua
C_Calendar.ContextMenuInviteDecline()
```

### ContextMenuInviteRemove

```lua
C_Calendar.ContextMenuInviteRemove()
```

### ContextMenuInviteTentative

```lua
C_Calendar.ContextMenuInviteTentative()
```

### ContextMenuSelectEvent

```lua
C_Calendar.ContextMenuSelectEvent(offsetMonths: number, monthDay: luaIndex, eventIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### CreateCommunitySignUpEvent

```lua
C_Calendar.CreateCommunitySignUpEvent()
```

### CreateGuildAnnouncementEvent

```lua
C_Calendar.CreateGuildAnnouncementEvent()
```

### CreateGuildSignUpEvent

```lua
C_Calendar.CreateGuildSignUpEvent()
```

### CreatePlayerEvent

```lua
C_Calendar.CreatePlayerEvent()
```

### EventAvailable

```lua
C_Calendar.EventAvailable()
```

### EventCanEdit

```lua
C_Calendar.EventCanEdit() -> canEdit: bool
```

### EventClearAutoApprove

```lua
C_Calendar.EventClearAutoApprove()
```

### EventClearLocked

```lua
C_Calendar.EventClearLocked()
```

### EventClearModerator

```lua
C_Calendar.EventClearModerator(inviteIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### EventDecline

```lua
C_Calendar.EventDecline()
```

### EventGetCalendarType

```lua
C_Calendar.EventGetCalendarType() -> calendarType: string?
```

### EventGetClubId

```lua
C_Calendar.EventGetClubId() -> info: ClubId?
```

### EventGetInvite

```lua
C_Calendar.EventGetInvite(eventIndex: luaIndex) -> info: CalendarEventInviteInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### EventGetInviteResponseTime

```lua
C_Calendar.EventGetInviteResponseTime(eventIndex: luaIndex) -> time: CalendarTime
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### EventGetInviteSortCriterion

```lua
C_Calendar.EventGetInviteSortCriterion() -> criterion: string, reverse: bool
```

### EventGetSelectedInvite

```lua
C_Calendar.EventGetSelectedInvite() -> inviteIndex: luaIndex?
```

### EventGetStatusOptions

```lua
C_Calendar.EventGetStatusOptions(eventIndex: luaIndex) -> options: CalendarEventStatusOption[]
```

`SecretArguments=AllowedWhenUntainted`

### EventGetTextures

```lua
C_Calendar.EventGetTextures(eventType: CalendarEventType) -> textures: CalendarEventTextureInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### EventGetTypes

```lua
C_Calendar.EventGetTypes() -> types: string[]
```

### EventGetTypesDisplayOrdered

```lua
C_Calendar.EventGetTypesDisplayOrdered() -> infos: CalendarEventTypeDisplayInfo[]
```

### EventHasPendingInvite

```lua
C_Calendar.EventHasPendingInvite() -> hasPendingInvite: bool
```

### EventHaveSettingsChanged

```lua
C_Calendar.EventHaveSettingsChanged() -> haveSettingsChanged: bool
```

### EventInvite

```lua
C_Calendar.EventInvite(name: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### EventRemoveInvite

```lua
C_Calendar.EventRemoveInvite(inviteIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### EventRemoveInviteByGuid

```lua
C_Calendar.EventRemoveInviteByGuid(guid: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### EventSelectInvite

```lua
C_Calendar.EventSelectInvite(inviteIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetAutoApprove

```lua
C_Calendar.EventSetAutoApprove()
```

### EventSetClubId

```lua
C_Calendar.EventSetClubId(clubId: ClubId?)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetDate

```lua
C_Calendar.EventSetDate(month: luaIndex, monthDay: luaIndex, year: number)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetDescription

```lua
C_Calendar.EventSetDescription(description: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetInviteStatus

```lua
C_Calendar.EventSetInviteStatus(eventIndex: luaIndex, status: CalendarStatus)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetLocked

```lua
C_Calendar.EventSetLocked()
```

### EventSetModerator

```lua
C_Calendar.EventSetModerator(inviteIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetTextureID

```lua
C_Calendar.EventSetTextureID(textureIndex: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetTime

```lua
C_Calendar.EventSetTime(hour: number, minute: number)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetTitle

```lua
C_Calendar.EventSetTitle(title: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### EventSetType

```lua
C_Calendar.EventSetType(typeIndex: CalendarEventType)
```

`SecretArguments=AllowedWhenUntainted`

### EventSignUp

```lua
C_Calendar.EventSignUp()
```

### EventSortInvites

```lua
C_Calendar.EventSortInvites(criterion: cstring, reverse: bool)
```

`SecretArguments=AllowedWhenUntainted`

### EventTentative

```lua
C_Calendar.EventTentative()
```

### GetClubCalendarEvents

```lua
C_Calendar.GetClubCalendarEvents(clubId: ClubId, startTime: CalendarTime, endTime: CalendarTime) -> events: CalendarDayEvent[]
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetDayEvent

```lua
C_Calendar.GetDayEvent(monthOffset: number, monthDay: luaIndex, index: luaIndex) -> event: CalendarDayEvent
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetDefaultGuildFilter

```lua
C_Calendar.GetDefaultGuildFilter() -> info: CalendarGuildFilterInfo
```

### GetEventIndex

```lua
C_Calendar.GetEventIndex() -> info: CalendarEventIndexInfo
```

`MayReturnNothing`

### GetEventIndexInfo

```lua
C_Calendar.GetEventIndexInfo(eventID: CalendarEventID, monthOffset: number?, monthDay: number?) -> eventIndexInfo: CalendarEventIndexInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetEventInfo

```lua
C_Calendar.GetEventInfo() -> info: CalendarEventInfo
```

`MayReturnNothing`

### GetFirstPendingInvite

```lua
C_Calendar.GetFirstPendingInvite(offsetMonths: number, monthDay: luaIndex) -> firstPendingInvite: luaIndex?
```

`SecretArguments=AllowedWhenUntainted`

### GetGuildEventInfo

```lua
C_Calendar.GetGuildEventInfo(index: luaIndex) -> info: CalendarGuildEventInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetGuildEventSelectionInfo

```lua
C_Calendar.GetGuildEventSelectionInfo(index: luaIndex) -> info: CalendarEventIndexInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHolidayInfo

```lua
C_Calendar.GetHolidayInfo(monthOffset: number, monthDay: luaIndex, index: luaIndex) -> event: CalendarHolidayInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMaxCreateDate

```lua
C_Calendar.GetMaxCreateDate() -> maxCreateDate: CalendarTime
```

### GetMinDate

```lua
C_Calendar.GetMinDate() -> minDate: CalendarTime
```

### GetMonthInfo

```lua
C_Calendar.GetMonthInfo(offsetMonths: number) -> monthInfo: CalendarMonthInfo
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `offsetMonths` | `number` | default `0` |

### GetNextClubId

```lua
C_Calendar.GetNextClubId() -> clubId: ClubId?
```

### GetNumDayEvents

```lua
C_Calendar.GetNumDayEvents(offsetMonths: number, monthDay: luaIndex) -> numDayEvents: number
```

`SecretArguments=AllowedWhenUntainted`

### GetNumGuildEvents

```lua
C_Calendar.GetNumGuildEvents() -> numGuildEvents: number
```

### GetNumInvites

```lua
C_Calendar.GetNumInvites() -> num: number
```

### GetNumPendingInvites

```lua
C_Calendar.GetNumPendingInvites() -> num: number
```

### GetRaidInfo

```lua
C_Calendar.GetRaidInfo(offsetMonths: number, monthDay: luaIndex, eventIndex: luaIndex) -> info: CalendarRaidInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### IsActionPending

```lua
C_Calendar.IsActionPending() -> actionPending: bool
```

### IsEventOpen

```lua
C_Calendar.IsEventOpen() -> isOpen: bool
```

### MassInviteCommunity

```lua
C_Calendar.MassInviteCommunity(clubId: ClubId, minLevel: number, maxLevel: number, maxRankOrder: luaIndex?)
```

`SecretArguments=AllowedWhenUntainted`

### MassInviteGuild

```lua
C_Calendar.MassInviteGuild(minLevel: number, maxLevel: number, maxRankOrder: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### OpenCalendar

```lua
C_Calendar.OpenCalendar()
```

### OpenEvent

```lua
C_Calendar.OpenEvent(offsetMonths: number, monthDay: luaIndex, index: luaIndex) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### RemoveEvent

```lua
C_Calendar.RemoveEvent()
```

### SetAbsMonth

```lua
C_Calendar.SetAbsMonth(month: luaIndex, year: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMonth

```lua
C_Calendar.SetMonth(offsetMonths: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetNextClubId

```lua
C_Calendar.SetNextClubId(clubId: ClubId?)
```

`SecretArguments=AllowedWhenUntainted`

### UpdateEvent

```lua
C_Calendar.UpdateEvent()
```

`HasRestrictions`

## Events

### CALENDAR_ACTION_PENDING

```lua
CALENDAR_ACTION_PENDING(pending: bool)
```

`SynchronousEvent`

### CALENDAR_CLOSE_EVENT

```lua
CALENDAR_CLOSE_EVENT()
```

`SynchronousEvent`

### CALENDAR_EVENT_ALARM

```lua
CALENDAR_EVENT_ALARM(title: cstring, hour: number, minute: number)
```

`SynchronousEvent`

### CALENDAR_NEW_EVENT

```lua
CALENDAR_NEW_EVENT(isCopy: bool)
```

`SynchronousEvent`

### CALENDAR_OPEN_EVENT

```lua
CALENDAR_OPEN_EVENT(calendarType: cstring)
```

`SynchronousEvent`

### CALENDAR_UPDATE_ERROR

```lua
CALENDAR_UPDATE_ERROR(errorReason: cstring)
```

`SynchronousEvent`

### CALENDAR_UPDATE_ERROR_WITH_COUNT

```lua
CALENDAR_UPDATE_ERROR_WITH_COUNT(errorReason: cstring, count: number)
```

`SynchronousEvent`

### CALENDAR_UPDATE_ERROR_WITH_PLAYER_NAME

```lua
CALENDAR_UPDATE_ERROR_WITH_PLAYER_NAME(errorReason: cstring, playerName: cstring)
```

`SynchronousEvent`

### CALENDAR_UPDATE_EVENT

```lua
CALENDAR_UPDATE_EVENT()
```

`SynchronousEvent`

### CALENDAR_UPDATE_EVENT_LIST

```lua
CALENDAR_UPDATE_EVENT_LIST()
```

`SynchronousEvent` `UniqueEvent`

### CALENDAR_UPDATE_GUILD_EVENTS

```lua
CALENDAR_UPDATE_GUILD_EVENTS()
```

`SynchronousEvent`

### CALENDAR_UPDATE_INVITE_LIST

```lua
CALENDAR_UPDATE_INVITE_LIST(hasCompleteList: bool?)
```

`SynchronousEvent`

### CALENDAR_UPDATE_PENDING_INVITES

```lua
CALENDAR_UPDATE_PENDING_INVITES()
```

`SynchronousEvent`

## Types

### CalendarDayEvent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `eventID` | `CalendarEventID` |  |
| `title` | `string` |  |
| `isCustomTitle` | `bool` |  |
| `startTime` | `CalendarTime` |  |
| `endTime` | `CalendarTime` |  |
| `calendarType` | `cstring` |  |
| `sequenceType` | `cstring` |  |
| `eventType` | `CalendarEventType` |  |
| `iconTexture` | `fileID?` |  |
| `modStatus` | `cstring` |  |
| `inviteStatus` | `CalendarStatus` |  |
| `invitedBy` | `string` |  |
| `difficulty` | `number` |  |
| `inviteType` | `CalendarInviteType` |  |
| `sequenceIndex` | `luaIndex` |  |
| `numSequenceDays` | `number` |  |
| `difficultyName` | `cstring` |  |
| `dontDisplayBanner` | `bool` |  |
| `dontDisplayEnd` | `bool` |  |
| `clubID` | `ClubId` |  |
| `isLocked` | `bool` |  |

### CalendarEventIndexInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `offsetMonths` | `number` |  |
| `monthDay` | `luaIndex` |  |
| `eventIndex` | `luaIndex` |  |

### CalendarEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `description` | `string` |  |
| `creator` | `string?` |  |
| `eventType` | `CalendarEventType` |  |
| `repeatOption` | `CalendarEventRepeatOptions` |  |
| `maxSize` | `number` |  |
| `textureIndex` | `luaIndex?` |  |
| `time` | `CalendarTime` |  |
| `lockoutTime` | `CalendarTime` |  |
| `isLocked` | `bool` |  |
| `isAutoApprove` | `bool` |  |
| `hasPendingInvite` | `bool` |  |
| `inviteStatus` | `CalendarStatus?` |  |
| `inviteType` | `CalendarInviteType?` |  |
| `calendarType` | `string` |  |
| `communityName` | `string?` |  |

### CalendarEventInviteInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `level` | `number` |  |
| `className` | `string?` |  |
| `classFilename` | `string?` |  |
| `inviteStatus` | `CalendarStatus?` |  |
| `modStatus` | `string?` |  |
| `inviteIsMine` | `bool` |  |
| `type` | `CalendarInviteType` |  |
| `notes` | `string` |  |
| `classID` | `number?` |  |
| `guid` | `WOWGUID` |  |

### CalendarEventStatusOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `status` | `CalendarStatus` |  |
| `statusString` | `string` |  |

### CalendarEventTextureInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `title` | `string` |  |
| `iconTexture` | `fileID` |  |
| `expansionLevel` | `number` |  |
| `difficultyId` | `number?` |  |
| `mapId` | `number?` |  |
| `isLfr` | `bool?` |  |

### CalendarEventTypeDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `displayString` | `string` |  |
| `eventType` | `CalendarEventType` |  |

### CalendarGuildEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `eventID` | `CalendarEventID` |  |
| `year` | `number` |  |
| `month` | `luaIndex` |  |
| `monthDay` | `luaIndex` |  |
| `weekday` | `luaIndex` |  |
| `hour` | `number` |  |
| `minute` | `number` |  |
| `eventType` | `CalendarEventType` |  |
| `title` | `string` |  |
| `calendarType` | `string` |  |
| `texture` | `fileID` |  |
| `inviteStatus` | `CalendarStatus` |  |
| `clubID` | `ClubId` |  |

### CalendarGuildFilterInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `minLevel` | `number` |  |
| `maxLevel` | `number` |  |
| `rank` | `number` |  |

### CalendarHolidayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `description` | `cstring` |  |
| `texture` | `fileID` |  |
| `startTime` | `CalendarTime?` |  |
| `endTime` | `CalendarTime?` |  |

### CalendarMonthInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `month` | `luaIndex` |  |
| `year` | `number` |  |
| `numDays` | `number` |  |
| `firstWeekday` | `luaIndex` |  |

### CalendarRaidInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `calendarType` | `string` |  |
| `raidID` | `number` |  |
| `time` | `CalendarTime` |  |
| `difficulty` | `number` |  |
| `difficultyName` | `string?` |  |
