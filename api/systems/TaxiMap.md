# TaxiMap

Namespace `C_TaxiMap` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/taximapdocumentation.lua` (FileDataID 4637260)

## Functions

### GetAllTaxiNodes

```lua
C_TaxiMap.GetAllTaxiNodes(uiMapID: number) -> taxiNodes: TaxiNodeInfo[]
```

Returns information on taxi nodes at the current flight master.

`SecretArguments=AllowedWhenUntainted`

### GetTaxiNodesForMap

```lua
C_TaxiMap.GetTaxiNodesForMap(uiMapID: number) -> mapTaxiNodes: MapTaxiNodeInfo[]
```

Returns information on taxi nodes for a given map, without considering the current flight master.

`SecretArguments=AllowedWhenUntainted`

### ShouldMapShowTaxiNodes

```lua
C_TaxiMap.ShouldMapShowTaxiNodes(uiMapID: number) -> shouldShowNodes: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### TAXIMAP_CLOSED

```lua
TAXIMAP_CLOSED()
```

`SynchronousEvent`

### TAXIMAP_OPENED

```lua
TAXIMAP_OPENED(system: number)
```

`SynchronousEvent`

### TAXI_NODE_STATUS_CHANGED

```lua
TAXI_NODE_STATUS_CHANGED()
```

`SynchronousEvent`

## Types

### FlightPathFaction

*Enumeration* · 3 values, 0..2

Access values as `Enum.FlightPathFaction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Neutral` | `FlightPathFaction` | = 0 |
| `Horde` | `FlightPathFaction` | = 1 |
| `Alliance` | `FlightPathFaction` | = 2 |

### FlightPathState

*Enumeration* · 3 values, 0..2

Access values as `Enum.FlightPathState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Current` | `FlightPathState` | = 0 |
| `Reachable` | `FlightPathState` | = 1 |
| `Unreachable` | `FlightPathState` | = 2 |

### MapTaxiNodeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `nodeID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `atlasName` | `cstring` |  |
| `faction` | `FlightPathFaction` |  |
| `textureKit` | `textureKit` |  |
| `isUndiscovered` | `bool` |  |

### TaxiNodeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `nodeID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `state` | `FlightPathState` |  |
| `slotIndex` | `luaIndex` |  |
| `textureKit` | `textureKit` |  |
| `useSpecialIcon` | `bool` |  |
| `specialIconCostString` | `string?` |  |
| `isMapLayerTransition` | `bool` |  |
