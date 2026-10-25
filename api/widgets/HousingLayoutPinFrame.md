# HousingLayoutPinFrame

Widget methods (`HousingLayoutPinFrameAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housinglayoutpinframeapidocumentation.lua` (FileDataID 5503355)

## Methods

### CanMove

```lua
HousingLayoutPinFrame:CanMove() -> moveRestriction: HousingLayoutRestriction
```

### CanRemove

```lua
HousingLayoutPinFrame:CanRemove() -> removalRestriction: HousingLayoutRestriction
```

### CanRotate

```lua
HousingLayoutPinFrame:CanRotate() -> rotateRestriction: HousingLayoutRestriction
```

### Drag

```lua
HousingLayoutPinFrame:Drag(isAccessible: bool)
```

`SecretArguments=AllowedWhenUntainted`

### GetDoorConnectionInfo

```lua
HousingLayoutPinFrame:GetDoorConnectionInfo() -> connectionInfo: DoorConnectionInfo?
```

### GetPinType

```lua
HousingLayoutPinFrame:GetPinType() -> type: HousingLayoutPinType
```

### GetRoomGUID

```lua
HousingLayoutPinFrame:GetRoomGUID() -> roomGUID: WOWGUID
```

### GetRoomName

```lua
HousingLayoutPinFrame:GetRoomName() -> name: cstring?
```

### IsAnyPartOfRoomSelected

```lua
HousingLayoutPinFrame:IsAnyPartOfRoomSelected() -> isSelected: bool
```

Returns true if this pin's associated room, or anything attached to it, is selected. Ex: If pin is for a door, returns true if its room, or any other doors on that room, are selected

### IsConnectedToDraggingRoom

```lua
HousingLayoutPinFrame:IsConnectedToDraggingRoom() -> isConnectedToDraggingRoom: bool
```

### IsOccupiedDoor

```lua
HousingLayoutPinFrame:IsOccupiedDoor() -> isOccupied: bool?
```

Will be nil if pin is not a Door

### IsPartOfDraggingRoom

```lua
HousingLayoutPinFrame:IsPartOfDraggingRoom() -> isPartOfDraggingRoom: bool
```

### IsSelected

```lua
HousingLayoutPinFrame:IsSelected() -> isSelected: bool
```

Returns true if this pin's object is itself selected; See IsAnyPartOfRoomSelected for a broader Selected check

### IsValid

```lua
HousingLayoutPinFrame:IsValid() -> isValid: bool
```

### IsValidForSelectedFloorplan

```lua
HousingLayoutPinFrame:IsValidForSelectedFloorplan() -> isValid: bool
```

### Select

```lua
HousingLayoutPinFrame:Select()
```

### SetUpdateCallback

```lua
HousingLayoutPinFrame:SetUpdateCallback(cb: PinUpdatedCallback)
```

`SecretArguments=AllowedWhenUntainted`
