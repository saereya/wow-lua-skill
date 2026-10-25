# ClientScene

Namespace `C_ClientScene` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/clientscenedocumentation.lua` (FileDataID 4637060)

## Functions

### IsSceneTypeActive

```lua
C_ClientScene.IsSceneTypeActive(desiredSceneType: ClientSceneType?) -> isPlaying: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### CLIENT_SCENE_CLOSED

```lua
CLIENT_SCENE_CLOSED()
```

`SynchronousEvent`

### CLIENT_SCENE_OPENED

```lua
CLIENT_SCENE_OPENED(sceneType: ClientSceneType)
```

`SynchronousEvent`

## Types

### ClientSceneType

*Enumeration* · 2 values, 0..1

Access values as `Enum.ClientSceneType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `DefaultSceneType` | `ClientSceneType` | = 0 |
| `MinigameSceneType` | `ClientSceneType` | = 1 |
