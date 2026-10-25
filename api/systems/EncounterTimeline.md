# EncounterTimeline

Namespace `C_EncounterTimeline` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encountertimelinedocumentation.lua` (FileDataID 7456201)

## Functions

### AddEditModeEvents

```lua
C_EncounterTimeline.AddEditModeEvents() -> loopTimerDuration: Seconds
```

Adds a predefined set of events to the timeline for display in Edit Mode.

### AddScriptEvent

```lua
C_EncounterTimeline.AddScriptEvent(eventInfo: EncounterTimelineScriptEventRequest) -> eventID: EncounterTimelineEventID
```

Adds a custom event to the timeline.

`SecretArguments=NotAllowed`

### CancelAllScriptEvents

```lua
C_EncounterTimeline.CancelAllScriptEvents()
```

Cancels all custom timeline events, removing them from the timeline.

### CancelEditModeEvents

```lua
C_EncounterTimeline.CancelEditModeEvents()
```

Removes all Edit Mode events from the timeline.

### CancelScriptEvent

```lua
C_EncounterTimeline.CancelScriptEvent(eventID: EncounterTimelineEventID)
```

Cancels a custom timeline event, removing it from the timeline.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### FinishScriptEvent

```lua
C_EncounterTimeline.FinishScriptEvent(eventID: EncounterTimelineEventID)
```

Finishes a custom timeline event, removing it from the timeline.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### GetCurrentTime

```lua
C_EncounterTimeline.GetCurrentTime() -> currentTime: Seconds
```

Returns the current timestamp used for rendering the timeline display.

### GetEventColor

```lua
C_EncounterTimeline.GetEventColor(eventID: EncounterTimelineEventID, overrideTrigger: EncounterEventColorTrigger?) -> color: colorRGBA
```

Returns the current color used to render timeline event.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent` `SecretWhenEncounterEvent`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |

### GetEventCountBySource

```lua
C_EncounterTimeline.GetEventCountBySource(source: EncounterTimelineEventSource) -> count: number
```

Returns the number of present events in the timeline by their source type.

`SecretArguments=AllowedWhenUntainted`

### GetEventHighlightTime

```lua
C_EncounterTimeline.GetEventHighlightTime() -> highlightTime: Seconds
```

Returns the duration at which timeline events will be highlighted for imminency.

### GetEventInfo

```lua
C_EncounterTimeline.GetEventInfo(eventID: EncounterTimelineEventID) -> info: EncounterTimelineEventInfo
```

Returns information about a timeline event. This data is generally expected to be static for the lifetime of an event.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent` `SecretWhenEncounterEvent`

### GetEventList

```lua
C_EncounterTimeline.GetEventList() -> events: EncounterTimelineEventID[]
```

Returns an unsorted list of event IDs present in the timeline.

### GetEventState

```lua
C_EncounterTimeline.GetEventState(eventID: EncounterTimelineEventID) -> state: EncounterTimelineEventState
```

Returns the current state of a timeline event.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### GetEventTimeElapsed

```lua
C_EncounterTimeline.GetEventTimeElapsed(eventID: EncounterTimelineEventID) -> timeElapsed: Seconds
```

Returns the elapsed duration of a timeline event.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### GetEventTimer

```lua
C_EncounterTimeline.GetEventTimer(eventID: EncounterTimelineEventID) -> duration: LuaDurationObject?
```

Returns a Duration object that tracks the elapsed duration of a timeline event. This object tracks the range [0, duration] of the event and automatically pauses its progression based on event state.

`SecretArguments=NotAllowed`

### GetEventTimeRemaining

```lua
C_EncounterTimeline.GetEventTimeRemaining(eventID: EncounterTimelineEventID) -> timeRemaining: Seconds
```

Returns the remaining duration of a timeline event.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### GetEventTrack

```lua
C_EncounterTimeline.GetEventTrack(eventID: EncounterTimelineEventID) -> track: EncounterTimelineTrack, trackSortIndex: luaIndex?
```

Returns information about the position of an event on the timeline.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### GetSortedEventList

```lua
C_EncounterTimeline.GetSortedEventList(maxEventCount: number?, maxEventDuration: Seconds?, excludeTerminalStates: bool, excludeHiddenEvents: bool) -> events: EncounterTimelineEventID[]
```

Returns a sorted list of event IDs present in the timeline from shortest to longest remaining durations, meeting the requirements of the specified filters.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `maxEventCount` | `number?` | Maximum number of sorted events to return. |
| `maxEventDuration` | `Seconds?` | Maximum duration of sorted events to return. |
| `excludeTerminalStates` | `bool` | default `true`; If false, include events that are terminal states such as Canceled or Finished. |
| `excludeHiddenEvents` | `bool` | default `true`; If false, include events that should be hidden by user configuration, such as events on long tracks when the user has opted to not show long countdowns. |

### GetTrackInfo

```lua
C_EncounterTimeline.GetTrackInfo(track: EncounterTimelineTrack) -> trackInfo: EncounterTimelineTrackInfo
```

Returns information for a single timeline track.

`SecretArguments=NotAllowed`

### GetTrackList

```lua
C_EncounterTimeline.GetTrackList() -> tracks: EncounterTimelineTrackInfo[]
```

Returns information about all timeline tracks.

### GetTrackMaxEventDuration

```lua
C_EncounterTimeline.GetTrackMaxEventDuration(track: EncounterTimelineTrack) -> maxEventDuration: Seconds
```

Returns the maximum permitted event duration on a single timeline track.

`SecretArguments=NotAllowed`

### GetTrackType

```lua
C_EncounterTimeline.GetTrackType(track: EncounterTimelineTrack) -> trackType: EncounterTimelineTrackType
```

Returns the type of a single timeline track.

`SecretArguments=NotAllowed`

### GetViewType

```lua
C_EncounterTimeline.GetViewType() -> viewType: EncounterTimelineViewType
```

Returns the current view type of the timeline.

### HasActiveEvents

```lua
C_EncounterTimeline.HasActiveEvents() -> hasActiveEvents: bool
```

Returns true if the timeline contains any events in the active state.

### HasAnyEvents

```lua
C_EncounterTimeline.HasAnyEvents() -> hasAnyEvents: bool
```

Returns true if the timeline contains any events in any state.

### HasPausedEvents

```lua
C_EncounterTimeline.HasPausedEvents() -> hasPausedEvents: bool
```

Returns true if the timeline contains any events in the paused state.

### HasVisibleEvents

```lua
C_EncounterTimeline.HasVisibleEvents() -> hasVisibleEvents: bool
```

Returns true if the timeline contains any events that are on visible tracks.

### IsEventBlocked

```lua
C_EncounterTimeline.IsEventBlocked(eventID: EncounterTimelineEventID) -> blocked: bool
```

Returns true if the event is in a 'blocked' state, where the cast for this event may not occur due to encounter conditions not being met.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### IsFeatureAvailable

```lua
C_EncounterTimeline.IsFeatureAvailable() -> isAvailable: bool
```

Returns true if the encounter timeline feature is available on this client.

### IsFeatureEnabled

```lua
C_EncounterTimeline.IsFeatureEnabled() -> isAvailableAndEnabled: bool
```

Returns true if the encounter timeline feature has been enabled by the player. This function will always return false if the feature is not available.

### PauseScriptEvent

```lua
C_EncounterTimeline.PauseScriptEvent(eventID: EncounterTimelineEventID)
```

Pauses a custom timeline event, hiding it from the timeline. A paused event can later be resumed to show it again, or canceled.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### ResumeScriptEvent

```lua
C_EncounterTimeline.ResumeScriptEvent(eventID: EncounterTimelineEventID)
```

Resumes a custom timeline event, showing it on the timeline again if it is currently paused.

`SecretArguments=NotAllowed` `RequiresValidTimelineEvent`

### SetEventIconTextures

```lua
C_EncounterTimeline.SetEventIconTextures(eventID: EncounterTimelineEventID, includeIcons: EncounterEventIconmask, textures: SimpleTexture[])
```

Updates a given vector of texture objects to reference art assets for icons associated with an event.

`SecretArguments=AllowedWhenUntainted` `RequiresValidTimelineEvent`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `eventID` | `EncounterTimelineEventID` |  |
| `includeIcons` | `EncounterEventIconmask` | Mask to apply to candidate icons. Any icon bits not present in this set will not be assigned to textures. |
| `textures` | `SimpleTexture[]` | Array of texture objects to update. This will change the assigned atlases and alpha values of the region, applying secret aspects to protect the data. |

### SetViewType

```lua
C_EncounterTimeline.SetViewType(viewType: EncounterTimelineViewType)
```

Changes the view type for the timeline. This adjusts track layouts to be more appropriate for a specific mode and optimizes event processing.

`SecretArguments=NotAllowed`

## Events

### ENCOUNTER_TIMELINE_EVENT_ADDED

```lua
ENCOUNTER_TIMELINE_EVENT_ADDED(eventInfo: EncounterTimelineEventInfo)
```

Fired when an event has been added to the timeline.

`SecretWhenEncounterEvent` `SynchronousEvent`

### ENCOUNTER_TIMELINE_EVENT_BLOCK_STATE_CHANGED

```lua
ENCOUNTER_TIMELINE_EVENT_BLOCK_STATE_CHANGED(eventID: EncounterTimelineEventID)
```

Fired when an event has transitioned into or out of a 'blocked' status.

`UniqueEvent`

### ENCOUNTER_TIMELINE_EVENT_COLOR_CHANGED

```lua
ENCOUNTER_TIMELINE_EVENT_COLOR_CHANGED(eventID: EncounterTimelineEventID)
```

Fired when an event has met a condition that should trigger a color change.

`UniqueEvent`

### ENCOUNTER_TIMELINE_EVENT_HIGHLIGHT

```lua
ENCOUNTER_TIMELINE_EVENT_HIGHLIGHT(eventID: EncounterTimelineEventID)
```

Fired when an event has met a condition that should trigger its highlight glow animation.

`UniqueEvent`

### ENCOUNTER_TIMELINE_EVENT_REMOVED

```lua
ENCOUNTER_TIMELINE_EVENT_REMOVED(eventID: EncounterTimelineEventID)
```

Fired when an event has been removed from the timeline. This is guaranteed to fire after an event has transitioned to a 'final' state such as Canceled or Finished, and will be delayed at least one game tick to allow for API queries to still access event data in OnUpdate scripts. This is fired post-removal of the event, and so queries using the supplied event ID will return nil.

`UniqueEvent`

### ENCOUNTER_TIMELINE_EVENT_STATE_CHANGED

```lua
ENCOUNTER_TIMELINE_EVENT_STATE_CHANGED(eventID: EncounterTimelineEventID)
```

Fired when an event has changed state.

`UniqueEvent`

### ENCOUNTER_TIMELINE_EVENT_TRACK_CHANGED

```lua
ENCOUNTER_TIMELINE_EVENT_TRACK_CHANGED(eventID: EncounterTimelineEventID)
```

Fired when an event has changed track, or has been re-ordered within its existing track.

`UniqueEvent`

### ENCOUNTER_TIMELINE_LAYOUT_UPDATED

```lua
ENCOUNTER_TIMELINE_LAYOUT_UPDATED()
```

Fired when the layout of tracks on the timeline has been updated. This can include changes to the minimum or maximum durations of tracks.

`SynchronousEvent`

### ENCOUNTER_TIMELINE_STATE_UPDATED

```lua
ENCOUNTER_TIMELINE_STATE_UPDATED()
```

Signaled when conditions controlling the visibility of the encounter timeline are updated.

`UniqueEvent`

### ENCOUNTER_TIMELINE_VIEW_ACTIVATED

```lua
ENCOUNTER_TIMELINE_VIEW_ACTIVATED(viewType: EncounterTimelineViewType)
```

Fired when a new timeline view is being activated. This is fired after a full layout and timeline data update, allowing the UI to immediately query the API and get usable results.

`SynchronousEvent`

### ENCOUNTER_TIMELINE_VIEW_DEACTIVATED

```lua
ENCOUNTER_TIMELINE_VIEW_DEACTIVATED(viewType: EncounterTimelineViewType)
```

Fired when the current timeline view is being deactivated. The UI should clear all stored timeline event data and release all frames back to pools during this event.

`SynchronousEvent`

## Types

### EncounterTimelineEventFilter

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maxEventCount` | `number?` | Maximum number of sorted events to return. |
| `maxEventDuration` | `Seconds?` | Maximum duration of sorted events to return. |
| `excludeTerminalStates` | `bool` | default `true`; If false, include events that are terminal states such as Canceled or Finished. |
| `excludeHiddenEvents` | `bool` | default `true`; If false, include events that should be hidden by user configuration, such as events on long tracks when the user has opted to not show long countdowns. |

### EncounterTimelineEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `EncounterTimelineEventID` | Instance ID for this event.; `NeverSecret` |
| `source` | `EncounterTimelineEventSource` | Source that this event came from.; `NeverSecret` |
| `spellName` | `string` | Spell name associated with this event. For script events, this may instead be the contents of the 'overrideName' field if it wasn't empty. |
| `spellID` | `number` | Spell ID associated with this event. |
| `iconFileID` | `fileID` | Icon file ID associated with this event. |
| `duration` | `Seconds` | Base duration of this event at the point that it was queued onto the timeline.; `NeverSecret` |
| `maxQueueDuration` | `Seconds` | Hold duration for this event after it reaches the end of the timeline. During this period, the event will sit in the queued track of the timeline until manually finished or this added duration expires.; `NeverSecret` |
| `icons` | `EncounterEventIconmask` | Bitmask of active icon states for this event. |
| `severity` | `EncounterEventSeverity` | Severity of this event. |
| `isApproximate` | `bool` | If true, this event is an approximation and may not occur exactly when the timeline suggests it will. |

### EncounterTimelineScriptEventRequest

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `spellID` | `number` |  |
| `iconFileID` | `fileID` |  |
| `duration` | `Seconds` |  |
| `maxQueueDuration` | `Seconds` | default `0` |
| `overrideName` | `stringView` | default `""` |
| `icons` | `EncounterEventIconmask?` |  |
| `severity` | `EncounterEventSeverity` | default `"Medium"` |
| `paused` | `bool` | default `false` |

### EncounterTimelineTrackInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `id` | `EncounterTimelineTrack` |  |
| `type` | `EncounterTimelineTrackType` |  |
| `minimumDuration` | `Seconds?` | The exclusive lower bound of durations for events on this track. If zero, this should be treated as an inclusive lower bound. This bound is ignored by the timeline sequence in circumstances where an adjacent Sorted track would exceed its maximum event count, requiring events be pushed 'to the left' by one track. |
| `maximumDuration` | `Seconds?` | The inclusive upper bound of durations for events on this track. |
| `minimumEventIntroDuration` | `Seconds?` | Lower duration bound for events that want to transition onto this track from an Indeterminate position. Events below this duration are artificially kept in the indeterminate track state until they can transition into a later track in the timeline sequence. |
| `minimumEventGapDuration` | `Seconds?` | Minimum duration gap that must exist between two sequential candidate events for this track. If two event durations have a distance under this figure, the later of the two events will be artifically kept in the indeterminate track state until it can transition into a later track in the timeline sequence. |
| `maximumEventCount` | `number?` | The maximum number of events permitted within this track. This only applies to Sorted tracks. |
| `sortDirection` | `EncounterTimelineEventSortDirection?` | Sort ordering for events within this track. This only applies to Sorted tracks. |

## Predicates

Conditions referenced by the flags above.

- `RequiresValidTimelineEvent` *Precondition* (failure mode: ReturnNothing)
- `SecretWhenEncounterEvent` *Secret*
