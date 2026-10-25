# NamePlate

Widget methods (`FrameAPINamePlate`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapinameplatedocumentation.lua` (FileDataID 7676212)

## Methods

### CanChangeHitTestPoints

```lua
NamePlate:CanChangeHitTestPoints() -> canChangeHitTestPoints: bool
```

Returns true if this nameplate permits changes to its hit-test points. Updates are normally blocked for tainted code during combat, except on the tick a unit is first assigned or when untainted code updates hit-test points on the same tick.

### ClearAllHitTestPoints

```lua
NamePlate:ClearAllHitTestPoints()
```

Clears the anchor points that determine where the mouse interacts with the nameplate.

`RequiresCanChangeHitTestPoints`

### GetHitTestPoints

```lua
NamePlate:GetHitTestPoints() -> anchors: AnchorBinding[]
```

Returns the anchor points that determine where the mouse interacts with the nameplate.

### SetAllHitTestPoints

```lua
NamePlate:SetAllHitTestPoints(relativeTo: ScriptRegion)
```

Sets the anchor points that determine where the mouse interacts with the nameplate to fully encompass the target region.

`SecretArguments=AllowedWhenUntainted` `RequiresCanChangeHitTestPoints`

### SetHitTestPoints

```lua
NamePlate:SetHitTestPoints(anchors: AnchorBinding[])
```

Sets the anchor points that determine where the mouse interacts with the nameplate.

`SecretArguments=AllowedWhenUntainted` `RequiresCanChangeHitTestPoints`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `anchors` | `AnchorBinding[]` | List of anchor points to use for hit testing. All existing points will be cleared. |

### SetStackingBoundsFrame

```lua
NamePlate:SetStackingBoundsFrame(frame: SimpleFrame)
```

`SecretArguments=AllowedWhenUntainted`

## Predicates

Conditions referenced by the flags above.

- `RequiresCanChangeHitTestPoints` *Precondition* (failure mode: Error): Guarded APIs require that the nameplate frame must allow changes to its hit test points.
