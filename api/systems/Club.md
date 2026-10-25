# Club

Namespace `C_Club` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/clubdocumentation.lua` (FileDataID 4637063)

## Functions

### AcceptInvitation

```lua
C_Club.AcceptInvitation(clubId: ClubId)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### AddClubStreamChatChannel

```lua
C_Club.AddClubStreamChatChannel(clubId: ClubId, streamId: ClubStreamId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### AdvanceStreamViewMarker

```lua
C_Club.AdvanceStreamViewMarker(clubId: ClubId, streamId: ClubStreamId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### AreMembersReady

```lua
C_Club.AreMembersReady(clubId: ClubId) -> membersReady: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### AssignMemberRole

```lua
C_Club.AssignMemberRole(clubId: ClubId, memberId: ClubMemberOpaqueId, roleId: ClubRoleIdentifier)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### CanResolvePlayerLocationFromClubMessageData

```lua
C_Club.CanResolvePlayerLocationFromClubMessageData(clubId: ClubId, streamId: ClubStreamId, epoch: BigUInteger, position: BigUInteger) -> canResolve: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### ClearAutoAdvanceStreamViewMarker

```lua
C_Club.ClearAutoAdvanceStreamViewMarker()
```

`RequiresClubsInitialized`

### ClearClubPresenceSubscription

```lua
C_Club.ClearClubPresenceSubscription()
```

`RequiresClubsInitialized`

### CompareBattleNetDisplayName

```lua
C_Club.CompareBattleNetDisplayName(clubId: ClubId, lhsMemberId: number, rhsMemberId: number) -> comparison: number
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### CreateClub

```lua
C_Club.CreateClub(name: string, shortName: string?, description: string, clubType: ClubType, avatarId: number, isCrossFaction: bool?)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `shortName` | `string?` |  |
| `description` | `string` |  |
| `clubType` | `ClubType` | Valid types are BattleNet or Character |
| `avatarId` | `number` |  |
| `isCrossFaction` | `bool?` |  |

### CreateStream

```lua
C_Club.CreateStream(clubId: ClubId, name: string, subject: string, leadersAndModeratorsOnly: bool)
```

Check the canCreateStream privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### CreateTicket

```lua
C_Club.CreateTicket(clubId: ClubId, allowedRedeemCount: number?, duration: number?, defaultStreamId: ClubStreamId?, isCrossFaction: bool?)
```

Check canCreateTicket privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `clubId` | `ClubId` |  |
| `allowedRedeemCount` | `number?` | Number of uses. nil means unlimited |
| `duration` | `number?` | Duration in seconds. nil never expires |
| `defaultStreamId` | `ClubStreamId?` |  |
| `isCrossFaction` | `bool?` |  |

### DeclineInvitation

```lua
C_Club.DeclineInvitation(clubId: ClubId)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### DestroyClub

```lua
C_Club.DestroyClub(clubId: ClubId)
```

Check the canDestroy privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### DestroyMessage

```lua
C_Club.DestroyMessage(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### DestroyStream

```lua
C_Club.DestroyStream(clubId: ClubId, streamId: ClubStreamId)
```

Check canDestroyStream privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### DestroyTicket

```lua
C_Club.DestroyTicket(clubId: ClubId, ticketId: string)
```

Check canDestroyTicket privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### DoesAnyCommunityHaveUnreadMessages

```lua
C_Club.DoesAnyCommunityHaveUnreadMessages() -> hasUnreadMessages: bool
```

`RequiresClubsInitialized`

### DoesCommunityHaveMembersOfTheOppositeFaction

```lua
C_Club.DoesCommunityHaveMembersOfTheOppositeFaction(clubId: ClubId) -> hasMembersOfOppositeFaction: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### EditClub

```lua
C_Club.EditClub(clubId: ClubId, name: string?, shortName: string?, description: string?, avatarId: number?, broadcast: string?, crossFaction: bool?)
```

nil arguments will not change existing club data

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### EditMessage

```lua
C_Club.EditMessage(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier, message: string)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### EditStream

```lua
C_Club.EditStream(clubId: ClubId, streamId: ClubStreamId, name: string?, subject: string?, leadersAndModeratorsOnly: bool?)
```

Check the canSetStreamName, canSetStreamSubject, canSetStreamAccess privileges. nil arguments will not change existing stream data.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### Flush

```lua
C_Club.Flush()
```

`RequiresClubsInitialized`

### FocusCommunityStreams

```lua
C_Club.FocusCommunityStreams()
```

`RequiresClubsInitialized`

### FocusMembers

```lua
C_Club.FocusMembers(clubId: ClubId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### FocusStream

```lua
C_Club.FocusStream(clubId: ClubId, streamId: ClubStreamId) -> focused: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetAssignableRoles

```lua
C_Club.GetAssignableRoles(clubId: ClubId, memberId: ClubMemberOpaqueId) -> assignableRoles: ClubRoleIdentifier[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetAvatarIdList

```lua
C_Club.GetAvatarIdList(clubType: ClubType) -> avatarIds: number[]?
```

listen for AVATAR_LIST_UPDATED event. This can happen if we haven't downloaded the battle.net avatar list yet

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetClubCapacity

```lua
C_Club.GetClubCapacity() -> capacity: number
```

`RequiresClubsInitialized`

### GetClubInfo

```lua
C_Club.GetClubInfo(clubId: ClubId) -> info: ClubInfo?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetClubLimits

```lua
C_Club.GetClubLimits(clubType: ClubType) -> clubLimits: ClubLimits
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetClubMembers

```lua
C_Club.GetClubMembers(clubId: ClubId, streamId: ClubStreamId?) -> members: ClubMemberOpaqueId[]
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetClubPrivileges

```lua
C_Club.GetClubPrivileges(clubId: ClubId) -> privilegeInfo: ClubPrivilegeInfo
```

The privileges for the logged in user for this club

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetClubStreamNotificationSettings

```lua
C_Club.GetClubStreamNotificationSettings(clubId: ClubId) -> settings: ClubStreamNotificationSetting[]
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetCommunityNameResultText

```lua
C_Club.GetCommunityNameResultText(result: ValidateNameResult) -> errorCode: cstring?
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetGuildClubId

```lua
C_Club.GetGuildClubId() -> guildClubId: ClubId?
```

`RequiresClubsInitialized`

### GetInfoFromLastCommunityChatLine

```lua
C_Club.GetInfoFromLastCommunityChatLine() -> messageInfo: ClubMessageInfo, clubId: ClubId, streamId: ClubStreamId, clubType: ClubType
```

`MayReturnNothing` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetInvitationCandidates

```lua
C_Club.GetInvitationCandidates(filter: string?, maxResults: number?, cursorPosition: number?, allowFullMatch: bool?, clubId: ClubId) -> candidates: ClubInvitationCandidateInfo[]
```

Returns a list of players that you can send a request to a Battle.net club. Returns an empty list for Character based clubs

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetInvitationInfo

```lua
C_Club.GetInvitationInfo(clubId: ClubId) -> invitation: ClubSelfInvitationInfo?
```

Get info about a specific club the active player has been invited to.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetInvitationsForClub

```lua
C_Club.GetInvitationsForClub(clubId: ClubId) -> invitations: ClubInvitationInfo[]
```

Get the pending invitations for this club. Call RequestInvitationsForClub() to retrieve invitations from server.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetInvitationsForSelf

```lua
C_Club.GetInvitationsForSelf() -> invitations: ClubSelfInvitationInfo[]
```

These are the clubs the active player has been invited to.

`RequiresClubsInitialized`

### GetLastTicketResponse

```lua
C_Club.GetLastTicketResponse(ticket: string) -> error: ClubErrorType, info: ClubInfo?, showError: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `HasRestrictions` `RequiresClubsInitialized`

### GetMemberInfo

```lua
C_Club.GetMemberInfo(clubId: ClubId, memberId: ClubMemberOpaqueId) -> info: ClubMemberInfo?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetMemberInfoForSelf

```lua
C_Club.GetMemberInfoForSelf(clubId: ClubId) -> info: ClubMemberInfo?
```

Info for the logged in user for this club

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### GetMessageInfo

```lua
C_Club.GetMessageInfo(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier) -> message: ClubMessageInfo?
```

Get info about a particular message.

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetMessageRanges

```lua
C_Club.GetMessageRanges(clubId: ClubId, streamId: ClubStreamId) -> ranges: ClubMessageRange[]
```

Get the ranges of the messages currently downloaded.

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetMessagesBefore

```lua
C_Club.GetMessagesBefore(clubId: ClubId, streamId: ClubStreamId, newest: ClubMessageIdentifier, count: number) -> messages: ClubMessageInfo[]
```

Get downloaded messages before (and including) the specified messageId limited by count. These are filtered by ignored players

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetMessagesInRange

```lua
C_Club.GetMessagesInRange(clubId: ClubId, streamId: ClubStreamId, oldest: ClubMessageIdentifier, newest: ClubMessageIdentifier) -> messages: ClubMessageInfo[]
```

Get downloaded messages in the given range. These are filtered by ignored players

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetStreamInfo

```lua
C_Club.GetStreamInfo(clubId: ClubId, streamId: ClubStreamId) -> streamInfo: ClubStreamInfo?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetStreams

```lua
C_Club.GetStreams(clubId: ClubId) -> streams: ClubStreamInfo[]
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetStreamViewMarker

```lua
C_Club.GetStreamViewMarker(clubId: ClubId, streamId: ClubStreamId) -> lastReadTime: BigUInteger?
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

Returns:

| Name | Type | Notes |
|---|---|---|
| `lastReadTime` | `BigUInteger?` | nil if stream view is at current |

### GetSubscribedClubs

```lua
C_Club.GetSubscribedClubs() -> clubs: ClubInfo[]
```

`SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### GetTickets

```lua
C_Club.GetTickets(clubId: ClubId) -> tickets: ClubTicketInfo[]
```

Get the existing tickets for this club. Call RequestTickets() to retrieve tickets from server.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### IsAccountMuted

```lua
C_Club.IsAccountMuted(clubId: ClubId) -> accountMuted: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### IsBeginningOfStream

```lua
C_Club.IsBeginningOfStream(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier) -> isBeginningOfStream: bool
```

Returns whether the given message is the first message in the stream, taking into account ignored messages

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### IsEnabled

```lua
C_Club.IsEnabled() -> clubsEnabled: bool
```

`RequiresClubsInitialized`

### IsRestricted

```lua
C_Club.IsRestricted() -> restrictionReason: ClubRestrictionReason
```

`RequiresClubsInitialized`

### IsSubscribedToStream

```lua
C_Club.IsSubscribedToStream(clubId: ClubId, streamId: ClubStreamId) -> subscribed: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### KickMember

```lua
C_Club.KickMember(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

Check kickableRoleIds privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### LeaveClub

```lua
C_Club.LeaveClub(clubId: ClubId)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### RedeemTicket

```lua
C_Club.RedeemTicket(ticketId: string)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### RequestInvitationsForClub

```lua
C_Club.RequestInvitationsForClub(clubId: ClubId)
```

Request invitations for this club from server. Check canGetInvitation privilege.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### RequestMoreMessagesBefore

```lua
C_Club.RequestMoreMessagesBefore(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier?, count: number?) -> alreadyHasMessages: bool
```

Call this when the user scrolls near the top of the message view, and more need to be displayed. The history will be downloaded backwards (newest to oldest).

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown` `RequiresClubsInitialized`

### RequestTicket

```lua
C_Club.RequestTicket(ticketId: string)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### RequestTickets

```lua
C_Club.RequestTickets(clubId: ClubId)
```

Request tickets from server. Check canGetTicket privilege.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### RevokeInvitation

```lua
C_Club.RevokeInvitation(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

Check canRevokeOwnInvitation or canRevokeOtherInvitation

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SendBattleTagFriendRequest

```lua
C_Club.SendBattleTagFriendRequest(guildClubId: ClubId, memberId: ClubMemberOpaqueId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SendCharacterInvitation

```lua
C_Club.SendCharacterInvitation(clubId: ClubId, character: string)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SendInvitation

```lua
C_Club.SendInvitation(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

Check the canSendInvitation privilege.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SendMessage

```lua
C_Club.SendMessage(clubId: ClubId, streamId: ClubStreamId, message: string)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SendTitleFriendRequest

```lua
C_Club.SendTitleFriendRequest(guildClubId: ClubId, memberId: ClubMemberOpaqueId)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SetAutoAdvanceStreamViewMarker

```lua
C_Club.SetAutoAdvanceStreamViewMarker(clubId: ClubId, streamId: ClubStreamId)
```

Only one stream can be set for auto-advance at a time. Focused streams will have their view times advanced automatically.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SetAvatarTexture

```lua
C_Club.SetAvatarTexture(texture: SimpleTexture, avatarId: number, clubType: ClubType)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SetClubMemberNote

```lua
C_Club.SetClubMemberNote(clubId: ClubId, memberId: ClubMemberOpaqueId, note: string)
```

Check the canSetOwnMemberNote and canSetOtherMemberNote privileges.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions` `RequiresClubsInitialized`

### SetClubPresenceSubscription

```lua
C_Club.SetClubPresenceSubscription(clubId: ClubId)
```

You can only be subscribed to 0 or 1 clubs for presence.  Subscribing to a new club automatically unsuscribes you to existing subscription.

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SetClubStreamNotificationSettings

```lua
C_Club.SetClubStreamNotificationSettings(clubId: ClubId, settings: ClubStreamNotificationSetting[])
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SetCommunityID

```lua
C_Club.SetCommunityID(communityID: BigUInteger)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SetFavorite

```lua
C_Club.SetFavorite(clubId: ClubId, isFavorite: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### SetSocialQueueingEnabled

```lua
C_Club.SetSocialQueueingEnabled(clubId: ClubId, enabled: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### ShouldAllowClubType

```lua
C_Club.ShouldAllowClubType(clubType: ClubType) -> clubTypeIsAllowed: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### UnfocusAllStreams

```lua
C_Club.UnfocusAllStreams(unsubscribe: bool)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### UnfocusMembers

```lua
C_Club.UnfocusMembers(clubId: ClubId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### UnfocusStream

```lua
C_Club.UnfocusStream(clubId: ClubId, streamId: ClubStreamId)
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

### ValidateText

```lua
C_Club.ValidateText(clubType: ClubType, text: string, clubFieldType: ClubFieldType) -> result: ValidateNameResult
```

`SecretArguments=AllowedWhenUntainted` `RequiresClubsInitialized`

## Events

### AVATAR_LIST_UPDATED

```lua
AVATAR_LIST_UPDATED(clubType: ClubType)
```

`SynchronousEvent`

### CLUB_ADDED

```lua
CLUB_ADDED(clubId: ClubId)
```

`SynchronousEvent`

### CLUB_ERROR

```lua
CLUB_ERROR(action: ClubActionType, error: ClubErrorType, clubType: ClubType)
```

`SynchronousEvent`

### CLUB_INVITATION_ADDED_FOR_SELF

```lua
CLUB_INVITATION_ADDED_FOR_SELF(invitation: ClubSelfInvitationInfo)
```

`SynchronousEvent`

### CLUB_INVITATION_REMOVED_FOR_SELF

```lua
CLUB_INVITATION_REMOVED_FOR_SELF(invitationId: ClubInvitationId)
```

`SynchronousEvent`

### CLUB_INVITATIONS_RECEIVED_FOR_CLUB

```lua
CLUB_INVITATIONS_RECEIVED_FOR_CLUB(clubId: ClubId)
```

`SynchronousEvent`

### CLUB_MEMBER_ADDED

```lua
CLUB_MEMBER_ADDED(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

`SynchronousEvent`

### CLUB_MEMBER_PRESENCE_UPDATED

```lua
CLUB_MEMBER_PRESENCE_UPDATED(clubId: ClubId, memberId: ClubMemberOpaqueId, presence: ClubMemberPresence)
```

`SynchronousEvent`

### CLUB_MEMBER_REMOVED

```lua
CLUB_MEMBER_REMOVED(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

`SynchronousEvent`

### CLUB_MEMBER_ROLE_UPDATED

```lua
CLUB_MEMBER_ROLE_UPDATED(clubId: ClubId, memberId: ClubMemberOpaqueId, roleId: number)
```

`SynchronousEvent`

### CLUB_MEMBERS_UPDATED

```lua
CLUB_MEMBERS_UPDATED(clubId: ClubId)
```

`UniqueEvent`

### CLUB_MEMBER_UPDATED

```lua
CLUB_MEMBER_UPDATED(clubId: ClubId, memberId: ClubMemberOpaqueId)
```

`SynchronousEvent`

### CLUB_MESSAGE_ADDED

```lua
CLUB_MESSAGE_ADDED(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier)
```

`SynchronousEvent`

### CLUB_MESSAGE_HISTORY_RECEIVED

```lua
CLUB_MESSAGE_HISTORY_RECEIVED(clubId: ClubId, streamId: ClubStreamId, downloadedRange: ClubMessageRange, contiguousRange: ClubMessageRange)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `clubId` | `ClubId` |  |
| `streamId` | `ClubStreamId` |  |
| `downloadedRange` | `ClubMessageRange` | Range of history messages received. |
| `contiguousRange` | `ClubMessageRange` | Range of contiguous messages that the received messages are in. |

### CLUB_MESSAGE_UPDATED

```lua
CLUB_MESSAGE_UPDATED(clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier)
```

`SynchronousEvent`

### CLUB_REMOVED

```lua
CLUB_REMOVED(clubId: ClubId)
```

`SynchronousEvent`

### CLUB_REMOVED_MESSAGE

```lua
CLUB_REMOVED_MESSAGE(clubName: string, clubRemovedReason: ClubRemovedReason)
```

`SynchronousEvent`

### CLUB_SELF_MEMBER_ROLE_UPDATED

```lua
CLUB_SELF_MEMBER_ROLE_UPDATED(clubId: ClubId, roleId: number)
```

`SynchronousEvent`

### CLUB_STREAM_ADDED

```lua
CLUB_STREAM_ADDED(clubId: ClubId, streamId: ClubStreamId)
```

`SynchronousEvent` `UniqueEvent`

### CLUB_STREAM_REMOVED

```lua
CLUB_STREAM_REMOVED(clubId: ClubId, streamId: ClubStreamId)
```

`SynchronousEvent` `UniqueEvent`

### CLUB_STREAMS_LOADED

```lua
CLUB_STREAMS_LOADED(clubId: ClubId)
```

`SynchronousEvent`

### CLUB_STREAM_SUBSCRIBED

```lua
CLUB_STREAM_SUBSCRIBED(clubId: ClubId, streamId: ClubStreamId)
```

`SynchronousEvent`

### CLUB_STREAM_UNSUBSCRIBED

```lua
CLUB_STREAM_UNSUBSCRIBED(clubId: ClubId, streamId: ClubStreamId)
```

`SynchronousEvent`

### CLUB_STREAM_UPDATED

```lua
CLUB_STREAM_UPDATED(clubId: ClubId, streamId: ClubStreamId)
```

`SynchronousEvent` `UniqueEvent`

### CLUB_TICKET_CREATED

```lua
CLUB_TICKET_CREATED(clubId: ClubId, ticketInfo: ClubTicketInfo)
```

`SynchronousEvent`

### CLUB_TICKET_RECEIVED

```lua
CLUB_TICKET_RECEIVED(ticket: string)
```

`SynchronousEvent`

### CLUB_TICKETS_RECEIVED

```lua
CLUB_TICKETS_RECEIVED(clubId: ClubId)
```

`SynchronousEvent`

### CLUB_UPDATED

```lua
CLUB_UPDATED(clubId: ClubId)
```

`SynchronousEvent`

### INITIAL_CLUBS_LOADED

```lua
INITIAL_CLUBS_LOADED()
```

`SynchronousEvent`

### STREAM_VIEW_MARKER_UPDATED

```lua
STREAM_VIEW_MARKER_UPDATED(clubId: ClubId, streamId: ClubStreamId, lastReadTime: BigUInteger?)
```

`SynchronousEvent` `UniqueEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `clubId` | `ClubId` |  |
| `streamId` | `ClubStreamId` |  |
| `lastReadTime` | `BigUInteger?` | nil if stream view is at current |

## Types

### ClubActionType

*Enumeration* · 27 values, 0..26

Access values as `Enum.ClubActionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ErrorClubActionSubscribe` | `ClubActionType` | = 0 |
| `ErrorClubActionCreate` | `ClubActionType` | = 1 |
| `ErrorClubActionEdit` | `ClubActionType` | = 2 |
| `ErrorClubActionDestroy` | `ClubActionType` | = 3 |
| `ErrorClubActionLeave` | `ClubActionType` | = 4 |
| `ErrorClubActionCreateTicket` | `ClubActionType` | = 5 |
| `ErrorClubActionDestroyTicket` | `ClubActionType` | = 6 |
| `ErrorClubActionRedeemTicket` | `ClubActionType` | = 7 |
| `ErrorClubActionGetTicket` | `ClubActionType` | = 8 |
| `ErrorClubActionGetTickets` | `ClubActionType` | = 9 |
| `ErrorClubActionGetBans` | `ClubActionType` | = 10 |
| `ErrorClubActionGetInvitations` | `ClubActionType` | = 11 |
| `ErrorClubActionRevokeInvitation` | `ClubActionType` | = 12 |
| `ErrorClubActionAcceptInvitation` | `ClubActionType` | = 13 |
| `ErrorClubActionDeclineInvitation` | `ClubActionType` | = 14 |
| `ErrorClubActionCreateStream` | `ClubActionType` | = 15 |
| `ErrorClubActionEditStream` | `ClubActionType` | = 16 |
| `ErrorClubActionDestroyStream` | `ClubActionType` | = 17 |
| `ErrorClubActionInviteMember` | `ClubActionType` | = 18 |
| `ErrorClubActionEditMember` | `ClubActionType` | = 19 |
| `ErrorClubActionEditMemberNote` | `ClubActionType` | = 20 |
| `ErrorClubActionKickMember` | `ClubActionType` | = 21 |
| `ErrorClubActionAddBan` | `ClubActionType` | = 22 |
| `ErrorClubActionRemoveBan` | `ClubActionType` | = 23 |
| `ErrorClubActionCreateMessage` | `ClubActionType` | = 24 |
| `ErrorClubActionEditMessage` | `ClubActionType` | = 25 |
| `ErrorClubActionDestroyMessage` | `ClubActionType` | = 26 |

### ClubErrorType

*Enumeration* · 42 values, 0..41

Access values as `Enum.ClubErrorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ErrorCommunitiesNone` | `ClubErrorType` | = 0 |
| `ErrorCommunitiesUnknown` | `ClubErrorType` | = 1 |
| `ErrorCommunitiesNeutralFaction` | `ClubErrorType` | = 2 |
| `ErrorCommunitiesUnknownRealm` | `ClubErrorType` | = 3 |
| `ErrorCommunitiesBadTarget` | `ClubErrorType` | = 4 |
| `ErrorCommunitiesWrongFaction` | `ClubErrorType` | = 5 |
| `ErrorCommunitiesRestricted` | `ClubErrorType` | = 6 |
| `ErrorCommunitiesIgnored` | `ClubErrorType` | = 7 |
| `ErrorCommunitiesGuild` | `ClubErrorType` | = 8 |
| `ErrorCommunitiesWrongRegion` | `ClubErrorType` | = 9 |
| `ErrorCommunitiesUnknownTicket` | `ClubErrorType` | = 10 |
| `ErrorCommunitiesMissingShortName` | `ClubErrorType` | = 11 |
| `ErrorCommunitiesProfanity` | `ClubErrorType` | = 12 |
| `ErrorCommunitiesTrial` | `ClubErrorType` | = 13 |
| `ErrorCommunitiesVeteranTrial` | `ClubErrorType` | = 14 |
| `ErrorCommunitiesChatMute` | `ClubErrorType` | = 15 |
| `ErrorClubFull` | `ClubErrorType` | = 16 |
| `ErrorClubNoClub` | `ClubErrorType` | = 17 |
| `ErrorClubNotMember` | `ClubErrorType` | = 18 |
| `ErrorClubAlreadyMember` | `ClubErrorType` | = 19 |
| `ErrorClubNoSuchMember` | `ClubErrorType` | = 20 |
| `ErrorClubNoSuchInvitation` | `ClubErrorType` | = 21 |
| `ErrorClubInvitationAlreadyExists` | `ClubErrorType` | = 22 |
| `ErrorClubInvalidRoleID` | `ClubErrorType` | = 23 |
| `ErrorClubInsufficientPrivileges` | `ClubErrorType` | = 24 |
| `ErrorClubTooManyClubsJoined` | `ClubErrorType` | = 25 |
| `ErrorClubVoiceFull` | `ClubErrorType` | = 26 |
| `ErrorClubStreamNoStream` | `ClubErrorType` | = 27 |
| `ErrorClubStreamInvalidName` | `ClubErrorType` | = 28 |
| `ErrorClubStreamCountAtMin` | `ClubErrorType` | = 29 |
| `ErrorClubStreamCountAtMax` | `ClubErrorType` | = 30 |
| `ErrorClubMemberHasRequiredRole` | `ClubErrorType` | = 31 |
| `ErrorClubSentInvitationCountAtMax` | `ClubErrorType` | = 32 |
| `ErrorClubReceivedInvitationCountAtMax` | `ClubErrorType` | = 33 |
| `ErrorClubTargetIsBanned` | `ClubErrorType` | = 34 |
| `ErrorClubBanAlreadyExists` | `ClubErrorType` | = 35 |
| `ErrorClubBanCountAtMax` | `ClubErrorType` | = 36 |
| `ErrorClubTicketCountAtMax` | `ClubErrorType` | = 37 |
| `ErrorClubTicketNoSuchTicket` | `ClubErrorType` | = 38 |
| `ErrorClubTicketHasConsumedAllowedRedeemCount` | `ClubErrorType` | = 39 |
| `ErrorClubDoesntAllowCrossFaction` | `ClubErrorType` | = 40 |
| `ErrorClubEditHasCrossFactionMembers` | `ClubErrorType` | = 41 |

### ClubFieldType

*Enumeration* · 7 values, 0..6

Access values as `Enum.ClubFieldType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ClubName` | `ClubFieldType` | = 0 |
| `ClubShortName` | `ClubFieldType` | = 1 |
| `ClubDescription` | `ClubFieldType` | = 2 |
| `ClubBroadcast` | `ClubFieldType` | = 3 |
| `ClubStreamName` | `ClubFieldType` | = 4 |
| `ClubStreamSubject` | `ClubFieldType` | = 5 |
| `NumTypes` | `ClubFieldType` | = 6 |

### ClubInvitationCandidateStatus

*Enumeration* · 3 values, 0..2

Access values as `Enum.ClubInvitationCandidateStatus.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Available` | `ClubInvitationCandidateStatus` | = 0 |
| `InvitePending` | `ClubInvitationCandidateStatus` | = 1 |
| `AlreadyMember` | `ClubInvitationCandidateStatus` | = 2 |

### ClubMemberPresence

*Enumeration* · 6 values, 0..5

Access values as `Enum.ClubMemberPresence.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unknown` | `ClubMemberPresence` | = 0 |
| `Online` | `ClubMemberPresence` | = 1 |
| `OnlineMobile` | `ClubMemberPresence` | = 2 |
| `Offline` | `ClubMemberPresence` | = 3 |
| `Away` | `ClubMemberPresence` | = 4 |
| `Busy` | `ClubMemberPresence` | = 5 |

### ClubRemovedReason

*Enumeration* · 4 values, 0..3

Access values as `Enum.ClubRemovedReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubRemovedReason` | = 0 |
| `Banned` | `ClubRemovedReason` | = 1 |
| `Removed` | `ClubRemovedReason` | = 2 |
| `ClubDestroyed` | `ClubRemovedReason` | = 3 |

### ClubRestrictionReason

*Enumeration* · 2 values, 0..1

Access values as `Enum.ClubRestrictionReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubRestrictionReason` | = 0 |
| `Unavailable` | `ClubRestrictionReason` | = 1 |

### ClubStreamNotificationFilter

*Enumeration* · 3 values, 0..2

Access values as `Enum.ClubStreamNotificationFilter.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `ClubStreamNotificationFilter` | = 0 |
| `Mention` | `ClubStreamNotificationFilter` | = 1 |
| `All` | `ClubStreamNotificationFilter` | = 2 |

### ClubStreamType

*Enumeration* · 5 values, 0..4

Access values as `Enum.ClubStreamType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `General` | `ClubStreamType` | = 0 |
| `Guild` | `ClubStreamType` | = 1 |
| `Officer` | `ClubStreamType` | = 2 |
| `Discord` | `ClubStreamType` | = 3 |
| `Other` | `ClubStreamType` | = 4 |

### ClubType

*Enumeration* · 4 values, 0..3

Access values as `Enum.ClubType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `BattleNet` | `ClubType` | = 0 |
| `Character` | `ClubType` | = 1 |
| `Guild` | `ClubType` | = 2 |
| `Other` | `ClubType` | = 3 |

### ClubInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `clubId` | `ClubId` | `NeverSecret` |
| `name` | `string` |  |
| `shortName` | `string?` |  |
| `description` | `string` |  |
| `broadcast` | `string` |  |
| `clubType` | `ClubType` | `NeverSecret` |
| `avatarId` | `number` |  |
| `memberCount` | `number?` | `NeverSecret` |
| `favoriteTimeStamp` | `BigUInteger?` |  |
| `joinTime` | `BigUInteger?` |  |
| `socialQueueingEnabled` | `bool?` |  |
| `crossFaction` | `bool?` |  |

### ClubInvitationCandidateInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `memberId` | `ClubMemberOpaqueId` |  |
| `name` | `string` |  |
| `priority` | `luaIndex` |  |
| `status` | `ClubInvitationCandidateStatus` |  |

### ClubInvitationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `invitationId` | `ClubInvitationId` |  |
| `isMyInvitation` | `bool` |  |
| `invitee` | `ClubMemberInfo` |  |

### ClubLimits

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maximumNumberOfStreams` | `number` |  |

### ClubMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isSelf` | `bool` | `NeverSecret` |
| `memberId` | `ClubMemberOpaqueId` |  |
| `name` | `string?` | name may be encoded as a Kstring |
| `role` | `ClubRoleIdentifier?` |  |
| `presence` | `ClubMemberPresence` |  |
| `clubType` | `ClubType?` |  |
| `guid` | `WOWGUID?` |  |
| `bnetAccountId` | `number?` |  |
| `memberNote` | `string?` |  |
| `officerNote` | `string?` |  |
| `classID` | `number?` |  |
| `race` | `number?` |  |
| `level` | `number?` |  |
| `zone` | `string?` |  |
| `achievementPoints` | `number?` |  |
| `profession1ID` | `number?` |  |
| `profession1Rank` | `number?` |  |
| `profession1Name` | `string?` |  |
| `profession2ID` | `number?` |  |
| `profession2Rank` | `number?` |  |
| `profession2Name` | `string?` |  |
| `lastOnlineYear` | `number?` |  |
| `lastOnlineMonth` | `number?` |  |
| `lastOnlineDay` | `number?` |  |
| `lastOnlineHour` | `number?` |  |
| `guildRank` | `string?` |  |
| `guildRankOrder` | `luaIndex?` |  |
| `isRemoteChat` | `bool?` |  |
| `overallDungeonScore` | `number?` |  |
| `faction` | `PvPFaction?` | `NeverSecret` |
| `timerunningSeasonID` | `number?` |  |
| `discordInfo` | `DiscordChatInfo?` |  |

### ClubMessageIdentifier

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `epoch` | `BigUInteger` | number of microseconds since the UNIX epoch. |
| `position` | `BigUInteger` | sort order for messages at the same time |

### ClubMessageInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `messageId` | `ClubMessageIdentifier` |  |
| `content` | `kstringClubMessage` |  |
| `author` | `ClubMemberInfo` |  |
| `destroyer` | `ClubMemberInfo?` | May be nil even if the message has been destroyed |
| `destroyed` | `bool` |  |
| `edited` | `bool` |  |

### ClubMessageRange

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `oldestMessageId` | `ClubMessageIdentifier` |  |
| `newestMessageId` | `ClubMessageIdentifier` |  |

### ClubPrivilegeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `canDestroy` | `bool` |  |
| `canSetAttribute` | `bool` |  |
| `canSetName` | `bool` |  |
| `canSetDescription` | `bool` |  |
| `canSetAvatar` | `bool` |  |
| `canSetBroadcast` | `bool` |  |
| `canSetPrivacyLevel` | `bool` |  |
| `canSetOwnMemberAttribute` | `bool` |  |
| `canSetOtherMemberAttribute` | `bool` |  |
| `canSetOwnMemberNote` | `bool` |  |
| `canSetOtherMemberNote` | `bool` |  |
| `canSetOwnVoiceState` | `bool` |  |
| `canSetOwnPresenceLevel` | `bool` |  |
| `canUseVoice` | `bool` |  |
| `canVoiceMuteMemberForAll` | `bool` |  |
| `canGetInvitation` | `bool` |  |
| `canSendInvitation` | `bool` |  |
| `canSendGuestInvitation` | `bool` |  |
| `canRevokeOwnInvitation` | `bool` |  |
| `canRevokeOtherInvitation` | `bool` |  |
| `canGetBan` | `bool` |  |
| `canGetSuggestion` | `bool` |  |
| `canSuggestMember` | `bool` |  |
| `canGetTicket` | `bool` |  |
| `canCreateTicket` | `bool` |  |
| `canDestroyTicket` | `bool` |  |
| `canAddBan` | `bool` |  |
| `canRemoveBan` | `bool` |  |
| `canCreateStream` | `bool` |  |
| `canDestroyStream` | `bool` |  |
| `canSetStreamPosition` | `bool` |  |
| `canSetStreamAttribute` | `bool` |  |
| `canSetStreamName` | `bool` |  |
| `canSetStreamSubject` | `bool` |  |
| `canSetStreamAccess` | `bool` |  |
| `canSetStreamVoiceLevel` | `bool` |  |
| `canCreateMessage` | `bool` |  |
| `canDestroyOwnMessage` | `bool` |  |
| `canDestroyOtherMessage` | `bool` |  |
| `canEditOwnMessage` | `bool` |  |
| `canPinMessage` | `bool` |  |
| `kickableRoleIds` | `number[]` | Roles that can be kicked and banned |

### ClubRoleInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `roleId` | `number` |  |
| `name` | `string` |  |
| `required` | `bool` | At least one user must be in this role |
| `unique` | `bool` | At most one user can be in this role |

### ClubSelfInvitationInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `invitationId` | `ClubInvitationId` |  |
| `club` | `ClubInfo` |  |
| `inviter` | `ClubMemberInfo` |  |
| `leaders` | `ClubMemberInfo[]` |  |

### ClubStreamInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `streamId` | `ClubStreamId` |  |
| `name` | `string` |  |
| `subject` | `string` |  |
| `leadersAndModeratorsOnly` | `bool` |  |
| `streamType` | `ClubStreamType` | `NeverSecret` |
| `creationTime` | `BigUInteger` |  |

### ClubStreamNotificationSetting

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `streamId` | `ClubStreamId` |  |
| `filter` | `ClubStreamNotificationFilter` |  |

### ClubTicketInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `ticketId` | `string` |  |
| `allowedRedeemCount` | `number` |  |
| `currentRedeemCount` | `number` |  |
| `creationTime` | `BigUInteger` | Creation time in microseconds since the UNIX epoch. |
| `expirationTime` | `BigUInteger` | Expiration time in microseconds since the UNIX epoch. |
| `defaultStreamId` | `ClubStreamId?` |  |
| `creator` | `ClubMemberInfo` |  |

## Predicates

Conditions referenced by the flags above.

- `RequiresClubsInitialized` *Precondition* (failure mode: ReturnNothing)
