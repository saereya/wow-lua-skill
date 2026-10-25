# OffScreenFrame

Widget methods (`SimpleOffScreenFrameAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleoffscreenframeapidocumentation.lua` (FileDataID 4637231)

## Methods

### ApplySnapshot

```lua
OffScreenFrame:ApplySnapshot(texture: SimpleTexture, snapshotID: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

### Flush

```lua
OffScreenFrame:Flush()
```

### GetMaxSnapshots

```lua
OffScreenFrame:GetMaxSnapshots() -> maxSnapshots: number
```

### IsSnapshotValid

```lua
OffScreenFrame:IsSnapshotValid(snapshotID: number) -> isValid: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetMaxSnapshots

```lua
OffScreenFrame:SetMaxSnapshots(maxSnapshots: number)
```

`SecretArguments=AllowedWhenUntainted`

### TakeSnapshot

```lua
OffScreenFrame:TakeSnapshot() -> snapshotID: number?
```

### TestPrintToFile

```lua
OffScreenFrame:TestPrintToFile(snapshotID: number, filename: cstring) -> success: bool
```

Unavailable in public builds

`SecretArguments=AllowedWhenUntainted`

### UsesNPOT

```lua
OffScreenFrame:UsesNPOT() -> usesNPOT: bool?
```
