# WorldLootObject

Namespace `C_WorldLootObject` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/worldlootobjectdocumentation.lua` (FileDataID 5500607)

## Functions

### DoesSlotMatchInventoryType

```lua
C_WorldLootObject.DoesSlotMatchInventoryType(slot: number, inventoryType: InventoryType) -> matches: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetWorldLootObjectDistanceSquared

```lua
C_WorldLootObject.GetWorldLootObjectDistanceSquared(unitToken: UnitToken) -> distanceSquared: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetWorldLootObjectInfo

```lua
C_WorldLootObject.GetWorldLootObjectInfo(unitToken: UnitToken) -> info: WorldLootObjectInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetWorldLootObjectInfoByGUID

```lua
C_WorldLootObject.GetWorldLootObjectInfoByGUID(objectGUID: WOWGUID) -> info: WorldLootObjectInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### IsWorldLootObject

```lua
C_WorldLootObject.IsWorldLootObject(unitToken: UnitToken) -> isWorldLootObject: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsWorldLootObjectByGUID

```lua
C_WorldLootObject.IsWorldLootObjectByGUID(guid: WOWGUID) -> isWorldLootObject: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsWorldLootObjectInRange

```lua
C_WorldLootObject.IsWorldLootObjectInRange(unitToken: UnitToken) -> isWorldLootObjectInRange: bool
```

`SecretArguments=AllowedWhenUntainted`

### OnWorldLootObjectClick

```lua
C_WorldLootObject.OnWorldLootObjectClick(unitToken: UnitToken, isLeftClick: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### WORLD_LOOT_OBJECT_INFO_UPDATED

```lua
WORLD_LOOT_OBJECT_INFO_UPDATED(guid: WOWGUID)
```

`SynchronousEvent`

## Types

### WorldLootObjectInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `inventoryType` | `InventoryType` |  |
| `atMaxQuality` | `bool` |  |
| `isUpgrade` | `bool` |  |
