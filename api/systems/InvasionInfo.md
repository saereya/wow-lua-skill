# InvasionInfo

Namespace `C_InvasionInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/invasioninfodocumentation.lua` (FileDataID 4637112)

## Functions

### AreInvasionsAvailable

```lua
C_InvasionInfo.AreInvasionsAvailable() -> areInvasionsAvailable: bool
```

Returns true if invasions are active in the same physical area as the player.

### GetInvasionForUiMapID

```lua
C_InvasionInfo.GetInvasionForUiMapID(uiMapID: number) -> invasionID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetInvasionInfo

```lua
C_InvasionInfo.GetInvasionInfo(invasionID: number) -> invasionInfo: InvasionMapInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInvasionTimeLeft

```lua
C_InvasionInfo.GetInvasionTimeLeft(invasionID: number) -> timeLeftMinutes: number?
```

`SecretArguments=AllowedWhenUntainted`

## Types

### InvasionMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `invasionID` | `number` |  |
| `name` | `string` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `atlasName` | `textureAtlas` |  |
| `rewardQuestID` | `number?` |  |
