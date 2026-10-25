# ConfigurationWarnings

Namespace `C_ConfigurationWarnings` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/configurationwarningsdocumentation.lua` (FileDataID 4637071)

## Functions

### GetConfigurationWarnings

```lua
C_ConfigurationWarnings.GetConfigurationWarnings(includeSeenWarnings: bool) -> configurationWarnings: ConfigurationWarning[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `includeSeenWarnings` | `bool` | default `false` |

### GetConfigurationWarningSeen

```lua
C_ConfigurationWarnings.GetConfigurationWarningSeen(configurationWarning: ConfigurationWarning) -> hasSeenConfigurationWarning: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetConfigurationWarningString

```lua
C_ConfigurationWarnings.GetConfigurationWarningString(configurationWarning: ConfigurationWarning) -> configurationWarningString: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### SetConfigurationWarningSeen

```lua
C_ConfigurationWarnings.SetConfigurationWarningSeen(configurationWarning: ConfigurationWarning)
```

`SecretArguments=AllowedWhenUntainted`
