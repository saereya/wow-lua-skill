# EncounterEvents

Namespace `C_EncounterEvents` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/encountereventsdocumentation.lua` (FileDataID 7730093)

## Functions

### GetEventColor

```lua
C_EncounterEvents.GetEventColor(encounterEventID: number, trigger: EncounterEventColorTrigger) -> color: colorRGBA?
```

Returns any custom color override applied for an encounter event.

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA?` | `Mixin=ColorMixin` |

### GetEventInfo

```lua
C_EncounterEvents.GetEventInfo(encounterEventID: number) -> encounterEventInfo: EncounterEventInfo
```

Returns information about an encounter event.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetEventList

```lua
C_EncounterEvents.GetEventList() -> encounterEventIDs: number[]
```

Returns a list of all encounter event IDs.

### GetEventSound

```lua
C_EncounterEvents.GetEventSound(encounterEventID: number, trigger: EncounterEventSoundTrigger) -> sound: EncounterEventSoundInfo
```

Returns information on a custom sound file to be played when an encounter event trigger occurs.

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasEventInfo

```lua
C_EncounterEvents.HasEventInfo(encounterEventID: number) -> exists: bool
```

Returns true if an encounter event record with a specified ID exists.

`SecretArguments=AllowedWhenUntainted`

### PlayEventSound

```lua
C_EncounterEvents.PlayEventSound(encounterEventID: number, trigger: EncounterEventSoundTrigger) -> handle: SoundHandle
```

Plays any registered custom sound file for a given encounter event trigger.

`SecretArguments=AllowedWhenUntainted`

### SetEventColor

```lua
C_EncounterEvents.SetEventColor(encounterEventID: number, trigger: EncounterEventColorTrigger, color: colorRGBA?)
```

Sets a custom color override for an encounter event. This can be used to colorize text or timer bars individually.

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `encounterEventID` | `number` |  |
| `trigger` | `EncounterEventColorTrigger` |  |
| `color` | `colorRGBA?` | `Mixin=ColorMixin` |

### SetEventSound

```lua
C_EncounterEvents.SetEventSound(encounterEventID: number, trigger: EncounterEventSoundTrigger, sound: EncounterEventSoundInfo?)
```

Sets a custom sound file to be played when an encounter event trigger occurs.

`SecretArguments=NotAllowed`
