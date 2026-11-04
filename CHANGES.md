# Addon API changes: wowf 1.60.1.70707 → wowf 1.60.1.70755

Compared with build WOW-70707patch1.60.1_Retail. Code written for the older build that uses a removed or changed symbol below needs updating. Search `signatures.txt` for replacements.

| | Added | Removed | Changed |
|---|---:|---:|---:|
| functions | 1 | 0 | 6 |
| enums | 0 | 0 | 1 |
| structures | 0 | 0 | 1 |
| FrameXML functions | 1 | 0 | 0 |
| mixins | 0 | 1 | 7 |

## C_ActionBar

Documentation table `ActionBar`.

- **added** `C_ActionBar.IsHighestSpellRank(spellID: SpellIdentifier) -> isHighestRank: bool`

## C_BattleNet

Documentation table `BattleNet`.

- **changed** `BNetGameAccountInfo`
  - before: `BNetGameAccountInfo { gameAccountID: number, clientProgram: string, isOnline: bool, isGameBusy: bool, isGameAFK: bool, isAppearOffline: bool, wowProjectID: number?, characterName: string?, realmName: string?, realmDisplayName: string?, realmID: number?, factionName: string?, raceName: string?, classID: number?, className: string?, classFilename: cstring?, areaName: string?, characterLevel: number?, richPresence: string?, playerGuid: WOWGUID?, canSummon: bool, hasFocus: bool, regionID: number, isInCurrentRegion: bool, timerunningSeasonID: number? }`
  - after: `BNetGameAccountInfo { gameAccountID: number, clientProgram: string, isOnline: bool, isGameBusy: bool, isGameAFK: bool, isAppearOffline: bool, wowProjectID: number?, characterName: string?, realmName: string?, realmDisplayName: string?, realmID: number?, factionName: string?, raceName: string?, classID: number?, className: string?, classFilename: cstring?, areaName: string?, characterLevel: number?, richPresence: string?, playerGuid: WOWGUID?, canSummon: bool, hasFocus: bool, regionID: number, isInCurrentRegion: bool, timerunningSeasonID: number?, subIcon: string? }`
  - field `subIcon: string?` added

## Expansion

- **changed** `Enum.SubscriptionInterstitialType`
  - before: `Enum.SubscriptionInterstitialType { Standard=0, LeftNpeArea=1, MaxLevel=2 }`
  - after: `Enum.SubscriptionInterstitialType { Standard=0, LeftNpeArea=1, MaxLevel=2, SubscriptionPeriod=3 }`
  - value `SubscriptionPeriod = 3` added

## C_PaperDollInfo

Documentation table `PaperDollInfo`.

- **changed** `C_PaperDollInfo.CancelTemporaryEnchantment`
  - description changed
- **changed** `C_PaperDollInfo.GetTemporaryEnchantmentInfo`
  - description changed

## C_Roleset

Documentation table `RolesetSystem`.

- **changed** `C_Roleset.ApplyRolesetFilters`
  - now `HasRestrictions`
  - description changed

## C_Texture

Documentation table `TextureUtils`.

- **changed** `C_Texture.GetTitleIconTexture`
  - before: `C_Texture.GetTitleIconTexture(titleID: string, version: TitleIconVersion, callback: GetTitleIconTextureCallback)`
  - after: `C_Texture.GetTitleIconTexture(titleID: string, version: TitleIconVersion, callback: GetTitleIconTextureCallback, subIcon: string?)`
  - argument `subIcon: string?` added
- **changed** `C_Texture.IsTitleIconTextureReady`
  - before: `C_Texture.IsTitleIconTextureReady(titleID: string, version: TitleIconVersion) -> ready: bool`
  - after: `C_Texture.IsTitleIconTextureReady(titleID: string, version: TitleIconVersion, subIcon: string?) -> ready: bool`
  - argument `subIcon: string?` added
- **changed** `C_Texture.SetTitleIconTexture`
  - before: `C_Texture.SetTitleIconTexture(texture: SimpleTexture, titleID: string, version: TitleIconVersion)`
  - after: `C_Texture.SetTitleIconTexture(texture: SimpleTexture, titleID: string, version: TitleIconVersion, subIcon: string?)`
  - argument `subIcon: string?` added

## FrameXML global functions

- **added** `SubscriptionInterstitial_ShowSubscriptionPeriod()`

## FrameXML mixins

- **changed** `ActionButtonUtil`
  - method `OverrideStatusForUnplacedSpell` added
- **changed** `MainMenuBarEndCapMixin`
  - method `DoesFitOnScreen` added
  - method `OnEvent` added
- **changed** `MenuMixin`
  - method `FinalizeGridLayout` added
- **changed** `NamePlateAuraItemMixin`
  - method `OnEnter` removed
  - method `OnLeave` removed
  - method `RefreshTooltip` removed
  - method `SetUnit` removed
  - method `UpdateTooltip` removed
- **changed** `SocialUIBattleNetMenuButtonMixin`
  - method `ShouldShowBroadcastMenuOption` removed
- **removed** `SubscriptionInterstitialCloseButtonMixin`
- **changed** `SubscriptionInterstitialFrameMixin`
  - method `CreateShadowOverlay` added
  - method `HideInterstitial` added
  - method `ShowInterstitial` added
- **changed** `SubscriptionInterstitialSubscribeButtonBaseMixin`
  - before: `SubscriptionInterstitialSubscribeButtonBaseMixin`
  - after: `SubscriptionInterstitialSubscribeButtonBaseMixin (from SmartNavigationClickTrackingMixin)`
  - method `ClearClickState` removed
  - method `OnClick` removed
  - method `OnShow` removed
  - method `WasClicked` removed
