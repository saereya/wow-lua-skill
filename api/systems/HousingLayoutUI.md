# HousingLayoutUI

Namespace `C_HousingLayout` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housinglayoutuidocumentation.lua` (FileDataID 5503356)

## Functions

### AnyRoomsOnFloor

```lua
C_HousingLayout.AnyRoomsOnFloor(floor: number) -> anyRooms: bool
```

`SecretArguments=AllowedWhenUntainted`

### CancelActiveLayoutEditing

```lua
C_HousingLayout.CancelActiveLayoutEditing()
```

### CanSetViewedFloor

```lua
C_HousingLayout.CanSetViewedFloor(floor: number) -> canSet: bool
```

`SecretArguments=AllowedWhenUntainted`

### ConfirmStairChoice

```lua
C_HousingLayout.ConfirmStairChoice(choice: HousingLayoutStairDirection?)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `choice` | `HousingLayoutStairDirection?` | If not set, the pending stair operation will be cancelled |

### DeselectFloorplan

```lua
C_HousingLayout.DeselectFloorplan()
```

### DeselectRoomOrDoor

```lua
C_HousingLayout.DeselectRoomOrDoor()
```

### GetBaseRoomFloor

```lua
C_HousingLayout.GetBaseRoomFloor() -> floor: number
```

### GetHighestOccupiedFloorIndex

```lua
C_HousingLayout.GetHighestOccupiedFloorIndex() -> highestFloorIndex: number
```

### GetLowestOccupiedFloorIndex

```lua
C_HousingLayout.GetLowestOccupiedFloorIndex() -> lowestFloorIndex: number
```

### GetNumActiveRooms

```lua
C_HousingLayout.GetNumActiveRooms() -> numRooms: number
```

### GetRoomPlacementBudget

```lua
C_HousingLayout.GetRoomPlacementBudget() -> placementBudget: number?
```

Returns the max room placement budget for the current owned house's interior; Can be increased via house level

Returns:

| Name | Type | Notes |
|---|---|---|
| `placementBudget` | `number?` | Will be nil if not in an owned House or Plot |

### GetRoomPlayerIsIn

```lua
C_HousingLayout.GetRoomPlayerIsIn() -> roomGUID: WOWGUID
```

Returns the guid of the interior room the player is standing in, or nil if not currently standing in one

`MayReturnNothing`

### GetSelectedBlueprintFloorplan

```lua
C_HousingLayout.GetSelectedBlueprintFloorplan() -> roomID: number, shareCode: cstring
```

`MayReturnNothing`

### GetSelectedDoor

```lua
C_HousingLayout.GetSelectedDoor() -> selectedDoorComponentID: number, roomGUID: WOWGUID
```

If a door is selected, returns its component id and the guid of the room it belongs to; Otherwise returns nothing

`MayReturnNothing`

### GetSelectedFloorplan

```lua
C_HousingLayout.GetSelectedFloorplan() -> roomID: number?
```

### GetSelectedRoom

```lua
C_HousingLayout.GetSelectedRoom() -> roomGUID: WOWGUID
```

If a Room is selected, returns the room's guid; Otherwise returns nothing

`MayReturnNothing`

### GetSelectedStairwellRoomCount

```lua
C_HousingLayout.GetSelectedStairwellRoomCount() -> stairwellRoomCount: number
```

### GetSpentPlacementBudget

```lua
C_HousingLayout.GetSpentPlacementBudget() -> spentPlacementBudget: number?
```

Returns how much of the current owned house's room placement budget has been spent; Different kinds of rooms take up different budget amounts, so this value isn't an individual room count, see GetNumActiveRooms for that

Returns:

| Name | Type | Notes |
|---|---|---|
| `spentPlacementBudget` | `number?` | Will be nil if not in an owned House |

### GetViewedFloor

```lua
C_HousingLayout.GetViewedFloor() -> floor: number
```

### HasAnySelections

```lua
C_HousingLayout.HasAnySelections() -> hasAnySelections: bool
```

Returns true if any room, door, or floorplan is currently selected or being dragged

### HasRoomPlacementBudget

```lua
C_HousingLayout.HasRoomPlacementBudget() -> hasBudget: bool
```

Returns whether there's a max room placement budget available and active for the current player, in the current house's interior

### HasSelectedBlueprintFloorplan

```lua
C_HousingLayout.HasSelectedBlueprintFloorplan() -> hasSelectedBlueprintFloorplan: bool
```

### HasSelectedDoor

```lua
C_HousingLayout.HasSelectedDoor() -> hasSelectedDoor: bool
```

Returns true if a door component is currently selected

### HasSelectedFloorplan

```lua
C_HousingLayout.HasSelectedFloorplan() -> hasSelectedFloorplan: bool
```

### HasSelectedRoom

```lua
C_HousingLayout.HasSelectedRoom() -> hasSelectedRoom: bool
```

Returns true if a room is selected, will NOT return true if a door is selected

### HasStairs

```lua
C_HousingLayout.HasStairs(roomRecordID: number) -> hasStairs: bool
```

`SecretArguments=AllowedWhenUntainted`

### HasValidConnection

```lua
C_HousingLayout.HasValidConnection(roomGUID: WOWGUID, componentID: number, roomId: number) -> canPlace: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsBaseRoom

```lua
C_HousingLayout.IsBaseRoom(roomGUID: WOWGUID) -> isBaseRoom: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsDraggingRoom

```lua
C_HousingLayout.IsDraggingRoom() -> isDragging: bool, isAccessibleDrag: bool
```

### MoveDraggedRoom

```lua
C_HousingLayout.MoveDraggedRoom(sourceDoorIndex: number, destRoom: WOWGUID, destDoorIndex: number)
```

Attempt to move the room currently being dragged to a specific connection point on a specific other room

`SecretArguments=AllowedWhenUntainted`

### MoveLayoutCamera

```lua
C_HousingLayout.MoveLayoutCamera(direction: HousingLayoutCameraDirection, isPressed: bool)
```

`SecretArguments=AllowedWhenUntainted`

### RemoveRoom

```lua
C_HousingLayout.RemoveRoom(roomGUID: WOWGUID)
```

Attempt to return a previously placed room to the House Chest

`SecretArguments=AllowedWhenUntainted`

### RoomHasStairs

```lua
C_HousingLayout.RoomHasStairs(roomGUID: WOWGUID) -> hasStairs: bool
```

Returns true of the provided roomGUID is a stairwell. Returns false if roomGUID is invalid

`SecretArguments=AllowedWhenUntainted`

### RotateFocusedRoom

```lua
C_HousingLayout.RotateFocusedRoom(isLeft: bool)
```

Rotates either the currently dragged or currently selected room, if either exist

`SecretArguments=AllowedWhenUntainted`

### RotateRoom

```lua
C_HousingLayout.RotateRoom(roomGUID: WOWGUID, isLeft: bool)
```

Attempt to rotate an already placed room

`SecretArguments=AllowedWhenUntainted`

### SelectFloorplan

```lua
C_HousingLayout.SelectFloorplan(roomID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetViewedFloor

```lua
C_HousingLayout.SetViewedFloor(floor: number)
```

`SecretArguments=AllowedWhenUntainted`

### StartDrag

```lua
C_HousingLayout.StartDrag()
```

### StopDrag

```lua
C_HousingLayout.StopDrag()
```

### StopDraggingRoom

```lua
C_HousingLayout.StopDraggingRoom()
```

### ZoomLayoutCamera

```lua
C_HousingLayout.ZoomLayoutCamera(zoomIn: bool) -> zoomChanged: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### HOUSING_LAYOUT_DOOR_SELECTED

```lua
HOUSING_LAYOUT_DOOR_SELECTED(roomGUID: WOWGUID, componentID: number)
```

Fired when one of the door nodes of an already placed room has been selected

`SynchronousEvent`

### HOUSING_LAYOUT_DOOR_SELECTION_CHANGED

```lua
HOUSING_LAYOUT_DOOR_SELECTION_CHANGED(hasSelection: bool)
```

Fired when one of the door nodes of an already placed room has been selected or deselected

`SynchronousEvent`

### HOUSING_LAYOUT_DRAG_TARGET_CHANGED

```lua
HOUSING_LAYOUT_DRAG_TARGET_CHANGED(isDraggingRoom: bool)
```

Fired when an already placed room has either started or stopped being dragged

`SynchronousEvent`

### HOUSING_LAYOUT_FLOORPLAN_SELECTION_CHANGED

```lua
HOUSING_LAYOUT_FLOORPLAN_SELECTION_CHANGED(hasSelection: bool, roomID: number, blueprintShareCode: cstring?)
```

Fired when a room option in the House Chest has been selected or deselected

`SynchronousEvent`

### HOUSING_LAYOUT_OCCUPIED_FLOOR_RANGE_CHANGED

```lua
HOUSING_LAYOUT_OCCUPIED_FLOOR_RANGE_CHANGED(lowestFloor: number, highestFloor: number)
```

`SynchronousEvent`

### HOUSING_LAYOUT_PIN_FRAME_ADDED

```lua
HOUSING_LAYOUT_PIN_FRAME_ADDED(pinFrame: HousingLayoutPinFrame)
```

`SynchronousEvent`

### HOUSING_LAYOUT_PIN_FRAME_RELEASED

```lua
HOUSING_LAYOUT_PIN_FRAME_RELEASED(pinFrame: HousingLayoutPinFrame)
```

`SynchronousEvent`

### HOUSING_LAYOUT_PIN_FRAMES_RELEASED

```lua
HOUSING_LAYOUT_PIN_FRAMES_RELEASED()
```

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_COMPONENT_THEME_SET_CHANGED

```lua
HOUSING_LAYOUT_ROOM_COMPONENT_THEME_SET_CHANGED(roomGUID: WOWGUID, componentID: number, newThemeSet: number, result: HousingResult)
```

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_MOVED

```lua
HOUSING_LAYOUT_ROOM_MOVED()
```

Fired when a previously placed room has been moved to a different position or rotation

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_MOVE_INVALID

```lua
HOUSING_LAYOUT_ROOM_MOVE_INVALID()
```

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_RECEIVED

```lua
HOUSING_LAYOUT_ROOM_RECEIVED(playAddedSound: bool)
```

Fired when info for a newly placed room has been recieved while in Layout Mode

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_REMOVED

```lua
HOUSING_LAYOUT_ROOM_REMOVED()
```

Fired when a previously placed room has been removed while in Layout Mode

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_RETURNED

```lua
HOUSING_LAYOUT_ROOM_RETURNED()
```

Fired when a room that was being dragged is let go of without being placed, and is returned to the House Chest

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_SELECTION_CHANGED

```lua
HOUSING_LAYOUT_ROOM_SELECTION_CHANGED(hasSelection: bool)
```

Fired when an already placed room has been selected or deselected

`SynchronousEvent`

### HOUSING_LAYOUT_ROOM_SNAPPED

```lua
HOUSING_LAYOUT_ROOM_SNAPPED()
```

Fired when a room being dragged has been snapped to a particular door connection

`SynchronousEvent`

### HOUSING_LAYOUT_VIEWED_FLOOR_CHANGED

```lua
HOUSING_LAYOUT_VIEWED_FLOOR_CHANGED(floor: number)
```

`SynchronousEvent`

### SHOW_STAIR_DIRECTION_CONFIRMATION

```lua
SHOW_STAIR_DIRECTION_CONFIRMATION()
```

`SynchronousEvent`
