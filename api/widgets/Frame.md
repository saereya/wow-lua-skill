# Frame

Widget methods (`SimpleFrameAPI`) · inherits [`ScriptRegion`](ScriptRegion.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleframeapidocumentation.lua` (FileDataID 4637218)

## Methods

### AbortDrag

```lua
Frame:AbortDrag()
```

### AddRoleset

```lua
Frame:AddRoleset(roleset: string)
```

Adds a roleset tag to this frame without removing existing ones.

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### CanChangeAttribute

```lua
Frame:CanChangeAttribute() -> canChangeAttributes: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### ClearAlphaGradient

```lua
Frame:ClearAlphaGradient()
```

### ClearAttribute

```lua
Frame:ClearAttribute(attributeName: cstring) -> cleared: bool
```

`SecretArguments=NotAllowed` `IsProtectedFunction` `SecretReturnsForAspect={ Enum.SecretAspect.Attributes }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### ClearAttributes

```lua
Frame:ClearAttributes()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### CreateFontString

```lua
Frame:CreateFontString(name: cstring?, drawLayer: DrawLayer?, templateName: cstring?) -> line: SimpleFontString
```

`SecretArguments=NotAllowed`

### CreateLine

```lua
Frame:CreateLine(name: cstring?, drawLayer: DrawLayer?, templateName: cstring?, subLevel: number?) -> line: SimpleLine
```

`SecretArguments=NotAllowed`

### CreateMaskTexture

```lua
Frame:CreateMaskTexture(name: cstring?, drawLayer: DrawLayer?, templateName: cstring?, subLevel: number?) -> maskTexture: SimpleMaskTexture
```

`SecretArguments=NotAllowed`

### CreateTexture

```lua
Frame:CreateTexture(name: cstring?, drawLayer: DrawLayer?, templateName: cstring?, subLevel: number?) -> texture: SimpleTexture
```

`SecretArguments=NotAllowed`

### CreateVectorGraphics

```lua
Frame:CreateVectorGraphics(name: cstring?, drawLayer: DrawLayer?, templateName: cstring?, subLevel: number?) -> vectorGraphics: SimpleVectorGraphics
```

`SecretArguments=NotAllowed`

### DesaturateHierarchy

```lua
Frame:DesaturateHierarchy(desaturation: number, excludeRoot: bool)
```

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `desaturation` | `number` |  |
| `excludeRoot` | `bool` | default `false` |

### DisableDrawLayer

```lua
Frame:DisableDrawLayer(layer: DrawLayer)
```

`SecretArguments=AllowedWhenUntainted`

### DoesClipChildren

```lua
Frame:DoesClipChildren() -> clipsChildren: bool
```

### DoesHyperlinkPropagateToParent

```lua
Frame:DoesHyperlinkPropagateToParent() -> canPropagate: bool
```

Returns whether hyperlink events (ex. OnHyperlinkEnter, OnHyperlinkLeave, OnHyperlinkClick) are propagated to this frame's parent.

### EnableDrawLayer

```lua
Frame:EnableDrawLayer(layer: DrawLayer)
```

`SecretArguments=AllowedWhenUntainted`

### EnableGamePadButton

```lua
Frame:EnableGamePadButton(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### EnableGamePadStick

```lua
Frame:EnableGamePadStick(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### EnableKeyboard

```lua
Frame:EnableKeyboard(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### ExecuteAttribute

```lua
Frame:ExecuteAttribute(attributeName: cstring, arguments: cstring?) -> success: bool, returns: cstring?
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.Attributes }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `attributeName` | `cstring` |  |
| `arguments` | `cstring?` | `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `success` | `bool` |  |
| `returns` | `cstring?` | `StrideIndex=1` |

### GetAlpha

```lua
Frame:GetAlpha() -> alpha: SingleColorValue
```

`SecretReturnsForAspect={ Enum.SecretAspect.Alpha }`

### GetAttribute

```lua
Frame:GetAttribute(attributeName: cstring) -> value: cstring
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.Attributes }` `ConstSecretAccessor`

### GetBoundsRect

```lua
Frame:GetBoundsRect() -> left: uiUnit, bottom: uiUnit, width: uiUnit, height: uiUnit
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `left` | `uiUnit` | `ConditionalSecret` |
| `bottom` | `uiUnit` | `ConditionalSecret` |
| `width` | `uiUnit` | `ConditionalSecret` |
| `height` | `uiUnit` | `ConditionalSecret` |

### GetChildren

```lua
Frame:GetChildren() -> children: SimpleFrame
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `children` | `SimpleFrame` | `StrideIndex=1` |

### GetClampRectInsets

```lua
Frame:GetClampRectInsets() -> left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit
```

### GetDontSavePosition

```lua
Frame:GetDontSavePosition() -> dontSave: bool
```

### GetEffectiveAlpha

```lua
Frame:GetEffectiveAlpha() -> effectiveAlpha: SingleColorValue
```

`RequiresScriptObjectAlphaAccess` `SecretReturnsForAspect={ Enum.SecretAspect.Alpha }`

### GetEffectivelyFlattensRenderLayers

```lua
Frame:GetEffectivelyFlattensRenderLayers() -> flatten: bool
```

### GetEffectiveScale

```lua
Frame:GetEffectiveScale() -> effectiveScale: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Scale }`

### GetFlattensRenderLayers

```lua
Frame:GetFlattensRenderLayers() -> flatten: bool
```

### GetFrameLevel

```lua
Frame:GetFrameLevel() -> frameLevel: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.FrameLevel }`

### GetFrameStrata

```lua
Frame:GetFrameStrata() -> strata: FrameStrata
```

`SecretReturnsForAspect={ Enum.SecretAspect.FrameStrata }`

### GetHighestFrameLevel

```lua
Frame:GetHighestFrameLevel(iterateAllChildren: bool) -> frameLevel: number
```

Returns the highest framelevel of the frame and its first order children, or all children if iterateAllChildren is true.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `iterateAllChildren` | `bool` | default `false` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `frameLevel` | `number` | `ConditionalSecret` |

### GetHitRectInsets

```lua
Frame:GetHitRectInsets() -> left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit
```

### GetHyperlinksEnabled

```lua
Frame:GetHyperlinksEnabled() -> enabled: bool
```

### GetID

```lua
Frame:GetID() -> id: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.ID }`

### GetNumChildren

```lua
Frame:GetNumChildren() -> numChildren: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

### GetNumRegions

```lua
Frame:GetNumRegions() -> numRegions: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

### GetOnUpdateMode

```lua
Frame:GetOnUpdateMode() -> onUpdateMode: OnUpdateMode
```

Returns the currently configured OnUpdate script execution mode.

### GetPropagateKeyboardInput

```lua
Frame:GetPropagateKeyboardInput() -> propagate: bool
```

### GetRaisedFrameLevel

```lua
Frame:GetRaisedFrameLevel() -> frameLevel: number
```

### GetRegions

```lua
Frame:GetRegions() -> regions: SimpleRegion
```

`SecretReturnsForAspect={ Enum.SecretAspect.Hierarchy }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `regions` | `SimpleRegion` | `StrideIndex=1` |

### GetResizeBounds

```lua
Frame:GetResizeBounds() -> minWidth: uiUnit, minHeight: uiUnit, maxWidth: uiUnit, maxHeight: uiUnit
```

### GetRolesetNames

```lua
Frame:GetRolesetNames() -> rolesets: string[]
```

Returns the roleset tags assigned to this frame. Returns a list containing 'roleless' if none are assigned.

### GetScale

```lua
Frame:GetScale() -> frameScale: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Scale }`

### GetWindow

```lua
Frame:GetWindow() -> window: SimpleWindow
```

### HasAlphaGradient

```lua
Frame:HasAlphaGradient() -> hasAlphaGradient: bool
```

### HasFixedFrameLevel

```lua
Frame:HasFixedFrameLevel() -> isFixed: bool
```

### HasFixedFrameStrata

```lua
Frame:HasFixedFrameStrata() -> isFixed: bool
```

### Hide

```lua
Frame:Hide()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### InterceptStartDrag

```lua
Frame:InterceptStartDrag(delegate: SimpleFrame) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsClampedToScreen

```lua
Frame:IsClampedToScreen() -> clampedToScreen: bool
```

### IsDrawLayerEnabled

```lua
Frame:IsDrawLayerEnabled(layer: DrawLayer) -> isEnabled: bool
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### IsEventRegistered

```lua
Frame:IsEventRegistered(eventName: cstring) -> isRegistered: bool, units: UnitTokenType?
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Returns:

| Name | Type | Notes |
|---|---|---|
| `isRegistered` | `bool` |  |
| `units` | `UnitTokenType?` | `StrideIndex=1` |

### IsFrameBuffer

```lua
Frame:IsFrameBuffer() -> isFrameBuffer: bool
```

### IsGamePadButtonEnabled

```lua
Frame:IsGamePadButtonEnabled() -> enabled: bool
```

### IsGamePadStickEnabled

```lua
Frame:IsGamePadStickEnabled() -> enabled: bool
```

### IsHighlightLocked

```lua
Frame:IsHighlightLocked() -> locked: bool
```

### IsIgnoringChildrenForBounds

```lua
Frame:IsIgnoringChildrenForBounds() -> ignore: bool
```

### IsIgnoringParentAlpha

```lua
Frame:IsIgnoringParentAlpha() -> ignore: bool
```

### IsIgnoringParentScale

```lua
Frame:IsIgnoringParentScale() -> ignore: bool
```

### IsKeyboardEnabled

```lua
Frame:IsKeyboardEnabled() -> enabled: bool
```

### IsMovable

```lua
Frame:IsMovable() -> isMovable: bool
```

### IsObjectLoaded

```lua
Frame:IsObjectLoaded() -> isLoaded: bool
```

### IsResizable

```lua
Frame:IsResizable() -> resizable: bool
```

### IsRolesetFiltered

```lua
Frame:IsRolesetFiltered() -> isRolesetFiltered: bool
```

Returns whether this frame is hidden because of its rolesets being filtered.

### IsShown

```lua
Frame:IsShown() -> isShown: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.Shown }`

### IsToplevel

```lua
Frame:IsToplevel() -> isTopLevel: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.Toplevel }`

### IsUserPlaced

```lua
Frame:IsUserPlaced() -> isUserPlaced: bool
```

### IsUsingParentLevel

```lua
Frame:IsUsingParentLevel() -> usingParentLevel: bool
```

### IsVisible

```lua
Frame:IsVisible() -> isVisible: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.Shown }`

### LockHighlight

```lua
Frame:LockHighlight()
```

### Lower

```lua
Frame:Lower()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### Raise

```lua
Frame:Raise()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### RegisterAllEvents

```lua
Frame:RegisterAllEvents()
```

### RegisterEvent

```lua
Frame:RegisterEvent(eventName: cstring) -> registered: bool
```

`SecretArguments=AllowedWhenUntainted`

### RegisterEventCallback

```lua
Frame:RegisterEventCallback(eventName: cstring, cb: FrameEventCallbackType) -> registered: bool
```

`SecretArguments=AllowedWhenUntainted`

### RegisterForDrag

```lua
Frame:RegisterForDrag(buttons: MouseButton)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `buttons` | `MouseButton` | `StrideIndex=1` |

### RegisterUnitEvent

```lua
Frame:RegisterUnitEvent(eventName: cstring, units: UnitTokenType) -> registered: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `eventName` | `cstring` |  |
| `units` | `UnitTokenType` | `StrideIndex=1` |

### RegisterUnitEventCallback

```lua
Frame:RegisterUnitEventCallback(eventName: cstring, cb: FrameEventCallbackType, units: UnitTokenType) -> registered: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `eventName` | `cstring` |  |
| `cb` | `FrameEventCallbackType` |  |
| `units` | `UnitTokenType` | `StrideIndex=1` |

### RemoveRoleset

```lua
Frame:RemoveRoleset(roleset: string)
```

Removes a roleset tag from this frame.

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### ResizeToBoundsRect

```lua
Frame:ResizeToBoundsRect()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### RotateTextures

```lua
Frame:RotateTextures(radians: number, x: number, y: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `radians` | `number` |  |
| `x` | `number` | default `0.5` |
| `y` | `number` | default `0.5` |

### SetAlpha

```lua
Frame:SetAlpha(alpha: SingleColorValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Alpha }`

### SetAlphaFromBoolean

```lua
Frame:SetAlphaFromBoolean(value: bool, alphaIfTrue: SingleColorValue, alphaIfFalse: SingleColorValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Alpha }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `bool` |  |
| `alphaIfTrue` | `SingleColorValue` | default `255` |
| `alphaIfFalse` | `SingleColorValue` | default `0` |

### SetAlphaGradient

```lua
Frame:SetAlphaGradient(index: number, gradient: vector2)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `index` | `number` |  |
| `gradient` | `vector2` | `Mixin=Vector2DMixin` |

### SetAttribute

```lua
Frame:SetAttribute(attributeName: cstring, value: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.Attributes }`

### SetAttributeNoHandler

```lua
Frame:SetAttributeNoHandler(attributeName: cstring, value: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.Attributes }`

### SetClampedToScreen

```lua
Frame:SetClampedToScreen(clampedToScreen: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetClampRectInsets

```lua
Frame:SetClampRectInsets(left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetClipsChildren

```lua
Frame:SetClipsChildren(clipsChildren: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDontSavePosition

```lua
Frame:SetDontSavePosition(dontSave: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetDrawLayerEnabled

```lua
Frame:SetDrawLayerEnabled(layer: DrawLayer, isEnabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `layer` | `DrawLayer` |  |
| `isEnabled` | `bool` | default `false` |

### SetFixedFrameLevel

```lua
Frame:SetFixedFrameLevel(isFixed: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetFixedFrameStrata

```lua
Frame:SetFixedFrameStrata(isFixed: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetFlattensRenderLayers

```lua
Frame:SetFlattensRenderLayers(flatten: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetFrameLevel

```lua
Frame:SetFrameLevel(frameLevel: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.FrameLevel }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetFrameStrata

```lua
Frame:SetFrameStrata(strata: FrameStrata)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.FrameStrata }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetHighlightLocked

```lua
Frame:SetHighlightLocked(locked: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetHitRectInsets

```lua
Frame:SetHitRectInsets(left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetHyperlinkPropagateToParent

```lua
Frame:SetHyperlinkPropagateToParent(canPropagate: bool)
```

Enables or disables propagating hyperlink events (ex. OnHyperlinkEnter, OnHyperlinkLeave, OnHyperlinkClick) to this frame's parent.

`SecretArguments=AllowedWhenUntainted`

### SetHyperlinksEnabled

```lua
Frame:SetHyperlinksEnabled(enabled: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetID

```lua
Frame:SetID(id: number)
```

`SecretArguments=AllowedWhenTainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.ID }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetIgnoreParentAlpha

```lua
Frame:SetIgnoreParentAlpha(ignore: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetIgnoreParentScale

```lua
Frame:SetIgnoreParentScale(ignore: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetIgnoringChildrenForBounds

```lua
Frame:SetIgnoringChildrenForBounds(ignore: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetIsFrameBuffer

```lua
Frame:SetIsFrameBuffer(isFrameBuffer: bool)
```

`SecretArguments=NotAllowed`

### SetMovable

```lua
Frame:SetMovable(movable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetOnUpdateMode

```lua
Frame:SetOnUpdateMode(onUpdateMode: OnUpdateMode)
```

Changes when OnUpdate scripts are executed for this object.

`SecretArguments=AllowedWhenUntainted`

### SetPropagateKeyboardInput

```lua
Frame:SetPropagateKeyboardInput(propagate: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetResizable

```lua
Frame:SetResizable(resizable: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetResizeBounds

```lua
Frame:SetResizeBounds(minWidth: uiUnit, minHeight: uiUnit, maxWidth: uiUnit?, maxHeight: uiUnit?)
```

`SecretArguments=AllowedWhenUntainted`

### SetRolesets

```lua
Frame:SetRolesets(rolesetsString: cstring?)
```

Sets the roleset tags for this frame, used by the UI mode system to gate visibility. Supports comma-separated names to assign multiple rolesets. Pass nil to clear.

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetScale

```lua
Frame:SetScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Scale }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetShown

```lua
Frame:SetShown(shown: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Shown }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `shown` | `bool` | default `false` |

### SetToplevel

```lua
Frame:SetToplevel(topLevel: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Toplevel }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetUserPlaced

```lua
Frame:SetUserPlaced(userPlaced: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetUsingParentLevel

```lua
Frame:SetUsingParentLevel(usingParentLevel: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetWindow

```lua
Frame:SetWindow(window: SimpleWindow?)
```

`SecretArguments=AllowedWhenUntainted`

### Show

```lua
Frame:Show()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### StartMoving

```lua
Frame:StartMoving(alwaysStartFromMouse: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `alwaysStartFromMouse` | `bool` | default `false` |

### StartSizing

```lua
Frame:StartSizing(resizePoint: FramePoint?, alwaysStartFromMouse: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `resizePoint` | `FramePoint?` |  |
| `alwaysStartFromMouse` | `bool` | default `false` |

### StopMovingOrSizing

```lua
Frame:StopMovingOrSizing()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### UnlockHighlight

```lua
Frame:UnlockHighlight()
```

### UnregisterAllEvents

```lua
Frame:UnregisterAllEvents()
```

### UnregisterEvent

```lua
Frame:UnregisterEvent(eventName: cstring) -> registered: bool
```

`SecretArguments=AllowedWhenUntainted`

## Types

### CreateRegionParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring?` |  |
| `drawLayer` | `DrawLayer?` |  |
| `templateName` | `cstring?` |  |
| `subLevel` | `number?` |  |

### FrameEventCallbackType

*CallbackType*
