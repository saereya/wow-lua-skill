# UIFrameManager

Namespace `C_FrameManager` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uiframemanagerdocumentation.lua` (FileDataID 4637284)

## Functions

### GetFrameVisibilityState

```lua
C_FrameManager.GetFrameVisibilityState(frameType: UIFrameType) -> shouldShow: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### FRAME_MANAGER_UPDATE_ALL

```lua
FRAME_MANAGER_UPDATE_ALL()
```

`SynchronousEvent`

### FRAME_MANAGER_UPDATE_FRAME

```lua
FRAME_MANAGER_UPDATE_FRAME(type: UIFrameType, show: bool)
```

`SynchronousEvent`

## Types

### UIFrameType

*Enumeration* · 2 values, 0..1

Access values as `Enum.UIFrameType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `JailersTowerBuffs` | `UIFrameType` | = 0 |
| `InterruptTutorial` | `UIFrameType` | = 1 |
