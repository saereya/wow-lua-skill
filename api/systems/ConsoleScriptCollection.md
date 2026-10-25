# ConsoleScriptCollection

Namespace `C_ConsoleScriptCollection` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/consolescriptcollectiondocumentation.lua` (FileDataID 5004766)

## Functions

### GetCollectionDataByID

```lua
C_ConsoleScriptCollection.GetCollectionDataByID(collectionID: number) -> data: ConsoleScriptCollectionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetCollectionDataByTag

```lua
C_ConsoleScriptCollection.GetCollectionDataByTag(collectionTag: string) -> data: ConsoleScriptCollectionData?
```

`SecretArguments=AllowedWhenUntainted`

### GetElements

```lua
C_ConsoleScriptCollection.GetElements(collectionID: number) -> elementIDs: ConsoleScriptCollectionElementData[]
```

`SecretArguments=AllowedWhenUntainted`

### GetScriptData

```lua
C_ConsoleScriptCollection.GetScriptData(consoleScriptID: number) -> data: ConsoleScriptData
```

`SecretArguments=AllowedWhenUntainted`

## Types

### ConsoleScriptCollectionData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `cstring` |  |

### ConsoleScriptCollectionElementData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `collectionID` | `number?` |  |
| `consoleScriptID` | `number?` |  |

### ConsoleScriptData

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ID` | `number` |  |
| `name` | `cstring` |  |
| `help` | `cstring` |  |
| `script` | `cstring` |  |
| `params` | `cstring` |  |
| `isLuaScript` | `bool` |  |

### ConsoleScriptParameter

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `description` | `string` |  |
