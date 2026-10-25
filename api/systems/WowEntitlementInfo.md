# WowEntitlementInfo

Namespace `C_WowEntitlementInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/wowentitlementinfodocumentation.lua` (FileDataID 4637300)

## Events

### ENTITLEMENT_DELIVERED

```lua
ENTITLEMENT_DELIVERED(entitlementType: WoWEntitlementType, textureID: number, name: string, payloadID: number?, showFancyToast: bool)
```

`SynchronousEvent`

### RAF_ENTITLEMENT_DELIVERED

```lua
RAF_ENTITLEMENT_DELIVERED(entitlementType: WoWEntitlementType, textureID: number, name: string, payloadID: number?, showFancyToast: bool, rafVersion: RecruitAFriendRewardsVersion)
```

`SynchronousEvent`

## Types

### WoWEntitlementType

*Enumeration* · 10 values, 0..9

Access values as `Enum.WoWEntitlementType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Item` | `WoWEntitlementType` | = 0 |
| `Mount` | `WoWEntitlementType` | = 1 |
| `Battlepet` | `WoWEntitlementType` | = 2 |
| `Toy` | `WoWEntitlementType` | = 3 |
| `Appearance` | `WoWEntitlementType` | = 4 |
| `AppearanceSet` | `WoWEntitlementType` | = 5 |
| `GameTime` | `WoWEntitlementType` | = 6 |
| `Title` | `WoWEntitlementType` | = 7 |
| `Illusion` | `WoWEntitlementType` | = 8 |
| `Invalid` | `WoWEntitlementType` | = 9 |
