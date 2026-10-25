# PartyInfo

Namespace `C_PartyInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/partyinfodocumentation.lua` (FileDataID 4637155)

## Functions

### AllowedToDoPartyConversion

```lua
C_PartyInfo.AllowedToDoPartyConversion(toRaid: bool) -> allowed: bool
```

`SecretArguments=AllowedWhenUntainted`

### CanFormCrossFactionParties

```lua
C_PartyInfo.CanFormCrossFactionParties() -> canFormCrossFactionParties: bool
```

### CanInvite

```lua
C_PartyInfo.CanInvite() -> allowedToInvite: bool
```

### CanStartInstanceAbandonVote

```lua
C_PartyInfo.CanStartInstanceAbandonVote() -> canStart: bool
```

Returns whether it's possible to start a vote at this time

### ChallengeModeRestrictionsActive

```lua
C_PartyInfo.ChallengeModeRestrictionsActive() -> restrictionsActive: bool
```

### ConfirmConvertToRaid

```lua
C_PartyInfo.ConfirmConvertToRaid()
```

Immediately convert to raid with no regard for potentially destructive actions.

`HasRestrictions`

### ConfirmInviteTravelPass

```lua
C_PartyInfo.ConfirmInviteTravelPass(targetName: cstring, targetGUID: WOWGUID)
```

`SecretArguments=AllowedWhenUntainted`

### ConfirmInviteUnit

```lua
C_PartyInfo.ConfirmInviteUnit(targetName: cstring)
```

Immediately invites the named unit to a party, with no regard for potentially destructive actions.

`SecretArguments=AllowedWhenUntainted` `RequiresValidInviteTarget`

### ConfirmLeaveParty

```lua
C_PartyInfo.ConfirmLeaveParty(category: luaIndex?)
```

Immediately leave the party with no regard for potentially destructive actions

`SecretArguments=AllowedWhenUntainted`

### ConfirmReadyCheck

```lua
C_PartyInfo.ConfirmReadyCheck(isReady: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### ConfirmRequestInviteFromUnit

```lua
C_PartyInfo.ConfirmRequestInviteFromUnit(targetName: cstring, tank: bool?, healer: bool?, dps: bool?)
```

Immediately request an invite into the target party, this is the confirmation function to call after RequestInviteFromUnit, or if you would like to skip the confirmation process.

`SecretArguments=AllowedWhenUntainted` `RequiresValidInviteTarget`

### ConvertToParty

```lua
C_PartyInfo.ConvertToParty()
```

`HasRestrictions`

### ConvertToRaid

```lua
C_PartyInfo.ConvertToRaid()
```

Usually this will convert to raid immediately. In some cases (e.g. PartySync) the user will be prompted to confirm converting to raid, because it's potentially destructive.

`HasRestrictions`

### DelveTeleportOut

```lua
C_PartyInfo.DelveTeleportOut()
```

### DemoteAssistant

```lua
C_PartyInfo.DemoteAssistant(name: cstring, exactNameMatch: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### DoCountdown

```lua
C_PartyInfo.DoCountdown(seconds: number) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### DoReadyCheck

```lua
C_PartyInfo.DoReadyCheck()
```

`HasRestrictions`

### GetActiveCategories

```lua
C_PartyInfo.GetActiveCategories() -> categories: number[]
```

`MayReturnNothing`

### GetAvailableLootMethods

```lua
C_PartyInfo.GetAvailableLootMethods() -> methods: LootMethod[]
```

### GetInstanceAbandonShutdownTime

```lua
C_PartyInfo.GetInstanceAbandonShutdownTime() -> durationSeconds: number, timeLeftSeconds: number
```

Returns the total duration of the shutdown time after a vote passes and how much time is left before it ends

Returns:

| Name | Type | Notes |
|---|---|---|
| `durationSeconds` | `number` | default `0` |
| `timeLeftSeconds` | `number` | default `0` |

### GetInstanceAbandonVoteCooldownTime

```lua
C_PartyInfo.GetInstanceAbandonVoteCooldownTime() -> durationSeconds: number, timeLeftSeconds: number
```

Returns the total duration of the abandon vote cooldown and how much time is left before it ends

`MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `durationSeconds` | `number` | default `0` |
| `timeLeftSeconds` | `number` | default `0` |

### GetInstanceAbandonVoteRequirements

```lua
C_PartyInfo.GetInstanceAbandonVoteRequirements() -> votesRequired: number, keystoneOwnerVoteWeight: number
```

Returns values controlling the vote

Returns:

| Name | Type | Notes |
|---|---|---|
| `votesRequired` | `number` | default `0` |
| `keystoneOwnerVoteWeight` | `number` | default `0` |

### GetInstanceAbandonVoteResponse

```lua
C_PartyInfo.GetInstanceAbandonVoteResponse() -> response: bool?
```

Returns how the player voted, nil for not yet

### GetInstanceAbandonVoteTime

```lua
C_PartyInfo.GetInstanceAbandonVoteTime() -> durationSeconds: number, timeLeftSeconds: number
```

Returns the total duration of the vote and how much time is left before it ends

Returns:

| Name | Type | Notes |
|---|---|---|
| `durationSeconds` | `number` | default `0` |
| `timeLeftSeconds` | `number` | default `0` |

### GetInviteConfirmationInvalidQueues

```lua
C_PartyInfo.GetInviteConfirmationInvalidQueues(inviteGUID: WOWGUID) -> invalidQueues: QueueSpecificInfo[]
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetInviteReferralInfo

```lua
C_PartyInfo.GetInviteReferralInfo(inviteGUID: WOWGUID) -> outReferredByGuid: WOWGUID, outReferredByName: cstring, outRelationType: PartyRequestJoinRelation, outIsQuickJoin: bool, outClubId: ClubId
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetLootMethod

```lua
C_PartyInfo.GetLootMethod() -> method: LootMethod, masterLootPartyID: number?, masterLooterRaidID: number?
```

### GetLootMethodStyle

```lua
C_PartyInfo.GetLootMethodStyle() -> methodStyle: LootMethodStyles
```

### GetMinItemLevel

```lua
C_PartyInfo.GetMinItemLevel(avgItemLevelCategory: AvgItemLevelCategories) -> minItemLevel: number, playerNameWithLowestItemLevel: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `avgItemLevelCategory` | `AvgItemLevelCategories` | The active party is always used |

### GetMinLevel

```lua
C_PartyInfo.GetMinLevel(category: luaIndex?) -> minLevel: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `category` | `luaIndex?` | If not provided, the active party is used |

### GetNumInstanceAbandonGroupVoteResponses

```lua
C_PartyInfo.GetNumInstanceAbandonGroupVoteResponses() -> count: number
```

Returns how many players have voted either way

### GetRestrictPings

```lua
C_PartyInfo.GetRestrictPings() -> restrictTo: RestrictPingsTo
```

### InviteUnit

```lua
C_PartyInfo.InviteUnit(targetName: cstring)
```

Attempt to invite the named unit to a party, requires confirmation in some cases (e.g. the party will convert to a raid, or if there is a party sync in progress).

`SecretArguments=AllowedWhenUntainted` `RequiresValidInviteTarget`

### IsChallengeModeActive

```lua
C_PartyInfo.IsChallengeModeActive() -> active: bool
```

### IsChallengeModeKeystoneOwner

```lua
C_PartyInfo.IsChallengeModeKeystoneOwner() -> isKeystoneOwner: bool
```

### IsCrossFactionParty

```lua
C_PartyInfo.IsCrossFactionParty(category: luaIndex?) -> isCrossFactionParty: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `category` | `luaIndex?` | If not provided, the active party is used |

### IsDelveComplete

```lua
C_PartyInfo.IsDelveComplete() -> isDelveComplete: bool
```

### IsDelveInProgress

```lua
C_PartyInfo.IsDelveInProgress() -> isDelveComplete: bool
```

### IsGUIDInGroup

```lua
C_PartyInfo.IsGUIDInGroup(guid: WOWGUID, category: luaIndex?) -> isInGroup: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `guid` | `WOWGUID` |  |
| `category` | `luaIndex?` | If not provided, the active party is used |

### IsLootMethodAvailable

```lua
C_PartyInfo.IsLootMethodAvailable(method: LootMethod) -> available: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPartyFull

```lua
C_PartyInfo.IsPartyFull(category: luaIndex?) -> isFull: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `category` | `luaIndex?` | If not provided, the active party is used |

### IsPartyInJailersTower

```lua
C_PartyInfo.IsPartyInJailersTower() -> isPartyInJailersTower: bool
```

### IsPartyWalkIn

```lua
C_PartyInfo.IsPartyWalkIn() -> isPartyWalkIn: bool
```

### LeaveParty

```lua
C_PartyInfo.LeaveParty(category: luaIndex?)
```

Usually this will leave the party immediately. In some cases (e.g. PartySync) the user will be prompted to confirm leaving the party, because it's potentially destructive

`SecretArguments=AllowedWhenUntainted`

### PromoteToAssistant

```lua
C_PartyInfo.PromoteToAssistant(name: cstring, exactNameMatch: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### PromoteToLeader

```lua
C_PartyInfo.PromoteToLeader(name: cstring, exactNameMatch: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RequestInviteFromUnit

```lua
C_PartyInfo.RequestInviteFromUnit(targetName: cstring, tank: bool?, healer: bool?, dps: bool?)
```

Attempt to request an invite into the target party, requires confirmation in some cases (e.g. there is a party sync in progress).

`SecretArguments=AllowedWhenUntainted` `RequiresValidInviteTarget`

### SetEveryoneIsAssistant

```lua
C_PartyInfo.SetEveryoneIsAssistant(isAssistant: bool) -> updated: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetInstanceAbandonVoteResponse

```lua
C_PartyInfo.SetInstanceAbandonVoteResponse(response: bool)
```

Vote on whether to abandon instance, true for yes, false for no

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetLootMethod

```lua
C_PartyInfo.SetLootMethod(method: LootMethod, lootMaster: string?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetRestrictPings

```lua
C_PartyInfo.SetRestrictPings(restrictTo: RestrictPingsTo)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### StartInstanceAbandonVote

```lua
C_PartyInfo.StartInstanceAbandonVote()
```

Start the vote

`HasRestrictions`

### UninviteUnit

```lua
C_PartyInfo.UninviteUnit(name: cstring, reason: cstring?, exactNameMatch: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### BNET_REQUEST_INVITE_CONFIRMATION

```lua
BNET_REQUEST_INVITE_CONFIRMATION(gameAccountID: number, questSessionActive: bool, tank: bool, healer: bool, dps: bool)
```

`SynchronousEvent`

### CONVERT_TO_RAID_CONFIRMATION

```lua
CONVERT_TO_RAID_CONFIRMATION()
```

`SynchronousEvent`

### ENTERED_DIFFERENT_INSTANCE_FROM_PARTY

```lua
ENTERED_DIFFERENT_INSTANCE_FROM_PARTY()
```

`SynchronousEvent`

### GROUP_FORMED

```lua
GROUP_FORMED(category: number, partyGUID: WOWGUID)
```

`SynchronousEvent`

### GROUP_INVITE_CONFIRMATION

```lua
GROUP_INVITE_CONFIRMATION()
```

`SynchronousEvent`

### GROUP_JOINED

```lua
GROUP_JOINED(category: number, partyGUID: WOWGUID)
```

`SynchronousEvent`

### GROUP_LEFT

```lua
GROUP_LEFT(category: number, partyGUID: WOWGUID)
```

`SynchronousEvent`

### GROUP_ROSTER_UPDATE

```lua
GROUP_ROSTER_UPDATE()
```

`UniqueEvent`

### INSTANCE_ABANDON_VOTE_FINISHED

```lua
INSTANCE_ABANDON_VOTE_FINISHED(votePassed: bool)
```

`SynchronousEvent`

### INSTANCE_ABANDON_VOTE_STARTED

```lua
INSTANCE_ABANDON_VOTE_STARTED()
```

`SynchronousEvent`

### INSTANCE_ABANDON_VOTE_UPDATED

```lua
INSTANCE_ABANDON_VOTE_UPDATED()
```

`SynchronousEvent`

### INSTANCE_BOOT_START

```lua
INSTANCE_BOOT_START()
```

`SynchronousEvent`

### INSTANCE_BOOT_STOP

```lua
INSTANCE_BOOT_STOP()
```

`SynchronousEvent`

### INSTANCE_GROUP_SIZE_CHANGED

```lua
INSTANCE_GROUP_SIZE_CHANGED()
```

`SynchronousEvent`

### INVITE_TO_PARTY_CONFIRMATION

```lua
INVITE_TO_PARTY_CONFIRMATION(targetName: cstring, willConvertToRaid: bool, questSessionActive: bool)
```

`SynchronousEvent`

### INVITE_TRAVEL_PASS_CONFIRMATION

```lua
INVITE_TRAVEL_PASS_CONFIRMATION(targetName: cstring, targetGUID: WOWGUID, willConvertToRaid: bool, questSessionActive: bool)
```

`SynchronousEvent`

### LEAVE_PARTY_CONFIRMATION

```lua
LEAVE_PARTY_CONFIRMATION(reason: LeavePartyConfirmReason)
```

`SynchronousEvent`

### PARTY_INVITE_CANCEL

```lua
PARTY_INVITE_CANCEL()
```

`SynchronousEvent`

### PARTY_INVITE_REQUEST

```lua
PARTY_INVITE_REQUEST(name: cstring, isTank: bool, isHealer: bool, isDamage: bool, isNativeRealm: bool, allowMultipleRoles: bool, inviterGUID: WOWGUID, questSessionActive: bool)
```

`SynchronousEvent`

### PARTY_LEADER_CHANGED

```lua
PARTY_LEADER_CHANGED()
```

`UniqueEvent`

### PARTY_LFG_RESTRICTED

```lua
PARTY_LFG_RESTRICTED()
```

`SynchronousEvent`

### PARTY_LOOT_METHOD_CHANGED

```lua
PARTY_LOOT_METHOD_CHANGED()
```

`UniqueEvent`

### PARTY_MEMBER_DISABLE

```lua
PARTY_MEMBER_DISABLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PARTY_MEMBER_ENABLE

```lua
PARTY_MEMBER_ENABLE(unitTarget: UnitTokenVariant)
```

`SynchronousEvent`

### PLAYER_DIFFICULTY_CHANGED

```lua
PLAYER_DIFFICULTY_CHANGED()
```

`SynchronousEvent`

### PLAYER_ROLES_ASSIGNED

```lua
PLAYER_ROLES_ASSIGNED()
```

`UniqueEvent`

### RAID_ROSTER_UPDATE

```lua
RAID_ROSTER_UPDATE()
```

`SynchronousEvent`

### READY_CHECK

```lua
READY_CHECK(initiatorName: cstring, readyCheckTimeLeft: time_t)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### READY_CHECK_CONFIRM

```lua
READY_CHECK_CONFIRM(unitTarget: UnitTokenVariant, isReady: bool)
```

`SynchronousEvent`

### READY_CHECK_FINISHED

```lua
READY_CHECK_FINISHED(preempted: bool)
```

`SynchronousEvent`

### REQUEST_INVITE_CONFIRMATION

```lua
REQUEST_INVITE_CONFIRMATION(targetName: cstring, partyLevelLink: number, questSessionActive: bool, tank: bool?, healer: bool?, dps: bool?)
```

`SynchronousEvent`

### VOTE_KICK_REASON_NEEDED

```lua
VOTE_KICK_REASON_NEEDED(name: cstring, resultGUID: WOWGUID)
```

`SynchronousEvent`

## Types

### LeavePartyConfirmReason

*Enumeration* · 2 values, 0..1

Access values as `Enum.LeavePartyConfirmReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `QuestSync` | `LeavePartyConfirmReason` | = 0 |
| `RestrictedChallengeMode` | `LeavePartyConfirmReason` | = 1 |

## Predicates

Conditions referenced by the flags above.

- `RequiresValidInviteTarget` *Precondition* (failure mode: ReturnNothing)
