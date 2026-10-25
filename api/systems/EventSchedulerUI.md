# EventSchedulerUI

Namespace `C_EventScheduler` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/eventscheduleruidocumentation.lua` (FileDataID 6383235)

## Functions

### CanShowEvents

```lua
C_EventScheduler.CanShowEvents() -> canShow: bool
```

Returns true if there are any events eligible to show for the player.

### ClearReminder

```lua
C_EventScheduler.ClearReminder(eventKey: string)
```

Clears reminder on a scheduled event. Must use endTime to identify which specific instance in the case of repeating ones.

`SecretArguments=AllowedWhenUntainted`

### GetActiveContinentName

```lua
C_EventScheduler.GetActiveContinentName() -> name: string
```

Returns the name of the continent with current events

`MayReturnNothing`

### GetEventUiMapID

```lua
C_EventScheduler.GetEventUiMapID(areaPoiID: number) -> uiMapID: number?
```

Will try to figure out a UiMap for an areaPOI.

`SecretArguments=AllowedWhenUntainted`

### GetEventZoneName

```lua
C_EventScheduler.GetEventZoneName(areaPoiID: number) -> name: string?
```

Will try to figure out a map zone name for an areaPOI

`SecretArguments=AllowedWhenUntainted`

### GetOngoingEvents

```lua
C_EventScheduler.GetOngoingEvents() -> events: OngoingEventInfo[]
```

Will request data from the server on a throttle

`MayReturnNothing`

### GetScheduledEvents

```lua
C_EventScheduler.GetScheduledEvents() -> events: ScheduledEventInfo[]
```

Will request data from the server on a throttle

`MayReturnNothing`

### HasData

```lua
C_EventScheduler.HasData() -> hasData: bool
```

True if the server sent a list, even if the list had 0 events.

### HasSavedReminders

```lua
C_EventScheduler.HasSavedReminders() -> hasSavedReminders: bool
```

Returns whether there are any event reminders saved. Can include reminders that have expired since set and haven't gotten removed yet. Has to be called after cvars are loaded.

### RequestEvents

```lua
C_EventScheduler.RequestEvents()
```

Requests events from the server, subject to throttle

### SetReminder

```lua
C_EventScheduler.SetReminder(eventKey: string)
```

Sets reminder on a scheduled event. Must use endTime to identify which specific instance in the case of repeating ones.

`SecretArguments=AllowedWhenUntainted`

## Events

### EVENT_SCHEDULER_UPDATE

```lua
EVENT_SCHEDULER_UPDATE()
```

`SynchronousEvent`

## Types

### EventDisplayInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `hideTimeLeft` | `bool` | default `false` |
| `hideDescription` | `bool` | default `false` |
| `overrideAtlas` | `textureAtlas?` |  |
| `overrideTooltipWidgetSetID` | `number?` |  |

### OngoingEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `rewardsClaimed` | `bool` | default `false` |
| `displayInfo` | `EventDisplayInfo` |  |

### ScheduledEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `eventKey` | `string` |  |
| `eventID` | `number` |  |
| `areaPoiID` | `number` |  |
| `startTime` | `time_t` |  |
| `endTime` | `time_t` |  |
| `duration` | `time_t` |  |
| `hasReminder` | `bool` | default `false` |
| `rewardsClaimed` | `bool` | default `false` |
| `displayInfo` | `EventDisplayInfo` |  |
