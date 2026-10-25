# SocialUI

Namespace `C_SocialUI` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/socialuidocumentation.lua` (FileDataID 7833664)

## Functions

### IsSystemEnabled

```lua
C_SocialUI.IsSystemEnabled() -> isSocialUISystemEnabled: bool
```

## Events

### SOCIAL_UI_SYSTEM_STATUS_UPDATED

```lua
SOCIAL_UI_SYSTEM_STATUS_UPDATED()
```

`SynchronousEvent`

## Types

### SocialSystemType

*Enumeration* · 5 values, 0..4

Access values as `Enum.SocialSystemType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Friends` | `SocialSystemType` | = 0 |
| `QuickJoin` | `SocialSystemType` | = 1 |
| `RaidList` | `SocialSystemType` | = 2 |
| `RecruitAFriend` | `SocialSystemType` | = 3 |
| `RecentAllies` | `SocialSystemType` | = 4 |

### SocialUIBlockType

*Enumeration* · 3 values, 0..2

Access values as `Enum.SocialUIBlockType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `SocialUIBlockType` | = 0 |
| `Ignore` | `SocialUIBlockType` | = 1 |
| `BattleNetInviteBlock` | `SocialUIBlockType` | = 2 |

### SocialUIPresenceType

*Enumeration* · 6 values, 0..5

Access values as `Enum.SocialUIPresenceType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unknown` | `SocialUIPresenceType` | = 0 |
| `Online` | `SocialUIPresenceType` | = 1 |
| `Offline` | `SocialUIPresenceType` | = 2 |
| `Away` | `SocialUIPresenceType` | = 3 |
| `Busy` | `SocialUIPresenceType` | = 4 |
| `AppearOffline` | `SocialUIPresenceType` | = 5 |
