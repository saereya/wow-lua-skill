# UserFeedback

Namespace `C_UserFeedback` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/userfeedbackdocumentation.lua` (FileDataID 4637291)

## Functions

### SubmitBug

```lua
C_UserFeedback.SubmitBug(bugInfo: cstring, suppressNotification: bool) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `bugInfo` | `cstring` |  |
| `suppressNotification` | `bool` | default `false` |

### SubmitSuggestion

```lua
C_UserFeedback.SubmitSuggestion(suggestion: cstring) -> success: bool
```

`SecretArguments=AllowedWhenUntainted`
