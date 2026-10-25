# PartyPose

Namespace `C_PartyPose` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/partyposeuidocumentation.lua` (FileDataID 4637152)

## Functions

### ExtraAction

```lua
C_PartyPose.ExtraAction(partyPoseID: number)
```

`SecretArguments=AllowedWhenUntainted`

### GetPartyPoseInfoByID

```lua
C_PartyPose.GetPartyPoseInfoByID(mapID: number) -> info: PartyPoseInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetPartyPoseInfoByMapID

```lua
C_PartyPose.GetPartyPoseInfoByMapID(mapID: number) -> info: PartyPoseInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### HasExtraAction

```lua
C_PartyPose.HasExtraAction(partyPoseID: number) -> hasExtraAction: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SHOW_PARTY_POSE_UI

```lua
SHOW_PARTY_POSE_UI(mapID: number, won: bool)
```

`SynchronousEvent`

## Types

### PartyPoseInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `partyPoseID` | `number` |  |
| `mapID` | `number` |  |
| `widgetSetID` | `number?` |  |
| `victoryModelSceneID` | `number` |  |
| `defeatModelSceneID` | `number` |  |
| `victorySoundKitID` | `number` |  |
| `defeatSoundKitID` | `number` |  |
| `uiTextureKit` | `textureKit?` |  |
| `titleText` | `string?` |  |
| `extraButtonText` | `string?` |  |
| `flags` | `PartyPoseFlags` |  |
