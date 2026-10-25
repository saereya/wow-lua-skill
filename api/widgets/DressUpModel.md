# DressUpModel

Widget methods (`FrameAPIDressUpModel`) · inherits [`PlayerModel`](PlayerModel.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapidressupmodeldocumentation.lua` (FileDataID 5203720)

## Methods

### Dress

```lua
DressUpModel:Dress()
```

### GetAutoDress

```lua
DressUpModel:GetAutoDress() -> enabled: bool
```

### GetItemTransmogInfo

```lua
DressUpModel:GetItemTransmogInfo(inventorySlot: luaIndex) -> itemTransmogInfo: ItemTransmogInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemTransmogInfo` | `ItemTransmogInfo` | `Mixin=ItemTransmogInfoMixin` |

### GetItemTransmogInfoList

```lua
DressUpModel:GetItemTransmogInfoList() -> infoList: ItemTransmogInfo[]
```

### GetObeyHideInTransmogFlag

```lua
DressUpModel:GetObeyHideInTransmogFlag() -> enabled: bool
```

### GetSheathed

```lua
DressUpModel:GetSheathed() -> sheathed: bool
```

### GetUseTransmogChoices

```lua
DressUpModel:GetUseTransmogChoices() -> enabled: bool
```

### GetUseTransmogSkin

```lua
DressUpModel:GetUseTransmogSkin() -> enabled: bool
```

### IsGeoReady

```lua
DressUpModel:IsGeoReady() -> ready: bool
```

### IsSlotAllowed

```lua
DressUpModel:IsSlotAllowed(slot: luaIndex) -> allowed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSlotVisible

```lua
DressUpModel:IsSlotVisible(slot: luaIndex) -> visible: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetAutoDress

```lua
DressUpModel:SetAutoDress(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetItemTransmogInfo

```lua
DressUpModel:SetItemTransmogInfo(itemTransmogInfo: ItemTransmogInfo, inventorySlot: luaIndex?, ignoreChildItems: bool) -> result: ItemTryOnReason
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `itemTransmogInfo` | `ItemTransmogInfo` | `Mixin=ItemTransmogInfoMixin` |
| `inventorySlot` | `luaIndex?` |  |
| `ignoreChildItems` | `bool` | default `false` |

### SetObeyHideInTransmogFlag

```lua
DressUpModel:SetObeyHideInTransmogFlag(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetSheathed

```lua
DressUpModel:SetSheathed(sheathed: bool, hideWeapons: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `sheathed` | `bool` | default `false` |
| `hideWeapons` | `bool` | default `false` |

### SetUseTransmogChoices

```lua
DressUpModel:SetUseTransmogChoices(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetUseTransmogSkin

```lua
DressUpModel:SetUseTransmogSkin(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### TryOn

```lua
DressUpModel:TryOn(linkOrItemModifiedAppearanceID: IDOrLink, handSlotName: cstring?, spellEnchantID: number?) -> result: ItemTryOnReason?
```

`SecretArguments=AllowedWhenUntainted`

### Undress

```lua
DressUpModel:Undress()
```

### UndressSlot

```lua
DressUpModel:UndressSlot(inventorySlot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`
