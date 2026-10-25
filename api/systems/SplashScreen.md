# SplashScreen

Namespace `C_SplashScreen` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/splashscreendocumentation.lua` (FileDataID 4637252)

## Functions

### AcknowledgeSplash

```lua
C_SplashScreen.AcknowledgeSplash()
```

### CanViewSplashScreen

```lua
C_SplashScreen.CanViewSplashScreen() -> canView: bool
```

### RequestLatestSplashScreen

```lua
C_SplashScreen.RequestLatestSplashScreen(fromGameMenu: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SendSplashScreenActionLaunchedTelem

```lua
C_SplashScreen.SendSplashScreenActionLaunchedTelem()
```

`HasRestrictions`

### SendSplashScreenCloseTelem

```lua
C_SplashScreen.SendSplashScreenCloseTelem()
```

`HasRestrictions`

## Events

### OPEN_SPLASH_SCREEN

```lua
OPEN_SPLASH_SCREEN(info: SplashScreenInfo?)
```

`SynchronousEvent`

## Types

### SplashScreenInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `textureKit` | `textureKit` |  |
| `minDisplayCharLevel` | `number` |  |
| `minQuestDisplayLevel` | `number` |  |
| `soundKitID` | `number` |  |
| `allianceQuestID` | `number?` |  |
| `hordeQuestID` | `number?` |  |
| `header` | `string` |  |
| `topLeftFeatureTitle` | `string` |  |
| `topLeftFeatureDesc` | `string` |  |
| `bottomLeftFeatureTitle` | `string` |  |
| `bottomLeftFeatureDesc` | `string` |  |
| `rightFeatureTitle` | `string` |  |
| `rightFeatureDesc` | `string` |  |
| `shouldShowQuest` | `bool` |  |
| `screenType` | `SplashScreenType` |  |
| `gameMenuRequest` | `bool` |  |
