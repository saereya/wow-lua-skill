# EncounterEventsShared

source `interface/addons/blizzard_apidocumentationgenerated/encountereventsshareddocumentation.lua` (FileDataID 7730270)

## Types

### EncounterEventColorTrigger

*Enumeration* · 3 values, 0..2

Access values as `Enum.EncounterEventColorTrigger.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `TextWarning` | `EncounterEventColorTrigger` | = 0; Color to be used when an encounter event shown as a text warning alert. |
| `TimelineEvent` | `EncounterEventColorTrigger` | = 1; Color to be used when an encounter event is placed on the timeline. |
| `TimelineEventHighlight` | `EncounterEventColorTrigger` | = 2; Color to be used when an encounter event reaches its 'highlight' duration on the timeline (typically, ~5s before the cast is due). |

### EncounterEventSoundTrigger

*Enumeration* · 3 values, 0..2

Access values as `Enum.EncounterEventSoundTrigger.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `OnTextWarningShown` | `EncounterEventSoundTrigger` | = 0; Trigger to be activated when an text warning is initially shown for an encounter event. |
| `OnTimelineEventFinished` | `EncounterEventSoundTrigger` | = 1; Trigger to be activated when an encounter event on the timeline transitions to a finished (ie. casted, or resolved) state. |
| `OnTimelineEventHighlight` | `EncounterEventSoundTrigger` | = 2; Trigger to be activated when an encounter event reaches its 'highlight' duration on the timeline (typically, ~5s before the cast is due). |

### EncounterEventInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `encounterEventID` | `number` | ID of the encounter event record. |
| `enabled` | `bool` | If true, this event should be displayed on boss ability HUD elements. |
| `spellID` | `number` | Spell ID that triggers this event. A single spell may be used by multiple encounter events. |
| `iconFileID` | `number` | Icon file ID for the event. Typically the same as the spell icon, but may be overridden. |
| `severity` | `EncounterEventSeverity` | Severity level of this event. |
| `icons` | `EncounterEventIconmask` | Bitmask of spell support icons to show for this event. |

### EncounterEventSoundInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `file` | `FileAsset` | Sound file to be played when triggered. |
| `channel` | `UISoundSubType` | default `"g_defaultSI3UISoundSubTypeForLua"`; Sound channel to play this file on. |
| `volume` | `number` | default `1`; Volume scalar for the sound file. |
