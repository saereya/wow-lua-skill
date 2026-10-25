# ScriptRegion

Widget methods (`SimpleScriptRegionAPI`) · inherits [`Object`](Object.md), [`ScriptRegionResizing`](ScriptRegionResizing.md), [`AnimatableObject`](AnimatableObject.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplescriptregionapidocumentation.lua` (FileDataID 4637232)

## Methods

### CanChangeProtectedState

```lua
ScriptRegion:CanChangeProtectedState() -> canChange: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### CanPropagateMouseClicks

```lua
ScriptRegion:CanPropagateMouseClicks() -> canPropagate: bool
```

### CanPropagateMouseMotion

```lua
ScriptRegion:CanPropagateMouseMotion() -> canPropagate: bool
```

### ClearScripts

```lua
ScriptRegion:ClearScripts()
```

Remove all script handlers set through Scripts in XML or SetScript in Lua

### CollapsesLayout

```lua
ScriptRegion:CollapsesLayout() -> collapsesLayout: bool
```

### EnableMouse

```lua
ScriptRegion:EnableMouse(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### EnableMouseMotion

```lua
ScriptRegion:EnableMouseMotion(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### EnableMouseWheel

```lua
ScriptRegion:EnableMouseWheel(enable: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enable` | `bool` | default `false` |

### FocusEnter

```lua
ScriptRegion:FocusEnter(fromMouseMotion: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `fromMouseMotion` | `bool` | default `true` |

### FocusExit

```lua
ScriptRegion:FocusExit(fromMouseMotion: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `fromMouseMotion` | `bool` | default `true` |

### GetBottom

```lua
ScriptRegion:GetBottom() -> bottom: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetCenter

```lua
ScriptRegion:GetCenter() -> x: uiUnit, y: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetHeight

```lua
ScriptRegion:GetHeight(ignoreRect: bool) -> height: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreRect` | `bool` | default `false` |

### GetLeft

```lua
ScriptRegion:GetLeft() -> left: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetRect

```lua
ScriptRegion:GetRect() -> left: uiUnit, bottom: uiUnit, width: uiUnit, height: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetRight

```lua
ScriptRegion:GetRight() -> right: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetRoundLayoutToNearestPixel

```lua
ScriptRegion:GetRoundLayoutToNearestPixel() -> enabled: bool
```

### GetScaledRect

```lua
ScriptRegion:GetScaledRect() -> left: uiUnit, bottom: uiUnit, width: uiUnit, height: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetScript

```lua
ScriptRegion:GetScript(scriptTypeName: ScriptTypeName, bindingType: ScriptBindingType) -> script: LuaFunctionReference
```

`SecretArguments=AllowedWhenUntainted` `RequiresSupportedScript` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### GetSize

```lua
ScriptRegion:GetSize(ignoreRect: bool) -> width: uiUnit, height: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreRect` | `bool` | default `false` |

### GetSourceLocation

```lua
ScriptRegion:GetSourceLocation() -> location: string
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectDebug }`

### GetTop

```lua
ScriptRegion:GetTop() -> top: uiUnit
```

`MayReturnNothing` `SecretWhenAnchoringSecret`

### GetWidth

```lua
ScriptRegion:GetWidth(ignoreRect: bool) -> width: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreRect` | `bool` | default `false` |

### HasScript

```lua
ScriptRegion:HasScript(scriptName: cstring) -> hasScript: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretReturnsForAspect={ Enum.SecretAspect.ObjectType }` `ConstSecretAccessor`

### Hide

```lua
ScriptRegion:Hide()
```

### HookScript

```lua
ScriptRegion:HookScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference, bindingType: ScriptBindingType) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `scriptTypeName` | `ScriptTypeName` |  |
| `script` | `LuaFunctionReference` |  |
| `bindingType` | `ScriptBindingType` | default `"Extrinsic"` |

### Intersects

```lua
ScriptRegion:Intersects(region: ScriptRegion) -> intersects: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret`

### IsAnchoringRestricted

```lua
ScriptRegion:IsAnchoringRestricted() -> isRestricted: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### IsAnchoringSecret

```lua
ScriptRegion:IsAnchoringSecret() -> isSecret: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecrets }`

### IsCollapsed

```lua
ScriptRegion:IsCollapsed() -> isCollapsed: bool
```

### IsDragging

```lua
ScriptRegion:IsDragging() -> isDragging: bool
```

### IsMouseClickEnabled

```lua
ScriptRegion:IsMouseClickEnabled() -> enabled: bool
```

### IsMouseEnabled

```lua
ScriptRegion:IsMouseEnabled() -> enabled: bool
```

### IsMouseMotionEnabled

```lua
ScriptRegion:IsMouseMotionEnabled() -> enabled: bool
```

### IsMouseMotionFocus

```lua
ScriptRegion:IsMouseMotionFocus() -> isMouseMotionFocus: bool
```

### IsMouseOver

```lua
ScriptRegion:IsMouseOver(offsetTop: uiUnit, offsetBottom: uiUnit, offsetLeft: uiUnit, offsetRight: uiUnit) -> isMouseOver: bool
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `offsetTop` | `uiUnit` | default `0` |
| `offsetBottom` | `uiUnit` | default `0` |
| `offsetLeft` | `uiUnit` | default `0` |
| `offsetRight` | `uiUnit` | default `0` |

### IsMouseWheelEnabled

```lua
ScriptRegion:IsMouseWheelEnabled() -> enabled: bool
```

### IsProtected

```lua
ScriptRegion:IsProtected() -> isProtected: bool, isProtectedExplicitly: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ObjectSecurity }`

### IsRectValid

```lua
ScriptRegion:IsRectValid() -> isValid: bool
```

### IsShown

```lua
ScriptRegion:IsShown() -> isShown: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.Shown }`

### IsVisible

```lua
ScriptRegion:IsVisible() -> isVisible: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.Shown }`

### MouseDown

```lua
ScriptRegion:MouseDown(button: cstring)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `button` | `cstring` | default `"LeftButton"` |

### MouseUp

```lua
ScriptRegion:MouseUp(button: cstring)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `button` | `cstring` | default `"LeftButton"` |

### SetCollapsesLayout

```lua
ScriptRegion:SetCollapsesLayout(collapsesLayout: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetMouseClickEnabled

```lua
ScriptRegion:SetMouseClickEnabled(enabled: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetMouseMotionEnabled

```lua
ScriptRegion:SetMouseMotionEnabled(enabled: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetParent

```lua
ScriptRegion:SetParent(parent: SimpleFrame?)
```

`SecretArguments=NotAllowed` `IsProtectedFunction` `CheckAllowChangeParent`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetPassThroughButtons

```lua
ScriptRegion:SetPassThroughButtons(buttons: MouseButton)
```

`SecretArguments=NotAllowed` `IsProtectedFunction` `HasRestrictions`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `buttons` | `MouseButton` | `StrideIndex=1` |

### SetPropagateMouseClicks

```lua
ScriptRegion:SetPropagateMouseClicks(propagate: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction` `HasRestrictions`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetPropagateMouseMotion

```lua
ScriptRegion:SetPropagateMouseMotion(propagate: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction` `HasRestrictions`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetRoundLayoutToNearestPixel

```lua
ScriptRegion:SetRoundLayoutToNearestPixel(enabled: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetScript

```lua
ScriptRegion:SetScript(scriptTypeName: ScriptTypeName, script: LuaFunctionReference?)
```

`SecretArguments=AllowedWhenUntainted` `RequiresAssignableScript`

### SetShown

```lua
ScriptRegion:SetShown(show: bool)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Shown }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `show` | `bool` | default `false` |

### ShouldButtonPassThrough

```lua
ScriptRegion:ShouldButtonPassThrough(button: MouseButton) -> shouldPassThrough: bool
```

`SecretArguments=AllowedWhenUntainted`

### Show

```lua
ScriptRegion:Show()
```
