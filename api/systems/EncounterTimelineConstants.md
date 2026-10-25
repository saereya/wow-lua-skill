# EncounterTimelineConstants

source `interface/addons/blizzard_apidocumentationgenerated/encountertimelineconstantsdocumentation.lua` (FileDataID 7456200)

## Types

### EncounterTimelineEventSortDirection

*Enumeration* · 2 values, 0..1

Access values as `Enum.EncounterTimelineEventSortDirection.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Descending` | `EncounterTimelineEventSortDirection` | = 0; Events are sorted in descending order (longest time remaining to shortest). |
| `Ascending` | `EncounterTimelineEventSortDirection` | = 1; Events are sorted in ascending order (shortest time remaining to longest). |

### EncounterTimelineEventSource

*Enumeration* · 3 values, 0..2

Enumeration of all encounter timeline event sources.

Access values as `Enum.EncounterTimelineEventSource.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Encounter` | `EncounterTimelineEventSource` | = 0; Source used for events added by an instance encounter. |
| `Script` | `EncounterTimelineEventSource` | = 1; Source used for events added by Lua scripting APIs. This is used to apply API restrictions; the Pause/Cancel/ResumeScriptEvent functions only work on Script events. |
| `EditMode` | `EncounterTimelineEventSource` | = 2; Source used for events added by the AddEditModeEvents script API. |

### EncounterTimelineEventState

*Enumeration* · 4 values, 0..3

Enumeration of all encounter timeline event states.

Access values as `Enum.EncounterTimelineEventState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Active` | `EncounterTimelineEventState` | = 0 |
| `Paused` | `EncounterTimelineEventState` | = 1 |
| `Finished` | `EncounterTimelineEventState` | = 2 |
| `Canceled` | `EncounterTimelineEventState` | = 3 |

### EncounterTimelineIconSet

*Enumeration* · 6 values, 1..6

Access values as `Enum.EncounterTimelineIconSet.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TankAlert` | `EncounterTimelineIconSet` | = 1 |
| `HealerAlert` | `EncounterTimelineIconSet` | = 2 |
| `DamageAlert` | `EncounterTimelineIconSet` | = 3 |
| `Deadly` | `EncounterTimelineIconSet` | = 4 |
| `Dispel` | `EncounterTimelineIconSet` | = 5 |
| `Enrage` | `EncounterTimelineIconSet` | = 6 |

### EncounterTimelineTrack

*Enumeration* · 5 values, 0..4

Enumeration of all encounter timeline tracks., Tracks are not permitted to overlap (but may have a zero duration span), and are contiguously ordered from shortest maximum duration to longest.

Access values as `Enum.EncounterTimelineTrack.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Queued` | `EncounterTimelineTrack` | = 0 |
| `Short` | `EncounterTimelineTrack` | = 1; This track always has a zero minimum duration. |
| `Medium` | `EncounterTimelineTrack` | = 2 |
| `Long` | `EncounterTimelineTrack` | = 3 |
| `Indeterminate` | `EncounterTimelineTrack` | = 4; This track is used as a placeholder for events whose position is not calculated and shouldn't appear on the timeline. |

### EncounterTimelineTrackType

*Enumeration* · 3 values, 0..2

Enumeration of all encounter timeline track types. Track types infer behavioral aspects of the track, for example whether or not we associate sort orders to events in the track.

Access values as `Enum.EncounterTimelineTrackType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Hidden` | `EncounterTimelineTrackType` | = 0 |
| `Sorted` | `EncounterTimelineTrackType` | = 1 |
| `Linear` | `EncounterTimelineTrackType` | = 2 |

### EncounterTimelineViewType

*Enumeration* · 3 values, 0..2

Enumeration of view types for the timeline., View types control layout parameters for the timeline such as maximum track durations and event counts, and optimize event processing for expected display behaviors.

Access values as `Enum.EncounterTimelineViewType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `EncounterTimelineViewType` | = 0; Configures the view for an empty timeline display. This mode is recommended for user addons that take full control of the timeline display. |
| `Timeline` | `EncounterTimelineViewType` | = 1; Configures the view for a linear timeline display. |
| `Bars` | `EncounterTimelineViewType` | = 2; Configures the view for a sorted timer bar display. |

### EncounterTimelineEventConstants

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `ENCOUNTER_TIMELINE_INVALID_EVENT` | `number` | = `0`; Constant used for invalid event IDs. Script APIs are guaranteed to always return nil data if supplied this ID, and events will never be added to the timeline with this ID. |
| `ENCOUNTER_TIMELINE_RESERVED_EVENT_COUNT` | `number` | = `40`; Minimum size of internal arrays that are preallocated for event storage. |

### EncounterTimelineIconMasks

*Constants*

Values:

| Name | Type | Notes |
|---|---|---|
| `EncounterTimelineTankAlertIcons` | `EncounterEventIconmask` | = `"TankRole"` |
| `EncounterTimelineHealerAlertIcons` | `EncounterEventIconmask` | = `"HealerRole"` |
| `EncounterTimelineDamageAlertIcons` | `EncounterEventIconmask` | = `"DpsRole"` |
| `EncounterTimelineDeadlyIcons` | `EncounterEventIconmask` | = `"DeadlyEffect"` |
| `EncounterTimelineDispelIcons` | `EncounterEventIconmask` | = `124` |
| `EncounterTimelineEnrageIcons` | `EncounterEventIconmask` | = `"EnrageEffect"` |
| `EncounterTimelineAllIcons` | `EncounterEventIconmask` | = `1023` |
| `EncounterTimelineRoleIcons` | `EncounterEventIconmask` | = `896` |
| `EncounterTimelineOtherIcons` | `EncounterEventIconmask` | = `127` |
| `EncounterTimelineNoIcons` | `EncounterEventIconmask` | = `0` |
