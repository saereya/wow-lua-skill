# MirrorTimer

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/mirrortimerdocumentation.lua` (FileDataID 5559829)

## Functions

### GetMirrorTimerInfo

```lua
GetMirrorTimerInfo(timerIndex: luaIndex) -> name: cstring, startValue: number, maxValue: number, scale: number, paused: number, label: cstring, spellID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetMirrorTimerProgress

```lua
GetMirrorTimerProgress(timerName: cstring) -> progress: number?
```

`SecretArguments=AllowedWhenUntainted`

## Types

### MirrorTimerInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `startValue` | `number` |  |
| `maxValue` | `number` |  |
| `scale` | `number` |  |
| `paused` | `number` |  |
| `label` | `cstring` |  |
| `spellID` | `number` |  |
