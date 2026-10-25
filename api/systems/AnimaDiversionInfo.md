# AnimaDiversionInfo

Namespace `C_AnimaDiversion` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/animadiversionuidocumentation.lua` (FileDataID 4637011)

## Functions

### CloseUI

```lua
C_AnimaDiversion.CloseUI()
```

### GetAnimaDiversionNodes

```lua
C_AnimaDiversion.GetAnimaDiversionNodes() -> animaNodes: AnimaDiversionNodeInfo[]
```

`MayReturnNothing`

### GetOriginPosition

```lua
C_AnimaDiversion.GetOriginPosition() -> normalizedPosition: vector2?
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `normalizedPosition` | `vector2?` | `Mixin=Vector2DMixin` |

### GetReinforceProgress

```lua
C_AnimaDiversion.GetReinforceProgress() -> progress: number
```

### GetTextureKit

```lua
C_AnimaDiversion.GetTextureKit() -> textureKit: textureKit
```

### OpenAnimaDiversionUI

```lua
C_AnimaDiversion.OpenAnimaDiversionUI()
```

### SelectAnimaNode

```lua
C_AnimaDiversion.SelectAnimaNode(talentID: number, temporary: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### ANIMA_DIVERSION_CLOSE

```lua
ANIMA_DIVERSION_CLOSE()
```

`SynchronousEvent`

### ANIMA_DIVERSION_OPEN

```lua
ANIMA_DIVERSION_OPEN(info: AnimaDiversionFrameInfo)
```

`SynchronousEvent`

### ANIMA_DIVERSION_TALENT_UPDATED

```lua
ANIMA_DIVERSION_TALENT_UPDATED()
```

`SynchronousEvent`

## Types

### AnimaDiversionNodeState

*Enumeration* · 5 values, 0..4

Access values as `Enum.AnimaDiversionNodeState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unavailable` | `AnimaDiversionNodeState` | = 0 |
| `Available` | `AnimaDiversionNodeState` | = 1 |
| `SelectedTemporary` | `AnimaDiversionNodeState` | = 2 |
| `SelectedPermanent` | `AnimaDiversionNodeState` | = 3 |
| `Cooldown` | `AnimaDiversionNodeState` | = 4 |

### AnimaDiversionCostInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `currencyID` | `number` |  |
| `quantity` | `number` |  |

### AnimaDiversionFrameInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `title` | `string` |  |
| `mapID` | `number` |  |

### AnimaDiversionNodeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `talentID` | `number` |  |
| `name` | `string` |  |
| `description` | `string` |  |
| `costs` | `AnimaDiversionCostInfo[]` |  |
| `currencyID` | `number` |  |
| `icon` | `number` |  |
| `normalizedPosition` | `vector2` | `Mixin=Vector2DMixin` |
| `state` | `AnimaDiversionNodeState` |  |
