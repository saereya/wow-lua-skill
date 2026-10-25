# ScrollFrame

Widget methods (`SimpleScrollFrameAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplescrollframeapidocumentation.lua` (FileDataID 4637236)

## Methods

### GetHorizontalScroll

```lua
ScrollFrame:GetHorizontalScroll() -> offset: uiUnit
```

`SecretReturnsForAspect={ Enum.SecretAspect.ScrollOffset }`

### GetHorizontalScrollRange

```lua
ScrollFrame:GetHorizontalScrollRange() -> range: uiUnit
```

`SecretReturnsForAspect={ Enum.SecretAspect.ScrollRange }`

### GetScrollChild

```lua
ScrollFrame:GetScrollChild() -> scrollChild: SimpleFrame
```

### GetVerticalScroll

```lua
ScrollFrame:GetVerticalScroll() -> offset: uiUnit
```

`SecretReturnsForAspect={ Enum.SecretAspect.ScrollOffset }`

### GetVerticalScrollRange

```lua
ScrollFrame:GetVerticalScrollRange() -> range: uiUnit
```

`SecretReturnsForAspect={ Enum.SecretAspect.ScrollRange }`

### SetHorizontalScroll

```lua
ScrollFrame:SetHorizontalScroll(offset: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.ScrollOffset }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetScrollChild

```lua
ScrollFrame:SetScrollChild(scrollChild: SimpleFrame)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `CheckAllowChangeParent`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetVerticalScroll

```lua
ScrollFrame:SetVerticalScroll(offset: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.ScrollOffset }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### UpdateScrollChildRect

```lua
ScrollFrame:UpdateScrollChildRect()
```
