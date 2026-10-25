# AchievementInfo

Namespace `C_AchievementInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/achievementinfodocumentation.lua` (FileDataID 4637014)

## Functions

### AreGuildAchievementsEnabled

```lua
C_AchievementInfo.AreGuildAchievementsEnabled() -> enabled: bool
```

### GetRewardItemID

```lua
C_AchievementInfo.GetRewardItemID(achievementID: number) -> rewardItemID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetSupercedingAchievements

```lua
C_AchievementInfo.GetSupercedingAchievements(achievementID: number) -> supercedingAchievements: number[]
```

`SecretArguments=AllowedWhenUntainted`

### IsGuildAchievement

```lua
C_AchievementInfo.IsGuildAchievement(achievementId: number) -> isGuild: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsValidAchievement

```lua
C_AchievementInfo.IsValidAchievement(achievementId: number) -> isValidAchievement: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetPortraitTexture

```lua
C_AchievementInfo.SetPortraitTexture(textureObject: SimpleTexture)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ACHIEVEMENT_EARNED

```lua
ACHIEVEMENT_EARNED(achievementID: number, alreadyEarned: bool?)
```

`SynchronousEvent`

### ACHIEVEMENT_PLAYER_NAME

```lua
ACHIEVEMENT_PLAYER_NAME(achievementID: number)
```

`SynchronousEvent`

### ACHIEVEMENT_SEARCH_UPDATED

```lua
ACHIEVEMENT_SEARCH_UPDATED()
```

`SynchronousEvent`

### CRITERIA_COMPLETE

```lua
CRITERIA_COMPLETE(criteriaID: number)
```

`SynchronousEvent`

### CRITERIA_EARNED

```lua
CRITERIA_EARNED(achievementID: number, description: cstring, achievementAlreadyEarnedOnAccount: bool)
```

`SynchronousEvent`

### CRITERIA_UPDATE

```lua
CRITERIA_UPDATE()
```

`SynchronousEvent`

### INSPECT_ACHIEVEMENT_READY

```lua
INSPECT_ACHIEVEMENT_READY(guid: WOWGUID)
```

`SynchronousEvent`

### RECEIVED_ACHIEVEMENT_LIST

```lua
RECEIVED_ACHIEVEMENT_LIST()
```

`UniqueEvent`

### RECEIVED_ACHIEVEMENT_MEMBER_LIST

```lua
RECEIVED_ACHIEVEMENT_MEMBER_LIST(achievementID: number)
```

`SynchronousEvent`

### TRACKED_ACHIEVEMENT_LIST_CHANGED

```lua
TRACKED_ACHIEVEMENT_LIST_CHANGED(achievementID: number?, added: bool?)
```

`SynchronousEvent`

### TRACKED_ACHIEVEMENT_UPDATE

```lua
TRACKED_ACHIEVEMENT_UPDATE(achievementID: number, criteriaID: number?, elapsed: time_t?, duration: number?)
```

`SynchronousEvent`
