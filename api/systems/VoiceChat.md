# VoiceChat

Namespace `C_VoiceChat` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/voicechatdocumentation.lua` (FileDataID 4637312)

## Functions

### ActivateChannel

```lua
C_VoiceChat.ActivateChannel(channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### ActivateChannelTranscription

```lua
C_VoiceChat.ActivateChannelTranscription(channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### BeginLocalCapture

```lua
C_VoiceChat.BeginLocalCapture(listenToLocalUser: bool)
```

`SecretArguments=AllowedWhenUntainted`

### CanAccessSettings

```lua
C_VoiceChat.CanAccessSettings() -> canAccess: bool
```

### CanPlayerUseVoiceChat

```lua
C_VoiceChat.CanPlayerUseVoiceChat() -> canUseVoiceChat: bool
```

### CreateChannel

```lua
C_VoiceChat.CreateChannel(channelDisplayName: cstring) -> status: VoiceChatStatusCode
```

`SecretArguments=AllowedWhenUntainted`

### DeactivateChannel

```lua
C_VoiceChat.DeactivateChannel(channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### DeactivateChannelTranscription

```lua
C_VoiceChat.DeactivateChannelTranscription(channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### EndLocalCapture

```lua
C_VoiceChat.EndLocalCapture()
```

### GetActiveChannelID

```lua
C_VoiceChat.GetActiveChannelID() -> channelID: VoiceChatID?
```

### GetActiveChannelType

```lua
C_VoiceChat.GetActiveChannelType() -> channelType: ChatChannelType?
```

### GetActiveVoiceProviderID

```lua
C_VoiceChat.GetActiveVoiceProviderID() -> activeVoiceProviderID: VoiceProviderID
```

### GetAvailableInputDevices

```lua
C_VoiceChat.GetAvailableInputDevices() -> inputDevices: VoiceAudioDevice[]?
```

### GetAvailableOutputDevices

```lua
C_VoiceChat.GetAvailableOutputDevices() -> outputDevices: VoiceAudioDevice[]?
```

### GetChannel

```lua
C_VoiceChat.GetChannel(channelID: VoiceChatID) -> channel: VoiceChatChannel
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetChannelForChannelType

```lua
C_VoiceChat.GetChannelForChannelType(channelType: ChatChannelType) -> channel: VoiceChatChannel
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetChannelForCommunityStream

```lua
C_VoiceChat.GetChannelForCommunityStream(clubId: ClubId, streamId: ClubStreamId) -> channel: VoiceChatChannel
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretInChatMessagingLockdown`

### GetCommunicationMode

```lua
C_VoiceChat.GetCommunicationMode() -> communicationMode: CommunicationMode?
```

### GetCurrentVoiceChatConnectionStatusCode

```lua
C_VoiceChat.GetCurrentVoiceChatConnectionStatusCode() -> statusCode: VoiceChatStatusCode?
```

### GetInputVolume

```lua
C_VoiceChat.GetInputVolume() -> volume: number?
```

### GetJoinClubVoiceChannelError

```lua
C_VoiceChat.GetJoinClubVoiceChannelError(clubId: ClubId) -> errorReason: VoiceChannelErrorReason?
```

`SecretArguments=AllowedWhenUntainted`

### GetLocalPlayerActiveChannelMemberInfo

```lua
C_VoiceChat.GetLocalPlayerActiveChannelMemberInfo() -> memberInfo: VoiceChatMember?
```

### GetLocalPlayerMemberID

```lua
C_VoiceChat.GetLocalPlayerMemberID(channelID: VoiceChatID) -> memberID: VoiceChatID?
```

`SecretArguments=AllowedWhenUntainted`

### GetMasterVolumeScale

```lua
C_VoiceChat.GetMasterVolumeScale() -> scale: number
```

### GetMemberGUID

```lua
C_VoiceChat.GetMemberGUID(memberID: VoiceChatID, channelID: VoiceChatID) -> memberGUID: WOWGUID
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetMemberID

```lua
C_VoiceChat.GetMemberID(channelID: VoiceChatID, memberGUID: WOWGUID) -> memberID: VoiceChatID?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetMemberInfo

```lua
C_VoiceChat.GetMemberInfo(memberID: VoiceChatID, channelID: VoiceChatID) -> memberInfo: VoiceChatMember?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetMemberName

```lua
C_VoiceChat.GetMemberName(memberID: VoiceChatID, channelID: VoiceChatID) -> memberName: string?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### GetMemberVolume

```lua
C_VoiceChat.GetMemberVolume(playerLocation: PlayerLocation) -> volume: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GetOutputVolume

```lua
C_VoiceChat.GetOutputVolume() -> volume: number?
```

### GetProcesses

```lua
C_VoiceChat.GetProcesses() -> processes: VoiceChatProcess[]
```

`MayReturnNothing`

### GetPTTButtonPressedState

```lua
C_VoiceChat.GetPTTButtonPressedState() -> isPressed: bool?
```

### GetPushToTalkBinding

```lua
C_VoiceChat.GetPushToTalkBinding() -> keys: string[]?
```

### GetRemoteTtsVoices

```lua
C_VoiceChat.GetRemoteTtsVoices() -> ttsVoices: VoiceTtsVoiceType[]
```

### GetTtsVoices

```lua
C_VoiceChat.GetTtsVoices() -> ttsVoices: VoiceTtsVoiceType[]
```

### GetVADSensitivity

```lua
C_VoiceChat.GetVADSensitivity() -> sensitivity: number?
```

### IsChannelJoinPending

```lua
C_VoiceChat.IsChannelJoinPending(channelType: ChatChannelType, clubId: ClubId?, streamId: ClubStreamId?) -> isPending: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsDeafened

```lua
C_VoiceChat.IsDeafened() -> isDeafened: bool?
```

### IsEnabled

```lua
C_VoiceChat.IsEnabled() -> isEnabled: bool
```

### IsLoggedIn

```lua
C_VoiceChat.IsLoggedIn() -> isLoggedIn: bool
```

### IsMemberLocalPlayer

```lua
C_VoiceChat.IsMemberLocalPlayer(memberID: VoiceChatID, channelID: VoiceChatID) -> isLocalPlayer: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsMemberMuted

```lua
C_VoiceChat.IsMemberMuted(playerLocation: PlayerLocation) -> mutedForMe: bool?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### IsMemberMutedForAll

```lua
C_VoiceChat.IsMemberMutedForAll(memberID: VoiceChatID, channelID: VoiceChatID) -> mutedForAll: bool?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### IsMemberSilenced

```lua
C_VoiceChat.IsMemberSilenced(memberID: VoiceChatID, channelID: VoiceChatID) -> silenced: bool?
```

`SecretArguments=AllowedWhenUntainted` `SecretInChatMessagingLockdown`

### IsMuted

```lua
C_VoiceChat.IsMuted() -> isMuted: bool?
```

### IsParentalDisabled

```lua
C_VoiceChat.IsParentalDisabled() -> isParentalDisabled: bool
```

### IsParentalMuted

```lua
C_VoiceChat.IsParentalMuted() -> isParentalMuted: bool
```

### IsPlayerUsingVoice

```lua
C_VoiceChat.IsPlayerUsingVoice(playerLocation: PlayerLocation) -> isUsingVoice: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### IsSilenced

```lua
C_VoiceChat.IsSilenced() -> isSilenced: bool?
```

### IsSpeakForMeActive

```lua
C_VoiceChat.IsSpeakForMeActive() -> isActive: bool
```

### IsSpeakForMeAllowed

```lua
C_VoiceChat.IsSpeakForMeAllowed() -> isAllowed: bool
```

### IsTranscribing

```lua
C_VoiceChat.IsTranscribing() -> isTranscribing: bool
```

### IsTranscriptionAllowed

```lua
C_VoiceChat.IsTranscriptionAllowed() -> isAllowed: bool
```

### IsVoiceChatConnected

```lua
C_VoiceChat.IsVoiceChatConnected() -> connected: bool
```

### LeaveChannel

```lua
C_VoiceChat.LeaveChannel(channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### Login

```lua
C_VoiceChat.Login(channelType: ChatChannelType?) -> status: VoiceChatStatusCode
```

`SecretArguments=AllowedWhenUntainted`

### Logout

```lua
C_VoiceChat.Logout() -> status: VoiceChatStatusCode
```

### MarkChannelsDiscovered

```lua
C_VoiceChat.MarkChannelsDiscovered()
```

Once the UI has enumerated all channels, use this to reset the channel discovery state, it will be updated again if appropriate

### RequestJoinAndActivateCommunityStreamChannel

```lua
C_VoiceChat.RequestJoinAndActivateCommunityStreamChannel(clubId: ClubId, streamId: ClubStreamId)
```

`SecretArguments=AllowedWhenUntainted`

### RequestJoinChannelByChannelType

```lua
C_VoiceChat.RequestJoinChannelByChannelType(channelType: ChatChannelType, autoActivate: bool?)
```

`SecretArguments=AllowedWhenUntainted`

### RestoreActiveVoiceProvider

```lua
C_VoiceChat.RestoreActiveVoiceProvider() -> changed: bool
```

Changes the active voice provider to the party voice provider, or to the preferred voice provider when the party has none.

### SetActiveVoiceProvider

```lua
C_VoiceChat.SetActiveVoiceProvider(voiceProviderID: VoiceProviderID) -> success: bool
```

Changes the active voice provider without changing the preferred voice provider.

`SecretArguments=AllowedWhenUntainted`

### SetCommunicationMode

```lua
C_VoiceChat.SetCommunicationMode(communicationMode: CommunicationMode)
```

`SecretArguments=AllowedWhenUntainted`

### SetDeafened

```lua
C_VoiceChat.SetDeafened(isDeafened: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetInputDevice

```lua
C_VoiceChat.SetInputDevice(deviceID: string)
```

`SecretArguments=AllowedWhenUntainted`

### SetInputVolume

```lua
C_VoiceChat.SetInputVolume(volume: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMasterVolumeScale

```lua
C_VoiceChat.SetMasterVolumeScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMemberMuted

```lua
C_VoiceChat.SetMemberMuted(playerLocation: PlayerLocation, muted: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |
| `muted` | `bool` |  |

### SetMemberVolume

```lua
C_VoiceChat.SetMemberVolume(playerLocation: PlayerLocation, volume: number)
```

Adjusts member volume across all channels

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |
| `volume` | `number` |  |

### SetMuted

```lua
C_VoiceChat.SetMuted(isMuted: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutputDevice

```lua
C_VoiceChat.SetOutputDevice(deviceID: string)
```

`SecretArguments=AllowedWhenUntainted`

### SetOutputVolume

```lua
C_VoiceChat.SetOutputVolume(volume: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetPortraitTexture

```lua
C_VoiceChat.SetPortraitTexture(textureObject: SimpleTexture, memberID: VoiceChatID, channelID: VoiceChatID)
```

`SecretArguments=AllowedWhenUntainted`

### SetPushToTalkBinding

```lua
C_VoiceChat.SetPushToTalkBinding(keys: string[])
```

`SecretArguments=AllowedWhenUntainted`

### SetVADSensitivity

```lua
C_VoiceChat.SetVADSensitivity(sensitivity: number)
```

`SecretArguments=AllowedWhenUntainted`

### ShouldDiscoverChannels

```lua
C_VoiceChat.ShouldDiscoverChannels() -> shouldDiscoverChannels: bool
```

Use this while loading to determine if the UI should attempt to rediscover the previously joined/active voice channels

### SpeakRemoteTextSample

```lua
C_VoiceChat.SpeakRemoteTextSample(text: string)
```

`SecretArguments=AllowedWhenUntainted`

### SpeakText

```lua
C_VoiceChat.SpeakText(voiceID: number, text: cstring, rate: number, volume: number, overlap: bool)
```

SpeakText also supports XML TTS tags on Windows including bookmarks - see SAPI XML TTS Tutorial in Microsoft's online documentation for more information.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `voiceID` | `number` | `NeverSecret` |
| `text` | `cstring` | `ConditionalSecret` |
| `rate` | `number` | `NeverSecret` |
| `volume` | `number` | `NeverSecret` |
| `overlap` | `bool` | default `false`; `NeverSecret` |

### StopSpeakingText

```lua
C_VoiceChat.StopSpeakingText()
```

### ToggleDeafened

```lua
C_VoiceChat.ToggleDeafened()
```

### ToggleMemberMuted

```lua
C_VoiceChat.ToggleMemberMuted(playerLocation: PlayerLocation)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### ToggleMuted

```lua
C_VoiceChat.ToggleMuted()
```

## Events

### VOICE_CHAT_ACTIVE_INPUT_DEVICE_UPDATED

```lua
VOICE_CHAT_ACTIVE_INPUT_DEVICE_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_ACTIVE_OUTPUT_DEVICE_UPDATED

```lua
VOICE_CHAT_ACTIVE_OUTPUT_DEVICE_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_ACTIVE_VOICE_PROVIDER_CHANGED

```lua
VOICE_CHAT_ACTIVE_VOICE_PROVIDER_CHANGED(voiceProviderID: VoiceProviderID)
```

`SynchronousEvent`

### VOICE_CHAT_AUDIO_CAPTURE_ENERGY

```lua
VOICE_CHAT_AUDIO_CAPTURE_ENERGY(isSpeaking: bool, energy: number)
```

`SynchronousEvent`

### VOICE_CHAT_AUDIO_CAPTURE_STARTED

```lua
VOICE_CHAT_AUDIO_CAPTURE_STARTED()
```

`SynchronousEvent`

### VOICE_CHAT_AUDIO_CAPTURE_STOPPED

```lua
VOICE_CHAT_AUDIO_CAPTURE_STOPPED()
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_ACTIVATED

```lua
VOICE_CHAT_CHANNEL_ACTIVATED(channelID: VoiceChatID)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_DEACTIVATED

```lua
VOICE_CHAT_CHANNEL_DEACTIVATED(channelID: VoiceChatID)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_DISPLAY_NAME_CHANGED

```lua
VOICE_CHAT_CHANNEL_DISPLAY_NAME_CHANGED(channelID: VoiceChatID, channelDisplayName: cstring)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_JOINED

```lua
VOICE_CHAT_CHANNEL_JOINED(status: VoiceChatStatusCode, channelID: VoiceChatID, channelType: ChatChannelType, clubId: ClubId?, streamId: ClubStreamId?)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_ACTIVE_STATE_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_ACTIVE_STATE_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, isActive: bool)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_ADDED

```lua
VOICE_CHAT_CHANNEL_MEMBER_ADDED(memberID: VoiceChatID, channelID: VoiceChatID)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_ENERGY_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_ENERGY_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, speakingEnergy: number)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_GUID_UPDATED

```lua
VOICE_CHAT_CHANNEL_MEMBER_GUID_UPDATED(memberID: VoiceChatID, channelID: VoiceChatID)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ALL_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ALL_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, isMutedForAll: bool)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ME_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ME_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, isMutedForMe: bool)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_REMOVED

```lua
VOICE_CHAT_CHANNEL_MEMBER_REMOVED(memberID: VoiceChatID, channelID: VoiceChatID)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_SILENCED_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_SILENCED_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, isSilenced: bool)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_SPEAKING_STATE_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_SPEAKING_STATE_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, isSpeaking: bool)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_STT_MESSAGE

```lua
VOICE_CHAT_CHANNEL_MEMBER_STT_MESSAGE(memberID: VoiceChatID, channelID: VoiceChatID, message: string, language: string)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MEMBER_VOLUME_CHANGED

```lua
VOICE_CHAT_CHANNEL_MEMBER_VOLUME_CHANGED(memberID: VoiceChatID, channelID: VoiceChatID, volume: number)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### VOICE_CHAT_CHANNEL_MUTE_STATE_CHANGED

```lua
VOICE_CHAT_CHANNEL_MUTE_STATE_CHANGED(channelID: VoiceChatID, isMuted: bool)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_PTT_CHANGED

```lua
VOICE_CHAT_CHANNEL_PTT_CHANGED(channelID: VoiceChatID, pushToTalkSetting: cstring)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_REMOVED

```lua
VOICE_CHAT_CHANNEL_REMOVED(channelID: VoiceChatID)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_TRANSCRIBING_CHANGED

```lua
VOICE_CHAT_CHANNEL_TRANSCRIBING_CHANGED(channelID: VoiceChatID, isTranscribing: bool)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_TRANSMIT_CHANGED

```lua
VOICE_CHAT_CHANNEL_TRANSMIT_CHANGED(channelID: VoiceChatID, isTransmitting: bool)
```

`SynchronousEvent`

### VOICE_CHAT_CHANNEL_VOLUME_CHANGED

```lua
VOICE_CHAT_CHANNEL_VOLUME_CHANGED(channelID: VoiceChatID, volume: number)
```

`SynchronousEvent`

### VOICE_CHAT_COMMUNICATION_MODE_CHANGED

```lua
VOICE_CHAT_COMMUNICATION_MODE_CHANGED(communicationMode: CommunicationMode)
```

`SynchronousEvent`

### VOICE_CHAT_CONNECTION_SUCCESS

```lua
VOICE_CHAT_CONNECTION_SUCCESS()
```

`SynchronousEvent`

### VOICE_CHAT_DEAFENED_CHANGED

```lua
VOICE_CHAT_DEAFENED_CHANGED(isDeafened: bool)
```

`SynchronousEvent`

### VOICE_CHAT_DISCORD_SETTINGS_UPDATED

```lua
VOICE_CHAT_DISCORD_SETTINGS_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_ERROR

```lua
VOICE_CHAT_ERROR(platformCode: number, statusCode: VoiceChatStatusCode)
```

`SynchronousEvent`

### VOICE_CHAT_INPUT_DEVICES_UPDATED

```lua
VOICE_CHAT_INPUT_DEVICES_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_LOGIN

```lua
VOICE_CHAT_LOGIN(status: VoiceChatStatusCode)
```

`SynchronousEvent`

### VOICE_CHAT_LOGOUT

```lua
VOICE_CHAT_LOGOUT(status: VoiceChatStatusCode)
```

`SynchronousEvent`

### VOICE_CHAT_MUTED_CHANGED

```lua
VOICE_CHAT_MUTED_CHANGED(isMuted: bool)
```

`SynchronousEvent`

### VOICE_CHAT_OUTPUT_DEVICES_UPDATED

```lua
VOICE_CHAT_OUTPUT_DEVICES_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_PENDING_CHANNEL_JOIN_STATE

```lua
VOICE_CHAT_PENDING_CHANNEL_JOIN_STATE(channelType: ChatChannelType, clubId: ClubId?, streamId: ClubStreamId?, pendingJoin: bool)
```

`SynchronousEvent`

### VOICE_CHAT_PTT_BUTTON_PRESSED_STATE_CHANGED

```lua
VOICE_CHAT_PTT_BUTTON_PRESSED_STATE_CHANGED(isPressed: bool)
```

`SynchronousEvent`

### VOICE_CHAT_SILENCED_CHANGED

```lua
VOICE_CHAT_SILENCED_CHANGED(isSilenced: bool)
```

`SynchronousEvent`

### VOICE_CHAT_SPEAK_FOR_ME_ACTIVE_STATUS_UPDATED

```lua
VOICE_CHAT_SPEAK_FOR_ME_ACTIVE_STATUS_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_SPEAK_FOR_ME_FEATURE_STATUS_UPDATED

```lua
VOICE_CHAT_SPEAK_FOR_ME_FEATURE_STATUS_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_TTS_PLAYBACK_BOOKMARK

```lua
VOICE_CHAT_TTS_PLAYBACK_BOOKMARK(utteranceID: number, bookmarkName: cstring)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `utteranceID` | `number` |  |
| `bookmarkName` | `cstring` | `ConditionalSecret` |

### VOICE_CHAT_TTS_PLAYBACK_FAILED

```lua
VOICE_CHAT_TTS_PLAYBACK_FAILED(utteranceID: number, status: VoiceTtsStatusCode)
```

`SynchronousEvent`

### VOICE_CHAT_TTS_PLAYBACK_FINISHED

```lua
VOICE_CHAT_TTS_PLAYBACK_FINISHED(utteranceID: number)
```

`SynchronousEvent`

### VOICE_CHAT_TTS_PLAYBACK_STARTED

```lua
VOICE_CHAT_TTS_PLAYBACK_STARTED(utteranceID: number)
```

`SynchronousEvent`

### VOICE_CHAT_TTS_SPEAK_TEXT_UPDATE

```lua
VOICE_CHAT_TTS_SPEAK_TEXT_UPDATE(status: VoiceTtsStatusCode, utteranceID: number)
```

`SynchronousEvent`

### VOICE_CHAT_TTS_VOICES_UPDATE

```lua
VOICE_CHAT_TTS_VOICES_UPDATE()
```

`SynchronousEvent`

### VOICE_CHAT_VAD_SETTINGS_UPDATED

```lua
VOICE_CHAT_VAD_SETTINGS_UPDATED()
```

`SynchronousEvent`

### VOICE_CHAT_VOICE_PROVIDER_CHANGED

```lua
VOICE_CHAT_VOICE_PROVIDER_CHANGED(voiceProviderID: VoiceProviderID)
```

`SynchronousEvent`

### VOICE_CHAT_VOICE_PROVIDERS_AVAILABLE_CHANGED

```lua
VOICE_CHAT_VOICE_PROVIDERS_AVAILABLE_CHANGED()
```

`SynchronousEvent`

## Types

### CommunicationMode

*Enumeration* · 2 values, 0..1

Access values as `Enum.CommunicationMode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `PushToTalk` | `CommunicationMode` | = 0 |
| `OpenMic` | `CommunicationMode` | = 1 |

### VoiceChannelErrorReason

*Enumeration* · 2 values, 0..1

Access values as `Enum.VoiceChannelErrorReason.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Unknown` | `VoiceChannelErrorReason` | = 0 |
| `IsBattleNetChannel` | `VoiceChannelErrorReason` | = 1 |

### VoiceChatStatusCode

*Enumeration* · 26 values, 0..25

Access values as `Enum.VoiceChatStatusCode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `VoiceChatStatusCode` | = 0 |
| `OperationPending` | `VoiceChatStatusCode` | = 1 |
| `TooManyRequests` | `VoiceChatStatusCode` | = 2 |
| `LoginProhibited` | `VoiceChatStatusCode` | = 3 |
| `ClientNotInitialized` | `VoiceChatStatusCode` | = 4 |
| `ClientNotLoggedIn` | `VoiceChatStatusCode` | = 5 |
| `ClientAlreadyLoggedIn` | `VoiceChatStatusCode` | = 6 |
| `ChannelNameTooShort` | `VoiceChatStatusCode` | = 7 |
| `ChannelNameTooLong` | `VoiceChatStatusCode` | = 8 |
| `ChannelAlreadyExists` | `VoiceChatStatusCode` | = 9 |
| `AlreadyInChannel` | `VoiceChatStatusCode` | = 10 |
| `TargetNotFound` | `VoiceChatStatusCode` | = 11 |
| `Failure` | `VoiceChatStatusCode` | = 12 |
| `ServiceLost` | `VoiceChatStatusCode` | = 13 |
| `UnableToLaunchProxy` | `VoiceChatStatusCode` | = 14 |
| `ProxyConnectionTimeOut` | `VoiceChatStatusCode` | = 15 |
| `ProxyConnectionUnableToConnect` | `VoiceChatStatusCode` | = 16 |
| `ProxyConnectionUnexpectedDisconnect` | `VoiceChatStatusCode` | = 17 |
| `Disabled` | `VoiceChatStatusCode` | = 18 |
| `UnsupportedChatChannelType` | `VoiceChatStatusCode` | = 19 |
| `InvalidCommunityStream` | `VoiceChatStatusCode` | = 20 |
| `PlayerSilenced` | `VoiceChatStatusCode` | = 21 |
| `PlayerVoiceChatParentalDisabled` | `VoiceChatStatusCode` | = 22 |
| `InvalidInputDevice` | `VoiceChatStatusCode` | = 23 |
| `InvalidOutputDevice` | `VoiceChatStatusCode` | = 24 |
| `PlayerVoiceChatAgeVerificationRestricted` | `VoiceChatStatusCode` | = 25 |

### VoiceProviderID

*Enumeration* · 2 values, 0..1

Access values as `Enum.VoiceProviderID.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Legacy` | `VoiceProviderID` | = 0 |
| `Discord` | `VoiceProviderID` | = 1 |

### VoiceTtsStatusCode

*Enumeration* · 14 values, 0..13

Access values as `Enum.VoiceTtsStatusCode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Success` | `VoiceTtsStatusCode` | = 0 |
| `InvalidEngineType` | `VoiceTtsStatusCode` | = 1 |
| `EngineAllocationFailed` | `VoiceTtsStatusCode` | = 2 |
| `NotSupported` | `VoiceTtsStatusCode` | = 3 |
| `MaxCharactersExceeded` | `VoiceTtsStatusCode` | = 4 |
| `UtteranceBelowMinimumDuration` | `VoiceTtsStatusCode` | = 5 |
| `InputTextEnqueued` | `VoiceTtsStatusCode` | = 6 |
| `SdkNotInitialized` | `VoiceTtsStatusCode` | = 7 |
| `DestinationQueueFull` | `VoiceTtsStatusCode` | = 8 |
| `EnqueueNotNecessary` | `VoiceTtsStatusCode` | = 9 |
| `UtteranceNotFound` | `VoiceTtsStatusCode` | = 10 |
| `ManagerNotFound` | `VoiceTtsStatusCode` | = 11 |
| `InvalidArgument` | `VoiceTtsStatusCode` | = 12 |
| `InternalError` | `VoiceTtsStatusCode` | = 13 |

### VoiceAudioDevice

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `deviceID` | `string` |  |
| `displayName` | `string` |  |
| `isActive` | `bool` |  |
| `isSystemDefault` | `bool` |  |
| `isCommsDefault` | `bool` |  |

### VoiceChatChannel

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `channelID` | `VoiceChatID` | `NeverSecret` |
| `channelType` | `ChatChannelType` | `NeverSecret` |
| `clubId` | `ClubId` | `NeverSecret` |
| `streamId` | `ClubStreamId` | `NeverSecret` |
| `volume` | `number` | `NeverSecret` |
| `isActive` | `bool` | `NeverSecret` |
| `isMuted` | `bool` | `NeverSecret` |
| `isTransmitting` | `bool` | `NeverSecret` |
| `isTranscribing` | `bool` | `NeverSecret` |
| `members` | `VoiceChatMember[]` |  |

### VoiceChatMember

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `energy` | `number` |  |
| `memberID` | `VoiceChatID` |  |
| `isActive` | `bool` |  |
| `isSpeaking` | `bool` |  |
| `isMutedForAll` | `bool` |  |
| `isSilenced` | `bool` |  |

### VoiceChatProcess

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `channels` | `VoiceChatChannel[]` |  |

### VoiceTtsVoiceType

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `voiceID` | `number` |  |
| `name` | `string` |  |
