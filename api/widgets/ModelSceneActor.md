# ModelSceneActor

Widget methods (`FrameAPIModelSceneFrameActor`) · inherits [`ModelSceneActorBase`](ModelSceneActorBase.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapimodelsceneframeactordocumentation.lua` (FileDataID 5264242)

## Methods

### AttachToMount

```lua
ModelSceneActor:AttachToMount(rider: ModelSceneFrameActor, animation: AnimationDataEnum, spellKitVisualID: number?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### CalculateMountScale

```lua
ModelSceneActor:CalculateMountScale(rider: ModelSceneFrameActor) -> scale: number
```

`SecretArguments=AllowedWhenUntainted`

### DetachFromMount

```lua
ModelSceneActor:DetachFromMount(rider: ModelSceneFrameActor) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### Dress

```lua
ModelSceneActor:Dress()
```

### DressPlayerSlot

```lua
ModelSceneActor:DressPlayerSlot(invSlot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoDress

```lua
ModelSceneActor:GetAutoDress() -> autoDress: bool
```

### GetItemTransmogInfo

```lua
ModelSceneActor:GetItemTransmogInfo(inventorySlots: number) -> itemTransmogInfo: ItemTransmogInfo?
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `itemTransmogInfo` | `ItemTransmogInfo?` | `Mixin=ItemTransmogInfoMixin` |

### GetItemTransmogInfoList

```lua
ModelSceneActor:GetItemTransmogInfoList() -> infoList: ItemTransmogInfo[]
```

### GetObeyHideInTransmogFlag

```lua
ModelSceneActor:GetObeyHideInTransmogFlag() -> obey: bool
```

### GetPaused

```lua
ModelSceneActor:GetPaused() -> paused: bool, globalPaused: bool
```

### GetSheathed

```lua
ModelSceneActor:GetSheathed() -> sheathed: bool
```

### GetUseTransmogChoices

```lua
ModelSceneActor:GetUseTransmogChoices() -> use: bool
```

### GetUseTransmogSkin

```lua
ModelSceneActor:GetUseTransmogSkin() -> use: bool
```

### IsGeoReady

```lua
ModelSceneActor:IsGeoReady() -> isReady: bool
```

### IsSlotAllowed

```lua
ModelSceneActor:IsSlotAllowed(inventorySlots: number) -> allowed: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsSlotVisible

```lua
ModelSceneActor:IsSlotVisible(inventorySlots: number) -> visible: bool
```

`SecretArguments=AllowedWhenUntainted`

### ReleaseFrontEndCharacterDisplays

```lua
ModelSceneActor:ReleaseFrontEndCharacterDisplays() -> success: bool
```

### ResetNextHandSlot

```lua
ModelSceneActor:ResetNextHandSlot()
```

### SetAutoDress

```lua
ModelSceneActor:SetAutoDress(autoDress: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetFrontEndLobbyModelFromDefaultCharacterDisplay

```lua
ModelSceneActor:SetFrontEndLobbyModelFromDefaultCharacterDisplay(characterIndex: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetItemTransmogInfo

```lua
ModelSceneActor:SetItemTransmogInfo(transmogInfo: ItemTransmogInfo, inventorySlots: number?, ignoreChildItems: bool) -> result: ItemTryOnReason
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `transmogInfo` | `ItemTransmogInfo` | `Mixin=ItemTransmogInfoMixin` |
| `inventorySlots` | `number?` |  |
| `ignoreChildItems` | `bool` | default `false` |

### SetModelByHyperlink

```lua
ModelSceneActor:SetModelByHyperlink(link: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetObeyHideInTransmogFlag

```lua
ModelSceneActor:SetObeyHideInTransmogFlag(obey: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPaused

```lua
ModelSceneActor:SetPaused(paused: bool, affectsGlobalPause: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `paused` | `bool` |  |
| `affectsGlobalPause` | `bool` | default `true` |

### SetSheathed

```lua
ModelSceneActor:SetSheathed(sheathed: bool, hidden: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `sheathed` | `bool` |  |
| `hidden` | `bool` | default `false` |

### SetSheathedCategory

```lua
ModelSceneActor:SetSheathedCategory(inventorySlots: number, category: TransmogOutfitSlotOptionSheatheCategory)
```

`SecretArguments=AllowedWhenUntainted`

### SetUseTransmogChoices

```lua
ModelSceneActor:SetUseTransmogChoices(use: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetUseTransmogSkin

```lua
ModelSceneActor:SetUseTransmogSkin(use: bool)
```

`SecretArguments=AllowedWhenUntainted`

### Undress

```lua
ModelSceneActor:Undress(includeWeapons: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `includeWeapons` | `bool` | default `true` |

### UndressSlot

```lua
ModelSceneActor:UndressSlot(inventorySlots: number)
```

`SecretArguments=AllowedWhenUntainted`

### UseUnitSheatheCategory

```lua
ModelSceneActor:UseUnitSheatheCategory(useCategory: bool)
```

`SecretArguments=AllowedWhenUntainted`
