# SimpleFrameScriptObjectConstants

source `interface/addons/blizzard_apidocumentationgenerated/simpleframescriptobjectconstantsdocumentation.lua` (FileDataID 8084346)

## Types

### OnUpdateMode

*Enumeration* · 5 values, 0..4

Access values as `Enum.OnUpdateMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Disabled` | `OnUpdateMode` | = 0; Disable OnUpdate execution. |
| `RunWhenVisible` | `OnUpdateMode` | = 1; Run OnUpdate only while object is visible. |
| `RunWhenVisibleOnce` | `OnUpdateMode` | = 2; Run OnUpdate once while object is visible; resets to Disabled before running. |
| `RunOnce` | `OnUpdateMode` | = 3; Run OnUpdate once regardless of visibility; resets to Disabled before running. |
| `RunAlways` | `OnUpdateMode` | = 4; Run OnUpdate regardless of visibility. |

### ScriptBindingType

*Enumeration* · 3 values, 0..2

Access values as `Enum.ScriptBindingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Postcall` | `ScriptBindingType` | = 2 |
| `Precall` | `ScriptBindingType` | = 0 |
| `Extrinsic` | `ScriptBindingType` | = 1 |

### ScriptObjectAccessRestriction

*Enumeration* · 1 values, 1..1

Access values as `Enum.ScriptObjectAccessRestriction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DenyTaintedAccessWhenAurasAreSecret` | `ScriptObjectAccessRestriction` | = 1; Denies access to this script object from tainted execution while aura information is secret. |

### ScriptObjectMetatable

*Enumeration* · 2 values, 0..1

Access values as `Enum.ScriptObjectMetatable.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Public` | `ScriptObjectMetatable` | = 0 |
| `Forbidden` | `ScriptObjectMetatable` | = 1 |

### ScriptObjectPartition

*Enumeration* · 2 values, 0..1

Access values as `Enum.ScriptObjectPartition.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Public` | `ScriptObjectPartition` | = 0 |
| `Forbidden` | `ScriptObjectPartition` | = 1 |

### ScriptObjectPropagationPath

*Enumeration* · 2 values, 0..1

Access values as `Enum.ScriptObjectPropagationPath.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Hierarchy` | `ScriptObjectPropagationPath` | = 0; Propagation through script object hierarchy relationships, such as parent-child ownership. |
| `Layout` | `ScriptObjectPropagationPath` | = 1; Propagation through layout dependency relationships, such as frames anchored relative to one another. |

## Predicates

Conditions referenced by the flags above.

- `RequiresAssignableScript` *Precondition* (failure mode: Error): Requires that this object permit assignment of scripts of this type. May fail for reasons such as the script type not being supported, or secret aspects blocking assignments.
- `RequiresSupportedScript` *Precondition* (failure mode: ReturnNothing): Requires a valid script type supported by this object. If not supported, functions will return no values.
