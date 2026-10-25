# SocialRestrictions

Namespace `C_SocialRestrictions` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/socialrestrictionsdocumentation.lua` (FileDataID 4637237)

## Functions

### AcknowledgeAgeVerificationRestriction

```lua
C_SocialRestrictions.AcknowledgeAgeVerificationRestriction()
```

### AcknowledgeRegionalChatDisabled

```lua
C_SocialRestrictions.AcknowledgeRegionalChatDisabled()
```

### CanReceiveChat

```lua
C_SocialRestrictions.CanReceiveChat() -> canReceiveChat: bool
```

Returns true if the player meets all conditions that allow them to receive chat messages.

### CanSendChat

```lua
C_SocialRestrictions.CanSendChat() -> canSendChat: bool
```

Returns true if the player meets all conditions that allow them to send chat messages.

### IsAgeVerificationRestricted

```lua
C_SocialRestrictions.IsAgeVerificationRestricted() -> restricted: bool
```

Returns true if the account is restricted by the Age Verification feature.

### IsAgeVerificationRestrictedMinor

```lua
C_SocialRestrictions.IsAgeVerificationRestrictedMinor() -> isMinor: bool
```

Returns true if the Age Verification restriction is because the account belongs to a minor, as opposed to an adult who has not yet verified their age.

`HasRestrictions`

### IsChatDisabled

```lua
C_SocialRestrictions.IsChatDisabled() -> disabled: bool
```

### IsFriendsDisabled

```lua
C_SocialRestrictions.IsFriendsDisabled() -> disabled: bool
```

### IsMuted

```lua
C_SocialRestrictions.IsMuted() -> isMuted: bool
```

### IsSilenced

```lua
C_SocialRestrictions.IsSilenced() -> isSilenced: bool
```

### IsSquelched

```lua
C_SocialRestrictions.IsSquelched() -> isSquelched: bool
```

### SetChatDisabled

```lua
C_SocialRestrictions.SetChatDisabled(disabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### ALERT_AGE_VERIFICATION_RESTRICTED

```lua
ALERT_AGE_VERIFICATION_RESTRICTED()
```

`SynchronousEvent`

### ALERT_REGIONAL_CHAT_DISABLED

```lua
ALERT_REGIONAL_CHAT_DISABLED()
```

`SynchronousEvent`

### CHAT_DISABLED_CHANGED

```lua
CHAT_DISABLED_CHANGED(disabled: bool)
```

`SynchronousEvent`

### CHAT_DISABLED_CHANGE_FAILED

```lua
CHAT_DISABLED_CHANGE_FAILED(disabled: bool)
```

`SynchronousEvent`
