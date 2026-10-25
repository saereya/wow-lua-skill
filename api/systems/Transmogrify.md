# Transmogrify

Namespace `C_Transmog` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/transmogdocumentation.lua` (FileDataID 4637270)

## Functions

### CanHaveSecondaryAppearanceForSlotID

```lua
C_Transmog.CanHaveSecondaryAppearanceForSlotID(slotID: luaIndex) -> canHaveSecondaryAppearance: bool
```

`SecretArguments=AllowedWhenUntainted`

### ExtractTransmogIDList

```lua
C_Transmog.ExtractTransmogIDList(input: cstring) -> transmogIDList: number[]
```

`SecretArguments=AllowedWhenUntainted`

### GetAllSetAppearancesByID

```lua
C_Transmog.GetAllSetAppearancesByID(setID: number) -> setItems: TransmogSetItemInfo[]?
```

`SecretArguments=AllowedWhenUntainted`

### GetItemIDForSource

```lua
C_Transmog.GetItemIDForSource(itemModifiedAppearanceID: number) -> itemID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSlotForInventoryType

```lua
C_Transmog.GetSlotForInventoryType(inventoryType: luaIndex) -> slot: luaIndex
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetSlotVisualInfo

```lua
C_Transmog.GetSlotVisualInfo(transmogLocation: TransmogLocation) -> slotVisualInfo: TransmogSlotVisualInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `transmogLocation` | `TransmogLocation` | `Mixin=TransmogLocationMixin` |

### IsAtTransmogNPC

```lua
C_Transmog.IsAtTransmogNPC() -> isAtNPC: bool
```

## Events

### TRANSMOG_COLLECTION_CAMERA_UPDATE

```lua
TRANSMOG_COLLECTION_CAMERA_UPDATE()
```

`SynchronousEvent`

### TRANSMOG_COLLECTION_ITEM_FAVORITE_UPDATE

```lua
TRANSMOG_COLLECTION_ITEM_FAVORITE_UPDATE(itemAppearanceID: number, isFavorite: bool)
```

`SynchronousEvent`

### TRANSMOG_COLLECTION_ITEM_UPDATE

```lua
TRANSMOG_COLLECTION_ITEM_UPDATE()
```

`UniqueEvent`

### TRANSMOG_COLLECTION_SOURCE_ADDED

```lua
TRANSMOG_COLLECTION_SOURCE_ADDED(itemModifiedAppearanceID: number)
```

`SynchronousEvent`

### TRANSMOG_COLLECTION_SOURCE_REMOVED

```lua
TRANSMOG_COLLECTION_SOURCE_REMOVED(itemModifiedAppearanceID: number)
```

`SynchronousEvent`

### TRANSMOG_COLLECTION_UPDATED

```lua
TRANSMOG_COLLECTION_UPDATED(collectionIndex: luaIndex?, modID: number?, itemAppearanceID: number?, reason: cstring?)
```

`SynchronousEvent` `UniqueEvent`

### TRANSMOG_COSMETIC_COLLECTION_SOURCE_ADDED

```lua
TRANSMOG_COSMETIC_COLLECTION_SOURCE_ADDED(itemModifiedAppearanceID: number)
```

`SynchronousEvent`

### TRANSMOGRIFY_CLOSE

```lua
TRANSMOGRIFY_CLOSE()
```

`SynchronousEvent`

### TRANSMOGRIFY_ITEM_UPDATE

```lua
TRANSMOGRIFY_ITEM_UPDATE()
```

`UniqueEvent`

### TRANSMOGRIFY_OPEN

```lua
TRANSMOGRIFY_OPEN()
```

`SynchronousEvent`

### TRANSMOGRIFY_SUCCESS

```lua
TRANSMOGRIFY_SUCCESS(transmogLocation: TransmogLocation)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `transmogLocation` | `TransmogLocation` | `Mixin=TransmogLocationMixin` |

### TRANSMOGRIFY_UPDATE

```lua
TRANSMOGRIFY_UPDATE(transmogLocation: TransmogLocation?, action: cstring?)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `transmogLocation` | `TransmogLocation?` | `Mixin=TransmogLocationMixin` |
| `action` | `cstring?` |  |

### TRANSMOG_SEARCH_UPDATED

```lua
TRANSMOG_SEARCH_UPDATED(searchType: TransmogSearchType, collectionType: TransmogCollectionType?)
```

`SynchronousEvent`

### TRANSMOG_SETS_UPDATE_FAVORITE

```lua
TRANSMOG_SETS_UPDATE_FAVORITE()
```

`SynchronousEvent`

### TRANSMOG_SOURCE_COLLECTABILITY_UPDATE

```lua
TRANSMOG_SOURCE_COLLECTABILITY_UPDATE(itemModifiedAppearanceID: number, collectable: bool)
```

`SynchronousEvent`

## Types

### TransmogPendingType

*Enumeration* · 4 values, 0..3

Access values as `Enum.TransmogPendingType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Apply` | `TransmogPendingType` | = 0 |
| `Revert` | `TransmogPendingType` | = 1 |
| `ToggleOn` | `TransmogPendingType` | = 2 |
| `ToggleOff` | `TransmogPendingType` | = 3 |

### TransmogApplyWarningInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemLink` | `string` |  |
| `text` | `string` |  |

### TransmogSetItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `itemID` | `number` |  |
| `itemModifiedAppearanceID` | `number` |  |
| `invSlot` | `number` |  |
| `invType` | `string` |  |

### TransmogSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isTransmogrified` | `bool` |  |
| `hasPending` | `bool` |  |
| `isPendingCollected` | `bool` |  |
| `canTransmogrify` | `bool` |  |
| `cannotTransmogrifyReason` | `number` |  |
| `hasUndo` | `bool` |  |
| `isHideVisual` | `bool` |  |
| `texture` | `fileID?` |  |

### TransmogSlotVisualInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `baseSourceID` | `number` |  |
| `baseVisualID` | `number` |  |
| `appliedSourceID` | `number` |  |
| `appliedVisualID` | `number` |  |
| `pendingSourceID` | `number` |  |
| `pendingVisualID` | `number` |  |
| `hasUndo` | `bool` |  |
| `isHideVisual` | `bool` |  |
| `itemSubclass` | `number` |  |
