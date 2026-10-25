# ChatShared

source `interface/addons/blizzard_apidocumentationgenerated/chatshareddocumentation.lua` (FileDataID 7872491)

## Types

### AddonMessageParams

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `prefix` | `cstring` |  |
| `message` | `cstring` |  |
| `chatType` | `cstring?` | ChatType, defaults to SLASH_CMD_PARTY. |
| `target` | `cstring?` | Only applies for targeted channels |
