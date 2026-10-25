# LimitedInput

Namespace `C_LimitedInput` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/limitedinputdocumentation.lua` (FileDataID 7664505)

## Functions

### LimitedInputAllowed

```lua
C_LimitedInput.LimitedInputAllowed(type: LimitedInputType) -> allowed: bool
```

`SecretArguments=AllowedWhenUntainted`

## Types

### LimitedInputType

*Enumeration* · 4 values, 0..3

Access values as `Enum.LimitedInputType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `MouseMove` | `LimitedInputType` | = 0 |
| `MouseDown` | `LimitedInputType` | = 1 |
| `MouseUp` | `LimitedInputType` | = 2 |
| `MouseWheel` | `LimitedInputType` | = 3 |
