# HousingLayoutUITypes

source `interface/addons/blizzard_apidocumentationgenerated/housinglayoutuitypesdocumentation.lua` (FileDataID 5503354)

## Types

### HousingLayoutCameraDirection

*Enumeration* · 5 values, 0..8

Access values as `Enum.HousingLayoutCameraDirection.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingLayoutCameraDirection` | = 0 |
| `Up` | `HousingLayoutCameraDirection` | = 1 |
| `Down` | `HousingLayoutCameraDirection` | = 2 |
| `Left` | `HousingLayoutCameraDirection` | = 4 |
| `Right` | `HousingLayoutCameraDirection` | = 8 |

### HousingLayoutPinType

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingLayoutPinType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Door` | `HousingLayoutPinType` | = 0 |
| `Room` | `HousingLayoutPinType` | = 1 |

### HousingLayoutStairDirection

*Enumeration* · 2 values, 0..1

Access values as `Enum.HousingLayoutStairDirection.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Up` | `HousingLayoutStairDirection` | = 0 |
| `Down` | `HousingLayoutStairDirection` | = 1 |

### DoorConnectionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `doorID` | `number` |  |
| `connectionType` | `HousingRoomComponentType` |  |
| `doorFacing` | `number` |  |

### RoomOptionInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `roomName` | `cstring` |  |
| `roomID` | `number` |  |
| `learned` | `bool` |  |
| `numOwned` | `number` |  |

### PinUpdatedCallback

*CallbackType*
