# SkillInfo

Namespace `C_SkillInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/skillinfodocumentation.lua` (FileDataID 4637242)

## Functions

### AbandonSkill

```lua
C_SkillInfo.AbandonSkill(skillLineID: number)
```

`SecretArguments=AllowedWhenUntainted`

### CollapseSkillHeader

```lua
C_SkillInfo.CollapseSkillHeader(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### ExpandSkillHeader

```lua
C_SkillInfo.ExpandSkillHeader(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetNumSkillLines

```lua
C_SkillInfo.GetNumSkillLines() -> numSkillLines: number
```

### GetSelectedSkill

```lua
C_SkillInfo.GetSelectedSkill() -> index: luaIndex
```

### GetSkillLineInfo

```lua
C_SkillInfo.GetSkillLineInfo(index: luaIndex) -> skillLineAttributes: SkillLineAttributes?
```

`SecretArguments=AllowedWhenUntainted`

### GetSkillLineInfoByID

```lua
C_SkillInfo.GetSkillLineInfoByID(ID: number) -> skillLineAttributes: SkillLineAttributes?
```

`SecretArguments=AllowedWhenUntainted`

### SetSelectedSkill

```lua
C_SkillInfo.SetSelectedSkill(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SKILL_LINES_CHANGED

```lua
SKILL_LINES_CHANGED()
```

`SynchronousEvent`

## Types

### SkillLineAttributes

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `skillID` | `number` |  |
| `name` | `cstring` |  |
| `isHeader` | `bool` |  |
| `isCollapsed` | `bool` |  |
| `rank` | `number` |  |
| `tempPoints` | `number` |  |
| `modifier` | `number` |  |
| `maxRank` | `number` |  |
| `isAbandonable` | `bool` |  |
| `stepCost` | `number` |  |
| `rankCost` | `number` |  |
| `minLevel` | `number` |  |
| `costType` | `number` |  |
| `parentSkillLineID` | `number` |  |
| `skillLineCategoryID` | `number` |  |
| `description` | `cstring` |  |
