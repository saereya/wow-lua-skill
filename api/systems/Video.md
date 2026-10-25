# Video

Namespace `C_VideoOptions` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/videodocumentation.lua` (FileDataID 4637310)

## Functions

### AreHighResTexturesAvailable

```lua
C_VideoOptions.AreHighResTexturesAvailable() -> areAvailable: bool
```

### GetCurrentGameWindowSize

```lua
C_VideoOptions.GetCurrentGameWindowSize() -> size: vector2
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `size` | `vector2` | `Mixin=Vector2DMixin` |

### GetDefaultGameWindowSize

```lua
C_VideoOptions.GetDefaultGameWindowSize(monitor: number) -> size: vector2
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `size` | `vector2` | `Mixin=Vector2DMixin` |

### GetGameWindowSizes

```lua
C_VideoOptions.GetGameWindowSizes(monitor: number, fullscreen: bool) -> sizes: vector2[]
```

`SecretArguments=AllowedWhenUntainted`

### GetGxAdapterInfo

```lua
C_VideoOptions.GetGxAdapterInfo() -> adapters: GxAdapterInfoDetails[]
```

### IsLinearEnabledOnStart

```lua
C_VideoOptions.IsLinearEnabledOnStart() -> isEnabled: bool
```

### IsOutlineModeSupported

```lua
C_VideoOptions.IsOutlineModeSupported() -> isSupported: bool
```

### IsPBRWaterSupported

```lua
C_VideoOptions.IsPBRWaterSupported() -> isSupported: bool
```

### IsSecondaryLightingSupported

```lua
C_VideoOptions.IsSecondaryLightingSupported() -> isSupported: bool
```

### IsSpellVisualDensitySystemSupported

```lua
C_VideoOptions.IsSpellVisualDensitySystemSupported() -> isSupported: bool
```

### SetGameWindowSize

```lua
C_VideoOptions.SetGameWindowSize(x: number, y: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ADAPTER_LIST_CHANGED

```lua
ADAPTER_LIST_CHANGED()
```

`SynchronousEvent`

### DISPLAY_SIZE_CHANGED

```lua
DISPLAY_SIZE_CHANGED()
```

`SynchronousEvent`

### GLUE_SCREENSHOT_FAILED

```lua
GLUE_SCREENSHOT_FAILED()
```

`SynchronousEvent`

### GLUE_SCREENSHOT_STARTED

```lua
GLUE_SCREENSHOT_STARTED()
```

`SynchronousEvent`

### GLUE_SCREENSHOT_SUCCEEDED

```lua
GLUE_SCREENSHOT_SUCCEEDED()
```

`SynchronousEvent`

### GX_RESTARTED

```lua
GX_RESTARTED()
```

`SynchronousEvent`

### SCREENSHOT_FAILED

```lua
SCREENSHOT_FAILED()
```

`SynchronousEvent`

### SCREENSHOT_STARTED

```lua
SCREENSHOT_STARTED()
```

`SynchronousEvent`

### SCREENSHOT_SUCCEEDED

```lua
SCREENSHOT_SUCCEEDED()
```

`SynchronousEvent`

## Types

### GraphicsValidationResult

*Enumeration* · 43 values, 0..42

Access values as `Enum.GraphicsValidationResult.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Supported` | `GraphicsValidationResult` | = 0 |
| `Illegal` | `GraphicsValidationResult` | = 1 |
| `Unsupported` | `GraphicsValidationResult` | = 2 |
| `Graphics` | `GraphicsValidationResult` | = 3 |
| `DualCore` | `GraphicsValidationResult` | = 4 |
| `QuadCore` | `GraphicsValidationResult` | = 5 |
| `CpuMem_2` | `GraphicsValidationResult` | = 6 |
| `CpuMem_4` | `GraphicsValidationResult` | = 7 |
| `CpuMem_8` | `GraphicsValidationResult` | = 8 |
| `Needs_5_0` | `GraphicsValidationResult` | = 9 |
| `Needs_6_0` | `GraphicsValidationResult` | = 10 |
| `NeedsRt` | `GraphicsValidationResult` | = 11 |
| `NeedsDx12` | `GraphicsValidationResult` | = 12 |
| `NeedsDx12Vrs2` | `GraphicsValidationResult` | = 13 |
| `NeedsAppleGpu` | `GraphicsValidationResult` | = 14 |
| `NeedsAmdGpu` | `GraphicsValidationResult` | = 15 |
| `NeedsIntelGpu` | `GraphicsValidationResult` | = 16 |
| `NeedsNvidiaGpu` | `GraphicsValidationResult` | = 17 |
| `NeedsQualcommGpu` | `GraphicsValidationResult` | = 18 |
| `NeedsMacOs_10_13` | `GraphicsValidationResult` | = 19 |
| `NeedsMacOs_10_14` | `GraphicsValidationResult` | = 20 |
| `NeedsMacOs_10_15` | `GraphicsValidationResult` | = 21 |
| `NeedsMacOs_11_0` | `GraphicsValidationResult` | = 22 |
| `NeedsMacOs_12_0` | `GraphicsValidationResult` | = 23 |
| `NeedsMacOs_13_0` | `GraphicsValidationResult` | = 24 |
| `NeedsWindows_10` | `GraphicsValidationResult` | = 25 |
| `NeedsWindows_11` | `GraphicsValidationResult` | = 26 |
| `MacOsUnsupported` | `GraphicsValidationResult` | = 27 |
| `WindowsUnsupported` | `GraphicsValidationResult` | = 28 |
| `LegacyUnsupported` | `GraphicsValidationResult` | = 29 |
| `Dx11Unsupported` | `GraphicsValidationResult` | = 30 |
| `Dx12Win7Unsupported` | `GraphicsValidationResult` | = 31 |
| `RemoteDesktopUnsupported` | `GraphicsValidationResult` | = 32 |
| `WineUnsupported` | `GraphicsValidationResult` | = 33 |
| `NvapiWineUnsupported` | `GraphicsValidationResult` | = 34 |
| `AppleGpuUnsupported` | `GraphicsValidationResult` | = 35 |
| `AmdGpuUnsupported` | `GraphicsValidationResult` | = 36 |
| `IntelGpuUnsupported` | `GraphicsValidationResult` | = 37 |
| `NvidiaGpuUnsupported` | `GraphicsValidationResult` | = 38 |
| `QualcommGpuUnsupported` | `GraphicsValidationResult` | = 39 |
| `GpuDriver` | `GraphicsValidationResult` | = 40 |
| `CompatMode` | `GraphicsValidationResult` | = 41 |
| `Unknown` | `GraphicsValidationResult` | = 42 |

### GxAdapterInfoDetails

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `isLowPower` | `bool` |  |
| `isExternal` | `bool` |  |
