# SecretWrapperConstants

source `interface/addons/blizzard_apidocumentationgenerated/secretwrapperconstantsdocumentation.lua` (FileDataID 7713906)

## Types

### SecrecyLevel

*Enumeration* · 3 values, 0..2

Access values as `Enum.SecrecyLevel.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `NeverSecret` | `SecrecyLevel` | = 0; Will never yield secret values when queried. |
| `AlwaysSecret` | `SecrecyLevel` | = 1; Will always yield secret values when queried. |
| `ContextuallySecret` | `SecrecyLevel` | = 2; May yield secret values when queried depending upon factors such as addon restriction states, unit disposition, etc. |
