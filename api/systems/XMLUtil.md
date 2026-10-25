# XMLUtil

Namespace `C_XMLUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/xmlutildocumentation.lua` (FileDataID 4637311)

## Functions

### GetTemplateInfo

```lua
C_XMLUtil.GetTemplateInfo(name: cstring) -> info: XMLTemplateInfo
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetTemplates

```lua
C_XMLUtil.GetTemplates() -> templates: XMLTemplateListInfo[]
```

## Types

### XMLTemplateInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `cstring` |  |
| `width` | `number` |  |
| `height` | `number` |  |
| `keyValues` | `XMLTemplateKeyValue[]` |  |
| `inherits` | `cstring?` |  |
| `sourceLocation` | `string` |  |

### XMLTemplateKeyValue

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `key` | `cstring` |  |
| `keyType` | `cstring` |  |
| `type` | `cstring` |  |
| `value` | `cstring` |  |

### XMLTemplateListInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `type` | `cstring` |  |
