# TimedSignalMapShared

source `interface/addons/blizzard_apidocumentationgenerated/timedsignalmapshareddocumentation.lua` (FileDataID 8312418)

## Types

### TimedSignalMapEntry

*Structure*

Structure associating a key with a scheduled time.

Fields:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | The key that has been scheduled. |
| `time` | `FrameTime` | Absolute time, on the same clock as GetTime(), at which the key is scheduled to signal. |

### TimedSignalMapCallback

*CallbackType*

Invoked by a timed signal map when a scheduled time has arrived.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | The key whose scheduled time has arrived; secret if the timed signal map has secret values.; `ConditionalSecret` |

## Predicates

Conditions referenced by the flags above.

- `RequiresTimedSignalMapAccess` *Precondition* (failure mode: Error): Guarded APIs on a timed signal map raise an error when the map holds secret values and is accessed from a tainted execution context.
