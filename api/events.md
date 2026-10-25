# Events

Register with `frame:RegisterEvent("NAME")`; the payload arrives as the `...` of `OnEvent`.


## AccountStore

See [AccountStore](systems/AccountStore.md).

- `ACCOUNT_STORE_CURRENCY_AVAILABLE_UPDATED`: currencyID: number
- `ACCOUNT_STORE_FRONT_UPDATED`: storeFrontID: number
- `ACCOUNT_STORE_ITEM_INFO_UPDATED`: itemID: number
- `ACCOUNT_STORE_TRANSACTION_ERROR`: result: AccountStoreTransactionResult
- `STORE_FRONT_STATE_UPDATED`: storeFrontID: number

## AchievementInfo

See [AchievementInfo](systems/AchievementInfo.md).

- `ACHIEVEMENT_EARNED`: achievementID: number, alreadyEarned: bool?
- `ACHIEVEMENT_PLAYER_NAME`: achievementID: number
- `ACHIEVEMENT_SEARCH_UPDATED`
- `CRITERIA_COMPLETE`: criteriaID: number
- `CRITERIA_EARNED`: achievementID: number, description: cstring, achievementAlreadyEarnedOnAccount: bool
- `CRITERIA_UPDATE`
- `INSPECT_ACHIEVEMENT_READY`: guid: WOWGUID
- `RECEIVED_ACHIEVEMENT_LIST`
- `RECEIVED_ACHIEVEMENT_MEMBER_LIST`: achievementID: number
- `TRACKED_ACHIEVEMENT_LIST_CHANGED`: achievementID: number?, added: bool?
- `TRACKED_ACHIEVEMENT_UPDATE`: achievementID: number, criteriaID: number?, elapsed: time_t?, duration: number?

## ActionBar

See [ActionBar](systems/ActionBar.md).

- `ACTIONBAR_HIDEGRID`
- `ACTIONBAR_PAGE_CHANGED`
- `ACTIONBAR_SHOWGRID`
- `ACTIONBAR_SHOW_BOTTOMLEFT`
- `ACTIONBAR_SLOT_CHANGED`: slot: number
- `ACTIONBAR_UPDATE_COOLDOWN`
- `ACTIONBAR_UPDATE_STATE`
- `ACTIONBAR_UPDATE_USABLE`
- `ACTION_RANGE_CHECK_UPDATE`: slot: luaIndex, isInRange: bool, checksRange: bool
- `ACTION_USABLE_CHANGED`: changes: ActionUsableState[]
- `PET_BAR_UPDATE`
- `UPDATE_BONUS_ACTIONBAR`
- `UPDATE_EXTRA_ACTIONBAR`
- `UPDATE_MULTI_CAST_ACTIONBAR`
- `UPDATE_OVERRIDE_ACTIONBAR`

## AddOns

See [AddOns](systems/AddOns.md).

- `ADDONS_UNLOADING`: closingClient: bool
- `ADDON_LOADED`: addOnName: cstring, containsBindings: bool
- `SAVED_VARIABLES_TOO_LARGE`: addOnName: cstring

## AdventureJournal

See [AdventureJournal](systems/AdventureJournal.md).

- `AJ_DUNGEON_ACTION`: lfgDungeonID: number
- `AJ_OPEN`
- `AJ_OPEN_COLLECTIONS_ACTION`
- `AJ_PVE_LFG_ACTION`
- `AJ_PVP_ACTION`: battleMasterListID: number
- `AJ_PVP_LFG_ACTION`
- `AJ_PVP_RBG_ACTION`
- `AJ_PVP_SKIRMISH_ACTION`
- `AJ_PVP_SPECIAL_BG_ACTION`
- `AJ_PVP_TRAINING_GROUNDS_ACTION`
- `AJ_QUEST_LOG_OPEN`: questID: number, uiMapID: number
- `AJ_RAID_ACTION`: lfgDungeonID: number
- `AJ_REFRESH_DISPLAY`: newAdventureNotice: bool
- `AJ_REWARD_DATA_RECEIVED`

## AdventureMap

See [AdventureMap](systems/AdventureMap.md).

- `ADVENTURE_MAP_CLOSE`
- `ADVENTURE_MAP_OPEN`: followerTypeID: number
- `ADVENTURE_MAP_QUEST_UPDATE`: questID: number
- `ADVENTURE_MAP_UPDATE_INSETS`
- `ADVENTURE_MAP_UPDATE_POIS`

## AlliedRaces

See [AlliedRaces](systems/AlliedRaces.md).

- `ALLIED_RACE_CLOSE`
- `ALLIED_RACE_OPEN`: raceID: number

## AnimaDiversionInfo

See [AnimaDiversionInfo](systems/AnimaDiversionInfo.md).

- `ANIMA_DIVERSION_CLOSE`
- `ANIMA_DIVERSION_OPEN`: info: AnimaDiversionFrameInfo
- `ANIMA_DIVERSION_TALENT_UPDATED`

## AreaPoiInfo

See [AreaPoiInfo](systems/AreaPoiInfo.md).

- `AREA_POIS_UPDATED`

## ArtifactUI

See [ArtifactUI](systems/ArtifactUI.md).

- `ARTIFACT_CLOSE`
- `ARTIFACT_ENDGAME_REFUND`: numRefundedPowers: number, refundedTier: ArtifactTiers, bagOrSlotIndex: luaIndex, slotIndex: luaIndex?
- `ARTIFACT_RELIC_FORGE_CLOSE`
- `ARTIFACT_RELIC_FORGE_PREVIEW_RELIC_CHANGED`
- `ARTIFACT_RELIC_FORGE_UPDATE`
- `ARTIFACT_RELIC_INFO_RECEIVED`
- `ARTIFACT_RESPEC_PROMPT`
- `ARTIFACT_TIER_CHANGED`: newTier: luaIndex, bagOrSlotIndex: luaIndex, slotIndex: luaIndex?
- `ARTIFACT_UPDATE`: newItem: bool
- `ARTIFACT_XP_UPDATE`

## AssistedCombat

See [AssistedCombat](systems/AssistedCombat.md).

- `ASSISTED_COMBAT_ACTION_SPELL_CAST`

## AuctionHouse

See [AuctionHouse](systems/AuctionHouse.md).

- `AUCTION_CANCELED`: auctionID: number
- `AUCTION_HOUSE_AUCTIONS_EXPIRED`: auctionID: number
- `AUCTION_HOUSE_AUCTION_CREATED`: auctionID: number
- `AUCTION_HOUSE_BROWSE_FAILURE`
- `AUCTION_HOUSE_BROWSE_RESULTS_ADDED`: addedBrowseResults: BrowseResultInfo[]
- `AUCTION_HOUSE_BROWSE_RESULTS_UPDATED`
- `AUCTION_HOUSE_CLOSED`
- `AUCTION_HOUSE_DISABLED`
- `AUCTION_HOUSE_FAVORITES_UPDATED`
- `AUCTION_HOUSE_ITEM_DELIVERY_DELAY_UPDATE`: purchasedItemDeliveryDelay: number, cancelledItemDeliveryDelay: number
- `AUCTION_HOUSE_NEW_BID_RECEIVED`: auctionID: number
- `AUCTION_HOUSE_NEW_RESULTS_RECEIVED`: itemKey: ItemKey?
- `AUCTION_HOUSE_POST_ERROR`
- `AUCTION_HOUSE_POST_WARNING`
- `AUCTION_HOUSE_PURCHASE_COMPLETED`: auctionID: number
- `AUCTION_HOUSE_SCRIPT_DEPRECATED`
- `AUCTION_HOUSE_SHOW`
- `AUCTION_HOUSE_SHOW_COMMODITY_WON_NOTIFICATION`: commodityName: string, commodityQuantity: number
- `AUCTION_HOUSE_SHOW_ERROR`: error: AuctionHouseError
- `AUCTION_HOUSE_SHOW_FORMATTED_NOTIFICATION`: notification: AuctionHouseNotification, text: string, auctionID: number?
- `AUCTION_HOUSE_SHOW_NOTIFICATION`: notification: AuctionHouseNotification
- `AUCTION_HOUSE_THROTTLED_MESSAGE_DROPPED`
- `AUCTION_HOUSE_THROTTLED_MESSAGE_QUEUED`
- `AUCTION_HOUSE_THROTTLED_MESSAGE_RESPONSE_RECEIVED`
- `AUCTION_HOUSE_THROTTLED_MESSAGE_SENT`
- `AUCTION_HOUSE_THROTTLED_SYSTEM_READY`
- `AUCTION_MULTISELL_FAILURE`
- `AUCTION_MULTISELL_START`: numRepetitions: number
- `AUCTION_MULTISELL_UPDATE`: createdCount: number, totalToCreate: number
- `BIDS_UPDATED`
- `BID_ADDED`: bidID: number
- `COMMODITY_PRICE_UNAVAILABLE`
- `COMMODITY_PRICE_UPDATED`: updatedUnitPrice: BigUInteger, updatedTotalPrice: BigUInteger
- `COMMODITY_PURCHASED`: itemID: number, quantity: number
- `COMMODITY_PURCHASE_FAILED`
- `COMMODITY_PURCHASE_SUCCEEDED`
- `COMMODITY_SEARCH_RESULTS_ADDED`: itemID: number
- `COMMODITY_SEARCH_RESULTS_RECEIVED`
- `COMMODITY_SEARCH_RESULTS_UPDATED`: itemID: number
- `EXTRA_BROWSE_INFO_RECEIVED`: itemID: number
- `ITEM_KEY_ITEM_INFO_RECEIVED`: itemID: number
- `ITEM_PURCHASED`: itemID: number
- `ITEM_SEARCH_RESULTS_ADDED`: itemKey: ItemKey
- `ITEM_SEARCH_RESULTS_UPDATED`: itemKey: ItemKey, newAuctionID: number?
- `OWNED_AUCTIONS_UPDATED`
- `OWNED_AUCTION_BIDDER_INFO_RECEIVED`: auctionID: number, bidderName: cstring
- `REPLICATE_ITEM_LIST_UPDATE`

## AzeriteEmpoweredItem

See [AzeriteEmpoweredItem](systems/AzeriteEmpoweredItem.md).

- `AZERITE_EMPOWERED_ITEM_EQUIPPED_STATUS_CHANGED`: isHeartEquipped: bool
- `AZERITE_EMPOWERED_ITEM_SELECTION_UPDATED`: azeriteEmpoweredItemLocation: AzeriteEmpoweredItemLocation

## AzeriteEssence

See [AzeriteEssence](systems/AzeriteEssence.md).

- `AZERITE_ESSENCE_ACTIVATED`: slot: AzeriteEssenceSlot, essenceID: number
- `AZERITE_ESSENCE_ACTIVATION_FAILED`: slot: AzeriteEssenceSlot, essenceID: number
- `AZERITE_ESSENCE_CHANGED`: essenceID: number, newRank: number
- `AZERITE_ESSENCE_FORGE_CLOSE`
- `AZERITE_ESSENCE_FORGE_OPEN`
- `AZERITE_ESSENCE_MILESTONE_UNLOCKED`: milestoneID: number
- `AZERITE_ESSENCE_UPDATE`
- `PENDING_AZERITE_ESSENCE_CHANGED`: essenceID: number?

## AzeriteItem

See [AzeriteItem](systems/AzeriteItem.md).

- `AZERITE_ITEM_ENABLED_STATE_CHANGED`: enabled: bool
- `AZERITE_ITEM_EXPERIENCE_CHANGED`: azeriteItemLocation: AzeriteItemLocation, oldExperienceAmount: number, newExperienceAmount: number
- `AZERITE_ITEM_POWER_LEVEL_CHANGED`: azeriteItemLocation: AzeriteItemLocation, oldPowerLevel: number, newPowerLevel: number, unlockedEmpoweredItemsInfo: UnlockedAzeriteEmpoweredItems[], azeriteItemID: number

## Bank

See [Bank](systems/Bank.md).

- `BANKFRAME_CLOSED`
- `BANKFRAME_OPENED`
- `BANK_BAG_SLOT_FLAGS_UPDATED`: slot: number
- `BANK_TABS_CHANGED`: bankType: BankType
- `BANK_TAB_SETTINGS_UPDATED`: bankType: BankType
- `PLAYERBANKSLOTS_CHANGED`: slot: number
- `PLAYER_ACCOUNT_BANK_TAB_SLOTS_CHANGED`: slot: number

## BarberShop

See [BarberShop](systems/BarberShop.md).

- `BARBER_SHOP_APPEARANCE_APPLIED`
- `BARBER_SHOP_CAMERA_VALUES_UPDATED`
- `BARBER_SHOP_CLOSE`
- `BARBER_SHOP_COST_UPDATE`
- `BARBER_SHOP_FORCE_CUSTOMIZATIONS_UPDATE`
- `BARBER_SHOP_OPEN`
- `BARBER_SHOP_RESULT`: success: bool

## BattlePet

See [BattlePet](systems/BattlePet.md).

- `PET_BATTLE_ABILITY_CHANGED`: owner: number, petIndex: number, abilityID: number
- `PET_BATTLE_ACTION_SELECTED`
- `PET_BATTLE_AURA_APPLIED`: owner: number, petIndex: number, auraInstanceID: number
- `PET_BATTLE_AURA_CANCELED`: owner: number, petIndex: number, auraInstanceID: number
- `PET_BATTLE_AURA_CHANGED`: owner: number, petIndex: number, auraInstanceID: number
- `PET_BATTLE_CAPTURED`: owner: number, petIndex: number
- `PET_BATTLE_CLOSE`
- `PET_BATTLE_FINAL_ROUND`: owner: number
- `PET_BATTLE_HEALTH_CHANGED`: owner: number, petIndex: number, healthChange: number
- `PET_BATTLE_LEVEL_CHANGED`: owner: number, petIndex: number, newLevel: number
- `PET_BATTLE_MAX_HEALTH_CHANGED`: owner: number, petIndex: number, healthChange: number
- `PET_BATTLE_OPENING_DONE`
- `PET_BATTLE_OPENING_START`
- `PET_BATTLE_OVER`
- `PET_BATTLE_OVERRIDE_ABILITY`: abilityIndex: number
- `PET_BATTLE_PET_CHANGED`: owner: number
- `PET_BATTLE_PET_ROUND_PLAYBACK_COMPLETE`: roundNumber: number
- `PET_BATTLE_PET_ROUND_RESULTS`: roundNumber: number
- `PET_BATTLE_PET_TYPE_CHANGED`: owner: number, petIndex: number, stateValue: number
- `PET_BATTLE_PVP_DUEL_REQUESTED`: fullName: cstring
- `PET_BATTLE_PVP_DUEL_REQUEST_CANCEL`
- `PET_BATTLE_QUEUE_PROPOSAL_ACCEPTED`
- `PET_BATTLE_QUEUE_PROPOSAL_DECLINED`
- `PET_BATTLE_QUEUE_PROPOSE_MATCH`
- `PET_BATTLE_QUEUE_STATUS`
- `PET_BATTLE_XP_CHANGED`: owner: number, petIndex: number, xpChange: number

## BehavioralMessaging

See [BehavioralMessaging](systems/BehavioralMessaging.md).

- `BEHAVIORAL_NOTIFICATION`: notificationType: string, dbId: NotificationDbId

## BlackMarketInfo

See [BlackMarketInfo](systems/BlackMarketInfo.md).

- `BLACK_MARKET_BID_RESULT`: marketID: number, resultCode: number
- `BLACK_MARKET_CLOSE`
- `BLACK_MARKET_ITEM_UPDATE`
- `BLACK_MARKET_OPEN`
- `BLACK_MARKET_OUTBID`: marketID: number, itemID: number
- `BLACK_MARKET_UNAVAILABLE`
- `BLACK_MARKET_WON`: marketID: number, itemID: number

## BlizzCon2026Scripts

See [BlizzCon2026Scripts](systems/BlizzCon2026Scripts.md).

- `BC_26_COLD_SWAP_FEATURE_ENABLED_CHANGED`: newEnabled: bool, oldEnabled: bool
- `BC_26_EXPERIENCE_CHANGED`: newExperience: Bc26Experience, oldExperience: Bc26Experience

## Browser

See [Browser](systems/Browser.md).

- `FULLSCREEN_BROWSER_SPINNER_HIDE`
- `FULLSCREEN_BROWSER_SPINNER_SHOW`
- `SIMPLE_BROWSER_POPUP`: url: string
- `SIMPLE_BROWSER_SOCIAL_CALLBACK_INVOKED`: url: string
- `SIMPLE_BROWSER_WEB_ERROR`: errorCode: number
- `SIMPLE_BROWSER_WEB_PROXY_FAILED`
- `SIMPLE_CHECKOUT_CLOSED`

## Calendar

See [Calendar](systems/Calendar.md).

- `CALENDAR_ACTION_PENDING`: pending: bool
- `CALENDAR_CLOSE_EVENT`
- `CALENDAR_EVENT_ALARM`: title: cstring, hour: number, minute: number
- `CALENDAR_NEW_EVENT`: isCopy: bool
- `CALENDAR_OPEN_EVENT`: calendarType: cstring
- `CALENDAR_UPDATE_ERROR`: errorReason: cstring
- `CALENDAR_UPDATE_ERROR_WITH_COUNT`: errorReason: cstring, count: number
- `CALENDAR_UPDATE_ERROR_WITH_PLAYER_NAME`: errorReason: cstring, playerName: cstring
- `CALENDAR_UPDATE_EVENT`
- `CALENDAR_UPDATE_EVENT_LIST`
- `CALENDAR_UPDATE_GUILD_EVENTS`
- `CALENDAR_UPDATE_INVITE_LIST`: hasCompleteList: bool?
- `CALENDAR_UPDATE_PENDING_INVITES`

## CatalogShop

See [CatalogShop](systems/CatalogShop.md).

- `BULK_PURCHASE_RESULT_RECEIVED`: result: BulkPurchaseResult, productResults: BulkPurchaseIndividualProductResult[], bestTopUpProductID: number?, totalCost: number?
- `BULK_REFUND_RESULT_RECEIVED`: result: BulkRefundResult
- `CATALOG_SHOP_ADD_PENDING_PRODUCT`: productID: number
- `CATALOG_SHOP_DATA_REFRESH`: shoppingSessionUUIDStr: string?
- `CATALOG_SHOP_DISABLED`
- `CATALOG_SHOP_FETCH_FAILURE`: shoppingSessionUUIDStr: string?
- `CATALOG_SHOP_FETCH_SUCCESS`: shoppingSessionUUIDStr: string?
- `CATALOG_SHOP_OPEN_SIMPLE_CHECKOUT`: checkoutID: number
- `CATALOG_SHOP_PURCHASE_SUCCESS`: productID: number
- `CATALOG_SHOP_REBUILD_SCROLL_BOX`
- `CATALOG_SHOP_REFUNDABLE_DECORS_UPDATED`
- `CATALOG_SHOP_REMOVE_PENDING_PRODUCT`: productID: number
- `CATALOG_SHOP_RESULT_ERROR`
- `CATALOG_SHOP_SPECIFIC_PRODUCT_REFRESH`: productID: number
- `CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE`: currencyCode: string, balance: string
- `CATALOG_SHOP_VIRTUAL_CURRENCY_BALANCE_UPDATE_FAILURE`: currencyCode: string
- `SET_SEEN_PRODUCTS`: productIds: number[]
- `SHOW_NEW_PRODUCT_NOTIFICATION`

## ChallengeModeInfo

See [ChallengeModeInfo](systems/ChallengeModeInfo.md).

- `CHALLENGE_MODE_COMPLETED`
- `CHALLENGE_MODE_COMPLETED_REWARDS`: mapID: number, medal: number, timeMS: number, money: number, rewards: ChallengeModeReward[]
- `CHALLENGE_MODE_DEATH_COUNT_UPDATED`
- `CHALLENGE_MODE_KEYSTONE_RECEPTABLE_OPEN`
- `CHALLENGE_MODE_KEYSTONE_SLOTTED`: keystoneID: number
- `CHALLENGE_MODE_LEADERBOARD_RESULT`: mapID: number, challengeModeID: number, page: number, results: MythicPlusLeaderboardResult[]
- `CHALLENGE_MODE_LEADERS_UPDATE`
- `CHALLENGE_MODE_LEAVER_TIMER_ENDED`
- `CHALLENGE_MODE_LEAVER_TIMER_STARTED`
- `CHALLENGE_MODE_MAPS_UPDATE`
- `CHALLENGE_MODE_MEMBER_INFO_UPDATED`
- `CHALLENGE_MODE_NEW_RECORD`: mapID: number, timeMS: number, medal: number
- `CHALLENGE_MODE_RESET`: mapID: number
- `CHALLENGE_MODE_START`: mapID: number

## ChatInfo

See [ChatInfo](systems/ChatInfo.md).

- `ALTERNATIVE_DEFAULT_LANGUAGE_CHANGED`
- `BN_CHAT_MSG_ADDON`: prefix: cstring, text: cstring, channel: cstring, senderID: number
- `CAN_LOCAL_WHISPER_TARGET_RESPONSE`: whisperTarget: WOWGUID, status: ChatWhisperTargetStatus
- `CAN_PLAYER_SPEAK_LANGUAGE_CHANGED`: languageId: number, canSpeakLanguage: bool
- `CAUTIONARY_CHANNEL_MESSAGE`: confirmNumber: number
- `CAUTIONARY_CHAT_MESSAGE`: chatLineID: number, confirmNumber: number
- `CHANNEL_COUNT_UPDATE`: displayIndex: number, count: number
- `CHANNEL_FLAGS_UPDATED`: displayIndex: number
- `CHANNEL_INVITE_REQUEST`: channelID: cstring, name: cstring
- `CHANNEL_LEFT`: chatChannelID: number, name: cstring
- `CHANNEL_PASSWORD_REQUEST`: channelID: cstring
- `CHANNEL_ROSTER_UPDATE`: displayIndex: number, count: number
- `CHANNEL_UI_UPDATE`
- `CHAT_COMBAT_MSG_ARENA_POINTS_GAIN`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_LOGGING_CHANGED`: whichLog: number, isEnabled: bool
- `CHAT_MSG_ACHIEVEMENT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_ADDON`: prefix: cstring, text: cstring, channel: cstring, sender: cstring, target: cstring, zoneChannelID: number, localID: number, name: cstring, instanceID: number
- `CHAT_MSG_ADDON_LOGGED`: prefix: cstring, text: cstring, channel: cstring, sender: cstring, target: cstring, zoneChannelID: number, localID: number, name: cstring, instanceID: number
- `CHAT_MSG_AFK`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BG_SYSTEM_ALLIANCE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BG_SYSTEM_HORDE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BG_SYSTEM_NEUTRAL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_INLINE_TOAST_ALERT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_INLINE_TOAST_BROADCAST`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_INLINE_TOAST_BROADCAST_INFORM`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_INLINE_TOAST_CONVERSATION`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_WHISPER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_WHISPER_INFORM`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_BN_WHISPER_PLAYER_OFFLINE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL_JOIN`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL_LEAVE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL_LEAVE_PREVENTED`: channelName: cstring
- `CHAT_MSG_CHANNEL_LIST`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL_NOTICE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CHANNEL_NOTICE_USER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COLLECTED_APPEARANCE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COMBAT_FACTION_CHANGE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COMBAT_HONOR_GAIN`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COMBAT_MISC_INFO`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COMBAT_XP_GAIN`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_COMMUNITIES_CHANNEL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_CURRENCY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_DND`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_EMOTE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_FILTERED`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_GUILD`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_GUILD_ACHIEVEMENT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_GUILD_DISCORD`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_GUILD_ITEM_LOOTED`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_IGNORED`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_INSTANCE_CHAT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_INSTANCE_CHAT_LEADER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_LOOT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONEY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONSTER_EMOTE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONSTER_PARTY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONSTER_SAY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONSTER_WHISPER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_MONSTER_YELL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_OFFICER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_OPENING`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PARTY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PARTY_LEADER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PET_BATTLE_COMBAT_LOG`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PET_BATTLE_INFO`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PET_INFO`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_PING`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RAID`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RAID_BOSS_EMOTE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RAID_BOSS_WHISPER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RAID_LEADER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RAID_WARNING`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_RESTRICTED`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_SAY`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_SKILL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_SYSTEM`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_TARGETICONS`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_TEXT_EMOTE`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_TRADESKILLS`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_VOICE_TEXT`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_WHISPER`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_WHISPER_INFORM`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_MSG_YELL`: text: cstring, playerName: cstring, languageName: cstring, channelName: cstring, playerName2: cstring, specialFlags: cstring, zoneChannelID: number, channelIndex: number, channelBaseName: cstring, languageID: number, lineID: number, guid: WOWGUID, bnSenderID: number, isMobile: bool, isSubtitle: bool, hideSenderInLetterbox: bool, suppressRaidIcons: bool, discordInfo: DiscordChatInfo
- `CHAT_REGIONAL_SEND_FAILED`
- `CHAT_REGIONAL_STATUS_CHANGED`: isServiceAvailable: bool
- `CHAT_SERVER_DISCONNECTED`: isInitialMessage: bool?
- `CHAT_SERVER_RECONNECTED`
- `CLEAR_BOSS_EMOTES`
- `DAILY_RESET_INSTANCE_WELCOME`: mapname: cstring, timeLeft: number
- `INSTANCE_RESET_WARNING`: warningMessage: cstring, timeLeft: number
- `LANGUAGE_LIST_CHANGED`
- `NOTIFY_CHAT_SUPPRESSED`
- `QUEST_BOSS_EMOTE`: text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool
- `RAID_BOSS_EMOTE`: text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool
- `RAID_BOSS_WHISPER`: text: cstring, playerName: cstring, displayTime: number, enableBossEmoteWarningSound: bool
- `RAID_INSTANCE_WELCOME`: mapname: cstring, timeLeft: number, locked: number, extended: number
- `UPDATE_CHAT_COLOR`: name: cstring, r: number, g: number, b: number
- `UPDATE_CHAT_COLOR_NAME_BY_CLASS`: name: cstring, colorNameByClass: bool
- `UPDATE_CHAT_WINDOWS`
- `UPDATE_FLOATING_CHAT_WINDOWS`

## Cinematic

See [Cinematic](systems/Cinematic.md).

- `CINEMATIC_START`: canBeCancelled: bool, forcedAspectRatio: CameraModeAspectRatio
- `CINEMATIC_STOP`
- `HIDE_SUBTITLE`
- `PLAY_MOVIE`: movieID: number
- `SHOW_SUBTITLE`: subtitle: cstring, sender: cstring?
- `STOP_MOVIE`

## ClassTalents

See [ClassTalents](systems/ClassTalents.md).

- `ACTIVE_COMBAT_CONFIG_CHANGED`: configID: number
- `CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_INDEX`: loadoutIndex: number
- `CLASS_TALENTS_SWITCH_TO_LOADOUT_BY_NAME`: loadoutName: cstring
- `CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_INDEX`: specIndex: number
- `CLASS_TALENTS_SWITCH_TO_SPECIALIZATION_BY_NAME`: specName: cstring
- `SELECTED_LOADOUT_CHANGED`
- `SPECIALIZATION_CHANGE_CAST_FAILED`
- `STARTER_BUILD_ACTIVATION_FAILED`

## ClassTrial

See [ClassTrial](systems/ClassTrial.md).

- `CLASS_TRIAL_TIMER_START`
- `CLASS_TRIAL_UPGRADE_COMPLETE`

## ClickBindings

See [ClickBindings](systems/ClickBindings.md).

- `CLICKBINDINGS_SET_HIGHLIGHTS_SHOWN`: showHighlights: bool

## ClientScene

See [ClientScene](systems/ClientScene.md).

- `CLIENT_SCENE_CLOSED`
- `CLIENT_SCENE_OPENED`: sceneType: ClientSceneType

## Club

See [Club](systems/Club.md).

- `AVATAR_LIST_UPDATED`: clubType: ClubType
- `CLUB_ADDED`: clubId: ClubId
- `CLUB_ERROR`: action: ClubActionType, error: ClubErrorType, clubType: ClubType
- `CLUB_INVITATIONS_RECEIVED_FOR_CLUB`: clubId: ClubId
- `CLUB_INVITATION_ADDED_FOR_SELF`: invitation: ClubSelfInvitationInfo
- `CLUB_INVITATION_REMOVED_FOR_SELF`: invitationId: ClubInvitationId
- `CLUB_MEMBERS_UPDATED`: clubId: ClubId
- `CLUB_MEMBER_ADDED`: clubId: ClubId, memberId: ClubMemberOpaqueId
- `CLUB_MEMBER_PRESENCE_UPDATED`: clubId: ClubId, memberId: ClubMemberOpaqueId, presence: ClubMemberPresence
- `CLUB_MEMBER_REMOVED`: clubId: ClubId, memberId: ClubMemberOpaqueId
- `CLUB_MEMBER_ROLE_UPDATED`: clubId: ClubId, memberId: ClubMemberOpaqueId, roleId: number
- `CLUB_MEMBER_UPDATED`: clubId: ClubId, memberId: ClubMemberOpaqueId
- `CLUB_MESSAGE_ADDED`: clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier
- `CLUB_MESSAGE_HISTORY_RECEIVED`: clubId: ClubId, streamId: ClubStreamId, downloadedRange: ClubMessageRange, contiguousRange: ClubMessageRange
- `CLUB_MESSAGE_UPDATED`: clubId: ClubId, streamId: ClubStreamId, messageId: ClubMessageIdentifier
- `CLUB_REMOVED`: clubId: ClubId
- `CLUB_REMOVED_MESSAGE`: clubName: string, clubRemovedReason: ClubRemovedReason
- `CLUB_SELF_MEMBER_ROLE_UPDATED`: clubId: ClubId, roleId: number
- `CLUB_STREAMS_LOADED`: clubId: ClubId
- `CLUB_STREAM_ADDED`: clubId: ClubId, streamId: ClubStreamId
- `CLUB_STREAM_REMOVED`: clubId: ClubId, streamId: ClubStreamId
- `CLUB_STREAM_SUBSCRIBED`: clubId: ClubId, streamId: ClubStreamId
- `CLUB_STREAM_UNSUBSCRIBED`: clubId: ClubId, streamId: ClubStreamId
- `CLUB_STREAM_UPDATED`: clubId: ClubId, streamId: ClubStreamId
- `CLUB_TICKETS_RECEIVED`: clubId: ClubId
- `CLUB_TICKET_CREATED`: clubId: ClubId, ticketInfo: ClubTicketInfo
- `CLUB_TICKET_RECEIVED`: ticket: string
- `CLUB_UPDATED`: clubId: ClubId
- `INITIAL_CLUBS_LOADED`
- `STREAM_VIEW_MARKER_UPDATED`: clubId: ClubId, streamId: ClubStreamId, lastReadTime: BigUInteger?

## ClubFinderInfo

See [ClubFinderInfo](systems/ClubFinderInfo.md).

- `CLUB_FINDER_APPLICANT_INVITE_RECIEVED`: clubFinderGUIDs: WOWGUID[]
- `CLUB_FINDER_APPLICATIONS_UPDATED`: type: ClubFinderRequestType, clubFinderGUIDs: WOWGUID[]
- `CLUB_FINDER_CAN_WHISPER_APPLICANT`: applicant: WOWGUID
- `CLUB_FINDER_CLUB_LIST_RETURNED`: type: ClubFinderRequestType
- `CLUB_FINDER_CLUB_REPORTED`: type: ClubFinderRequestType, clubFinderGUID: WOWGUID
- `CLUB_FINDER_COMMUNITY_OFFLINE_JOIN`: clubId: ClubId
- `CLUB_FINDER_ENABLED_OR_DISABLED`
- `CLUB_FINDER_GUILD_REALM_NAME_UPDATED`: clubFinderGUID: WOWGUID, realmName: string
- `CLUB_FINDER_LINKED_CLUB_RETURNED`: clubInfo: RecruitingClubInfo
- `CLUB_FINDER_MEMBERSHIP_LIST_CHANGED`
- `CLUB_FINDER_PLAYER_PENDING_LIST_RECIEVED`: type: ClubFinderRequestType
- `CLUB_FINDER_POST_UPDATED`: clubFinderGUIDs: WOWGUID[]
- `CLUB_FINDER_RECRUITMENT_POST_RETURNED`: type: ClubFinderRequestType
- `CLUB_FINDER_RECRUITS_UPDATED`: type: ClubFinderRequestType
- `CLUB_FINDER_RECRUIT_LIST_CHANGED`

## ColorOverrides

See [ColorOverrides](systems/ColorOverrides.md).

- `COLOR_OVERRIDES_RESET`
- `COLOR_OVERRIDE_UPDATED`: overrideType: ColorOverride

## CombatLog

See [CombatLog](systems/CombatLog.md).

- `COMBAT_LOG_ENTRIES_CLEARED`
- `COMBAT_LOG_EVENT`
- `COMBAT_LOG_EVENT_UNFILTERED`
- `COMBAT_LOG_MESSAGE_LIMIT_CHANGED`: messageLimit: number

## CombatLogInternal

See [CombatLogInternal](systems/CombatLogInternal.md).

- `COMBAT_LOG_EVENT_INTERNAL_UNFILTERED`

## CombatLogSecure

See [CombatLogSecure](systems/CombatLogSecure.md).

- `COMBAT_LOG_APPLY_FILTER_SETTINGS`: filterSettings: LuaValueVariant
- `COMBAT_LOG_MESSAGE`: message: string, colorR: number, colorG: number, colorB: number, order: CombatLogMessageOrder
- `COMBAT_LOG_REFILTER_ENTRIES`

## CombatText

See [CombatText](systems/CombatText.md).

- `COMBAT_TEXT_UPDATE`: combatTextType: cstring

## CommentatorFrame

See [CommentatorFrame](systems/CommentatorFrame.md).

- `COMMENTATOR_COMBAT_EVENT`
- `COMMENTATOR_ENTER_WORLD`
- `COMMENTATOR_HISTORY_FLUSHED`
- `COMMENTATOR_IMMEDIATE_FOV_UPDATE`: fov: number
- `COMMENTATOR_MAP_UPDATE`
- `COMMENTATOR_PLAYER_NAME_OVERRIDE_UPDATE`: nameToOverride: cstring, overrideName: cstring?
- `COMMENTATOR_PLAYER_UPDATE`
- `COMMENTATOR_RESET_SETTINGS`
- `COMMENTATOR_TEAMS_SWAPPED`: swapped: bool
- `COMMENTATOR_TEAM_NAME_UPDATE`: teamName: string

## CompactUnitFrames

See [CompactUnitFrames](systems/CompactUnitFrames.md).

- `COMPACT_UNIT_FRAME_PROFILES_LOADED`

## Console

See [Console](systems/Console.md).

- `CONSOLE_CLEAR`
- `CONSOLE_COLORS_CHANGED`
- `CONSOLE_FONT_SIZE_CHANGED`
- `CONSOLE_LOG`: message: cstring
- `CONSOLE_MESSAGE`: message: cstring, colorType: number
- `CVAR_UPDATE`: eventName: cstring, value: cstring
- `TOGGLE_CONSOLE`: showConsole: bool?

## Container

See [Container](systems/Container.md).

- `BAG_CLOSED`: bagID: BagIndex
- `BAG_CONTAINER_UPDATE`
- `BAG_NEW_ITEMS_UPDATED`
- `BAG_OPEN`: bagID: number
- `BAG_OVERFLOW_WITH_FULL_INVENTORY`
- `BAG_SLOT_FLAGS_UPDATED`: slot: number
- `BAG_UPDATE`: bagID: BagIndex
- `BAG_UPDATE_COOLDOWN`
- `BAG_UPDATE_DELAYED`
- `EQUIP_BIND_REFUNDABLE_CONFIRM`: slot: number, itemLocation: ItemLocation
- `EQUIP_BIND_TRADEABLE_CONFIRM`: slot: number, itemLocation: ItemLocation
- `EXPAND_BAG_BAR_CHANGED`: expandBagBar: bool
- `INVENTORY_SEARCH_UPDATE`
- `ITEM_LOCKED`: bagOrSlotIndex: BagIndex, slotIndex: luaIndex?
- `ITEM_LOCK_CHANGED`: bagOrSlotIndex: BagIndex, slotIndex: luaIndex?
- `ITEM_UNLOCKED`: bagOrSlotIndex: BagIndex, slotIndex: luaIndex?
- `USE_COMBINED_BAGS_CHANGED`: useCombinedBags: bool

## ContentTracking

See [ContentTracking](systems/ContentTracking.md).

- `CONTENT_TRACKING_IS_ENABLED_UPDATE`: isEnabled: bool
- `CONTENT_TRACKING_LIST_UPDATE`
- `CONTENT_TRACKING_UPDATE`: type: ContentTrackingType, id: number, isTracked: bool
- `TRACKABLE_INFO_UPDATE`: type: ContentTrackingType, id: number
- `TRACKING_TARGET_INFO_UPDATE`: targetType: ContentTrackingTargetType, targetID: number

## ContributionCollector

See [ContributionCollector](systems/ContributionCollector.md).

- `CONTRIBUTION_CHANGED`: state: ContributionState, result: ContributionResult, name: string, contributionID: number
- `CONTRIBUTION_COLLECTOR_PENDING`: contributionID: number, isPending: bool, result: number
- `CONTRIBUTION_COLLECTOR_UPDATE`
- `CONTRIBUTION_COLLECTOR_UPDATE_SINGLE`: contributionID: number

## CooldownViewer

See [CooldownViewer](systems/CooldownViewer.md).

- `COOLDOWN_VIEWER_DATA_LOADED`
- `COOLDOWN_VIEWER_SPELL_OVERRIDE_UPDATED`: baseSpellID: number, overrideSpellID: number?
- `COOLDOWN_VIEWER_TABLE_HOTFIXED`

## Covenant

See [Covenant](systems/Covenant.md).

- `COVENANT_CHOSEN`: covenantID: number

## CovenantCallings

See [CovenantCallings](systems/CovenantCallings.md).

- `COVENANT_CALLINGS_UPDATED`: callings: BountyInfo[]

## CovenantPreview

See [CovenantPreview](systems/CovenantPreview.md).

- `COVENANT_PREVIEW_CLOSE`
- `COVENANT_PREVIEW_OPEN`: previewInfo: CovenantPreviewInfo

## CovenantSanctumUI

See [CovenantSanctumUI](systems/CovenantSanctumUI.md).

- `COVENANT_RENOWN_CATCH_UP_STATE_UPDATE`
- `COVENANT_SANCTUM_RENOWN_LEVEL_CHANGED`: newRenownLevel: number, oldRenownLevel: number

## CraftingOrderUI

See [CraftingOrderUI](systems/CraftingOrderUI.md).

- `CRAFTINGORDERS_CAN_REQUEST`
- `CRAFTINGORDERS_CLAIMED_ORDER_ADDED`
- `CRAFTINGORDERS_CLAIMED_ORDER_REMOVED`
- `CRAFTINGORDERS_CLAIMED_ORDER_UPDATED`: orderID: BigUInteger
- `CRAFTINGORDERS_CLAIM_ORDER_RESPONSE`: result: CraftingOrderResult, orderID: BigUInteger
- `CRAFTINGORDERS_CRAFT_ORDER_RESPONSE`: result: CraftingOrderResult, orderID: BigUInteger
- `CRAFTINGORDERS_CUSTOMER_FAVORITES_CHANGED`
- `CRAFTINGORDERS_CUSTOMER_OPTIONS_PARSED`
- `CRAFTINGORDERS_DISPLAY_CRAFTER_FULFILLED_MSG`: orderTypeString: cstring, itemNameString: cstring, playerNameString: cstring, tipAmount: WOWMONEY, quantityCrafted: number
- `CRAFTINGORDERS_FULFILL_ORDER_RESPONSE`: result: CraftingOrderResult, orderID: BigUInteger
- `CRAFTINGORDERS_HIDE_CRAFTER`
- `CRAFTINGORDERS_HIDE_CUSTOMER`
- `CRAFTINGORDERS_ORDER_CANCEL_RESPONSE`: result: CraftingOrderResult
- `CRAFTINGORDERS_ORDER_PLACEMENT_RESPONSE`: result: CraftingOrderResult
- `CRAFTINGORDERS_REJECT_ORDER_RESPONSE`: result: CraftingOrderResult, orderID: BigUInteger
- `CRAFTINGORDERS_RELEASE_ORDER_RESPONSE`: result: CraftingOrderResult, orderID: BigUInteger
- `CRAFTINGORDERS_SHOW_CRAFTER`
- `CRAFTINGORDERS_SHOW_CUSTOMER`
- `CRAFTINGORDERS_UNEXPECTED_ERROR`
- `CRAFTINGORDERS_UPDATE_CUSTOMER_NAME`: customerName: cstring, orderID: BigUInteger
- `CRAFTINGORDERS_UPDATE_ORDER_COUNT`: orderType: CraftingOrderType, numOrders: number
- `CRAFTINGORDERS_UPDATE_PERSONAL_ORDER_COUNTS`
- `CRAFTINGORDERS_UPDATE_REWARDS`: npcOrderRewards: CraftingOrderRewardInfo[], orderID: BigUInteger
- `CRAFTING_HOUSE_DISABLED`

## CurrencySystem

See [CurrencySystem](systems/CurrencySystem.md).

- `ACCOUNT_CHARACTER_CURRENCY_DATA_RECEIVED`
- `ACCOUNT_MONEY`
- `CURRENCY_DISPLAY_UPDATE`: currencyType: number?, quantity: number?, quantityChange: number?, quantityGainSource: number?, destroyReason: number?
- `CURRENCY_TRANSFER_FAILED`: failureReason: AccountCurrencyTransferResult
- `CURRENCY_TRANSFER_INITIATED`
- `CURRENCY_TRANSFER_LOG_UPDATE`
- `CURRENCY_TRANSFER_SUCCESS`
- `PLAYER_MONEY`

## Cursor

See [Cursor](systems/Cursor.md).

- `BATTLE_PET_CURSOR_CLEAR`
- `CURSOR_CHANGED`: isDefault: bool, newCursorType: UICursorType, oldCursorType: UICursorType, oldCursorVirtualID: number
- `MOUNT_CURSOR_CLEAR`
- `WORLD_CURSOR_TOOLTIP_UPDATE`: anchorType: WorldCursorAnchorType

## DamageMeter

See [DamageMeter](systems/DamageMeter.md).

- `DAMAGE_METER_COMBAT_SESSION_UPDATED`: type: DamageMeterType, sessionID: number
- `DAMAGE_METER_CURRENT_SESSION_UPDATED`
- `DAMAGE_METER_RESET`

## DateAndTime

See [DateAndTime](systems/DateAndTime.md).

- `DIEL_CYCLE_CHANGED`: isDayTime: bool

## DeathAlert

See [DeathAlert](systems/DeathAlert.md).

- `HARDCORE_DEATHS`: memberName: cstring

## DeathInfo

See [DeathInfo](systems/DeathInfo.md).

- `AREA_SPIRIT_HEALER_IN_RANGE`
- `AREA_SPIRIT_HEALER_OUT_OF_RANGE`
- `CEMETERY_PREFERENCE_UPDATED`
- `CONFIRM_XP_LOSS`
- `CORPSE_IN_INSTANCE`
- `CORPSE_IN_RANGE`
- `CORPSE_OUT_OF_RANGE`
- `PLAYER_ALIVE`
- `PLAYER_DEAD`
- `PLAYER_SKINNED`: hasFreeRepop: number
- `PLAYER_UNGHOST`
- `REQUEST_CEMETERY_LIST_RESPONSE`: isGossipTriggered: bool
- `RESURRECT_REQUEST`: inviter: cstring
- `SELF_RES_SPELL_CHANGED`

## DelvesUI

See [DelvesUI](systems/DelvesUI.md).

- `ACTIVE_DELVE_DATA_UPDATE`
- `DELVES_ACCOUNT_DATA_ELEMENT_CHANGED`
- `DELVE_ASSIST_ACTION`: data: DelveAssistActionData
- `PARTY_ELIGIBILITY_FOR_DELVE_TIERS_CHANGED`: playerName: string, maxEligibleLevel: number
- `SHOW_DELVES_COMPANION_CONFIGURATION_UI`
- `WALK_IN_DATA_UPDATE`

## Discord

See [Discord](systems/Discord.md).

- `DISCORD_GUILD_ACHIEVEMENT`: achievementID: number
- `DISCORD_GUILD_LOBBY_UPDATE`
- `DISCORD_GUILD_SETTINGS_UPDATE`
- `DISCORD_LINK_UPDATE`
- `DISCORD_SERVER_LIST_UPDATE`
- `DISCORD_STATUS_UPDATE`

## DuelInfo

See [DuelInfo](systems/DuelInfo.md).

- `DUEL_FINISHED`
- `DUEL_INBOUNDS`
- `DUEL_OUTOFBOUNDS`
- `DUEL_REQUESTED`: playerName: cstring
- `DUEL_TO_THE_DEATH_REQUESTED`: playerName: cstring

## DyeColorInfo

See [DyeColorInfo](systems/DyeColorInfo.md).

- `DYE_COLOR_CATEGORY_UPDATED`: dyeColorCategoryID: number
- `DYE_COLOR_UPDATED`: dyeColorID: number

## EditModeManager

See [EditModeManager](systems/EditModeManager.md).

- `EDIT_MODE_LAYOUTS_UPDATED`: layoutInfo: EditModeLayouts, reconcileLayouts: bool

## EncounterInfo

See [EncounterInfo](systems/EncounterInfo.md).

- `BOSS_KILL`: encounterID: number, encounterName: cstring
- `DISABLE_LOW_LEVEL_RAID`
- `ENABLE_LOW_LEVEL_RAID`
- `ENCOUNTER_END`: encounterID: number, encounterName: cstring, difficultyID: number, groupSize: number, success: number, encounterUnitStatus: EncounterUnitStatus[]
- `ENCOUNTER_START`: encounterID: number, encounterName: cstring, difficultyID: number, groupSize: number
- `INSTANCE_LOCK_START`
- `INSTANCE_LOCK_STOP`
- `INSTANCE_LOCK_WARNING`
- `RAID_TARGET_UPDATE`
- `UPDATE_INSTANCE_INFO`

## EncounterJournal

See [EncounterJournal](systems/EncounterJournal.md).

- `EJ_DIFFICULTY_UPDATE`: difficultyID: number
- `EJ_LOOT_DATA_RECIEVED`: itemID: number?
- `SHOW_JOURNEYS_UI`: factionID: number

## EncounterTimeline

See [EncounterTimeline](systems/EncounterTimeline.md).

- `ENCOUNTER_TIMELINE_EVENT_ADDED`: eventInfo: EncounterTimelineEventInfo
- `ENCOUNTER_TIMELINE_EVENT_BLOCK_STATE_CHANGED`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_EVENT_COLOR_CHANGED`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_EVENT_HIGHLIGHT`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_EVENT_REMOVED`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_EVENT_STATE_CHANGED`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_EVENT_TRACK_CHANGED`: eventID: EncounterTimelineEventID
- `ENCOUNTER_TIMELINE_LAYOUT_UPDATED`
- `ENCOUNTER_TIMELINE_STATE_UPDATED`
- `ENCOUNTER_TIMELINE_VIEW_ACTIVATED`: viewType: EncounterTimelineViewType
- `ENCOUNTER_TIMELINE_VIEW_DEACTIVATED`: viewType: EncounterTimelineViewType

## EncounterWarnings

See [EncounterWarnings](systems/EncounterWarnings.md).

- `ENCOUNTER_WARNING`: encounterWarningInfo: EncounterWarningInfo

## EndOfMatchUI

See [EndOfMatchUI](systems/EndOfMatchUI.md).

- `SHOW_END_OF_MATCH_UI`

## EquipmentSet

See [EquipmentSet](systems/EquipmentSet.md).

- `EQUIPMENT_SETS_CHANGED`
- `EQUIPMENT_SWAP_FINISHED`: result: bool, setID: number?
- `EQUIPMENT_SWAP_PENDING`
- `TRANSMOG_CUSTOM_SETS_CHANGED`

## EventSchedulerUI

See [EventSchedulerUI](systems/EventSchedulerUI.md).

- `EVENT_SCHEDULER_UPDATE`

## Expansion

See [Expansion](systems/Expansion.md).

- `MAX_EXPANSION_LEVEL_UPDATED`
- `MIN_EXPANSION_LEVEL_UPDATED`
- `SHOW_SUBSCRIPTION_INTERSTITIAL`: type: SubscriptionInterstitialType

## ExternalEventURL

See [ExternalEventURL](systems/ExternalEventURL.md).

- `EXTERNAL_EVENT_LAUNCH_URL_RESULT`: result: bool
- `EXTERNAL_EVENT_URL_CHANGED`

## FogOfWar

See [FogOfWar](systems/FogOfWar.md).

- `FOG_OF_WAR_UPDATED`

## FriendList

See [FriendList](systems/FriendList.md).

- `BATTLE_NET_FRIEND_TAG_ENABLED_STATUS_UPDATED`
- `BATTLE_NET_TITLE_FRIEND_CUSTOM_NAME_ENABLED_STATUS_UPDATED`
- `BN_BLOCK_FAILED_TOO_MANY`: blockType: cstring
- `BN_BLOCK_LIST_UPDATED`
- `BN_CHAT_WHISPER_UNDELIVERABLE`: senderID: number
- `BN_CONNECTED`: suppressNotification: bool
- `BN_CUSTOM_MESSAGE_CHANGED`: id: number?
- `BN_CUSTOM_MESSAGE_LOADED`
- `BN_DISCONNECTED`: result: bool, suppressNotification: bool
- `BN_FRIEND_ACCOUNT_OFFLINE`: friendId: number, isCompanionApp: bool
- `BN_FRIEND_ACCOUNT_ONLINE`: friendId: number, isCompanionApp: bool
- `BN_FRIEND_INFO_CHANGED`: friendIndex: luaIndex?
- `BN_FRIEND_INVITE_ADDED`: accountID: number
- `BN_FRIEND_INVITE_LIST_INITIALIZED`: listSize: number
- `BN_FRIEND_INVITE_REMOVED`
- `BN_FRIEND_LIST_SIZE_CHANGED`: accountID: number?
- `BN_INFO_CHANGED`
- `BN_REQUEST_FOF_SUCCEEDED`
- `CONFIRM_BATTLE_NET_FRIEND_INVITE_SHOW`: name: cstring, friendLevel: BattleNetFriendLevel
- `FRIENDLIST_UPDATE`
- `IGNORELIST_UPDATE`
- `LEGACY_FRIEND_SYSTEM_STATUS_UPDATED`
- `MUTELIST_UPDATE`
- `NEW_MATCHMAKING_PARTY_INVITE`
- `REJECTED_MATCHMAKING_PARTY_INVITE`: name: cstring
- `SOCIAL_UI_FRIENDS_LIST_SYSTEM_STATUS_UPDATED`
- `WHO_LIST_UPDATE`

## GamePad

See [GamePad](systems/GamePad.md).

- `GAME_PAD_ACTIVE_CHANGED`: isActive: bool
- `GAME_PAD_ALLOW_HOVER_EVENTS_WITH_FREE_LOOK_CHANGED`: enabled: bool
- `GAME_PAD_CONFIGS_CHANGED`
- `GAME_PAD_CONNECTED`
- `GAME_PAD_DISCONNECTED`
- `GAME_PAD_POWER_CHANGED`: powerLevel: GamePadPowerLevel

## GamepadUI

See [GamepadUI](systems/GamepadUI.md).

- `GAMEPAD_POSSESS_BAR_OVERRIDE_CHANGED`: oldOverride: GamepadPossessBarOverride, newOverride: GamepadPossessBarOverride
- `GAMEPAD_STANCE_BAR_OVERRIDE_CHANGED`: oldOverride: GamepadStanceBarOverride, newOverride: GamepadStanceBarOverride

## GameRules

See [GameRules](systems/GameRules.md).

- `ACTIVE_GAME_MODE_UPDATED`: gameMode: GameMode
- `AVAILABLE_GAME_MODES_UPDATED`
- `EVENT_REALM_QUEUES_UPDATED`: eventRealmQueues: EventRealmQueues
- `GAME_MODE_DISPLAY_INFO_UPDATED`
- `GAME_MODE_DISPLAY_MODE_TOGGLE_DISABLED`: gameModeRecordID: number, disabled: bool
- `GAME_RULES_CHANGED`

## GarrisonInfo

See [GarrisonInfo](systems/GarrisonInfo.md).

- `GARRISON_ARCHITECT_CLOSED`
- `GARRISON_ARCHITECT_OPENED`: followerTypeID: number
- `GARRISON_BUILDING_ACTIVATABLE`: buildingName: cstring, garrisonType: number
- `GARRISON_BUILDING_ACTIVATED`: garrisonPlotInstanceID: number, garrisonBuildingID: number
- `GARRISON_BUILDING_ERROR`
- `GARRISON_BUILDING_LIST_UPDATE`: categoryID: number
- `GARRISON_BUILDING_PLACED`: garrisonPlotInstanceID: number, newPlacement: bool
- `GARRISON_BUILDING_REMOVED`: garrPlotInstanceID: number, garrBuildingID: number
- `GARRISON_BUILDING_UPDATE`: garrisonBuildingID: number, garrPlotInstanceID: number?
- `GARRISON_FOLLOWER_ADDED`: followerDbID: GarrisonFollower, followerName: cstring, followerClassName: cstring, followerLevel: number, followerQuality: number, isUpgraded: bool, textureKit: textureKit, followerTypeID: number
- `GARRISON_FOLLOWER_CATEGORIES_UPDATED`
- `GARRISON_FOLLOWER_DURABILITY_CHANGED`: garrFollowerTypeID: number, followerDbID: GarrisonFollower, followerDurability: number
- `GARRISON_FOLLOWER_HEALED`: followerID: GarrisonFollower
- `GARRISON_FOLLOWER_LIST_UPDATE`: followerTypeID: number
- `GARRISON_FOLLOWER_REMOVED`: followerTypeID: number
- `GARRISON_FOLLOWER_UPGRADED`: followerDbID: GarrisonFollower
- `GARRISON_FOLLOWER_XP_CHANGED`: garrFollowerTypeID: number, followerDbID: GarrisonFollower, xpChange: number, oldFollowerXp: number, oldFollowerLevel: number, oldFollowerQuality: number
- `GARRISON_HIDE_LANDING_PAGE`
- `GARRISON_INVASION_AVAILABLE`
- `GARRISON_INVASION_UNAVAILABLE`
- `GARRISON_LANDINGPAGE_SHIPMENTS`
- `GARRISON_MISSION_AREA_BONUS_ADDED`: garrisonMissonBonusAbilityID: number
- `GARRISON_MISSION_BONUS_ROLL_COMPLETE`: missionID: number, success: bool
- `GARRISON_MISSION_COMPLETE_RESPONSE`: missionID: number, canComplete: bool, success: bool, bonusRollSuccess: bool, followerDeaths: GarrisonFollowerDeathInfo[], autoCombatResult: AutoCombatResult?
- `GARRISON_MISSION_FINISHED`: followerTypeID: number, missionID: number
- `GARRISON_MISSION_LIST_UPDATE`: garrFollowerTypeID: number
- `GARRISON_MISSION_NPC_CLOSED`
- `GARRISON_MISSION_NPC_OPENED`: followerTypeID: number
- `GARRISON_MISSION_REWARD_INFO`: missionID: number, followerDbID: GarrisonFollower
- `GARRISON_MISSION_STARTED`: garrFollowerTypeID: number, missionID: number
- `GARRISON_MONUMENT_CLOSE_UI`
- `GARRISON_MONUMENT_LIST_LOADED`: success: bool
- `GARRISON_MONUMENT_REPLACED`: success: bool
- `GARRISON_MONUMENT_SELECTED_TROPHY_ID_LOADED`: success: bool
- `GARRISON_MONUMENT_SHOW_UI`
- `GARRISON_RANDOM_MISSION_ADDED`: followerTypeID: number, missionID: number
- `GARRISON_RECALL_PORTAL_LAST_USED_TIME`: success: bool, recallPortalLastUsedTime: number
- `GARRISON_RECALL_PORTAL_USED`: success: bool
- `GARRISON_RECRUITMENT_FOLLOWERS_GENERATED`
- `GARRISON_RECRUITMENT_NPC_CLOSED`
- `GARRISON_RECRUITMENT_NPC_OPENED`: followerTypeID: number
- `GARRISON_RECRUITMENT_READY`
- `GARRISON_RECRUIT_FOLLOWER_RESULT`
- `GARRISON_SHIPMENT_RECEIVED`
- `GARRISON_SHIPYARD_NPC_CLOSED`
- `GARRISON_SHIPYARD_NPC_OPENED`: followerTypeID: number
- `GARRISON_SHOW_LANDING_PAGE`
- `GARRISON_SPEC_GROUPS_CLEARED`: garrTypeID: number
- `GARRISON_SPEC_GROUP_UPDATED`: garrTypeID: number, specID: number
- `GARRISON_TALENT_COMPLETE`: garrTypeID: number, doAlert: bool
- `GARRISON_TALENT_EVENT_UPDATE`: eventType: number, eventID: number
- `GARRISON_TALENT_NPC_CLOSED`
- `GARRISON_TALENT_NPC_OPENED`: garrisonTypeID: number, garrisonTalentTreeID: number
- `GARRISON_TALENT_RESEARCH_STARTED`: garrTypeID: number, garrisonTalentTreeID: number, garrTalentID: number
- `GARRISON_TALENT_UNLOCKS_RESULT`
- `GARRISON_TALENT_UPDATE`: garrTypeID: number
- `GARRISON_TRADESKILL_NPC_CLOSED`
- `GARRISON_UPDATE`
- `GARRISON_UPGRADEABLE_RESULT`: garrisonUpgradeable: bool
- `GARRISON_USE_PARTY_GARRISON_CHANGED`
- `SHIPMENT_CRAFTER_CLOSED`
- `SHIPMENT_CRAFTER_INFO`: success: number, shipmentCount: number, maxShipments: number, ownedShipments: number, plotInstanceID: number
- `SHIPMENT_CRAFTER_OPENED`: charShipmentContainerID: number
- `SHIPMENT_CRAFTER_REAGENT_UPDATE`
- `SHIPMENT_UPDATE`: shipmentStarted: bool?, hasAttachedFollower: bool?

## GenericWidgetDisplay

See [GenericWidgetDisplay](systems/GenericWidgetDisplay.md).

- `GENERIC_WIDGET_DISPLAY_SHOW`: info: GenericWidgetDisplayFrameInfo

## Glue

See [Glue](systems/Glue.md).

- `ACCOUNT_CVARS_LOADED`

## GlyphInfo

See [GlyphInfo](systems/GlyphInfo.md).

- `ACTIVATE_GLYPH`: spellID: number
- `CANCEL_GLYPH_CAST`
- `USE_GLYPH`: spellID: number

## GMTicketInfo

See [GMTicketInfo](systems/GMTicketInfo.md).

- `GM_PLAYER_INFO`: name: cstring, info: cstring
- `ITEM_RESTORATION_BUTTON_STATUS`
- `PETITION_CLOSED`
- `PETITION_SHOW`
- `PLAYER_REPORT_SUBMITTED`: invitedByGUID: WOWGUID
- `QUICK_TICKET_SYSTEM_STATUS`
- `QUICK_TICKET_THROTTLE_CHANGED`
- `UPDATE_WEB_TICKET`: hasTicket: bool, numTickets: number?, ticketStatus: number?, caseIndex: number?, waitTimeMinutes: number?, waitMessage: cstring?, caseTitle: cstring?, caseDescription: cstring?

## GossipInfo

See [GossipInfo](systems/GossipInfo.md).

- `DYNAMIC_GOSSIP_POI_UPDATED`
- `GOSSIP_CLOSED`: interactionIsContinuing: bool
- `GOSSIP_CONFIRM`: gossipID: number, text: string, cost: WOWMONEY
- `GOSSIP_CONFIRM_CANCEL`
- `GOSSIP_ENTER_CODE`: gossipID: number
- `GOSSIP_OPTIONS_REFRESHED`
- `GOSSIP_SHOW`: uiTextureKit: textureKit?

## GuildBank

See [GuildBank](systems/GuildBank.md).

- `GUILDBANKBAGSLOTS_CHANGED`
- `GUILDBANKFRAME_CLOSED`
- `GUILDBANKFRAME_OPENED`
- `GUILDBANKLOG_UPDATE`
- `GUILDBANK_ITEM_LOCK_CHANGED`
- `GUILDBANK_TEXT_CHANGED`: guildBankTab: luaIndex
- `GUILDBANK_UPDATE_MONEY`
- `GUILDBANK_UPDATE_TABS`
- `GUILDBANK_UPDATE_TEXT`: guildBankTab: number
- `GUILDBANK_UPDATE_WITHDRAWMONEY`

## GuildInfo

See [GuildInfo](systems/GuildInfo.md).

- `CLOSE_TABARD_FRAME`
- `DISABLE_DECLINE_GUILD_INVITE`
- `ENABLE_DECLINE_GUILD_INVITE`
- `GUILDTABARD_UPDATE`
- `GUILD_CHALLENGE_COMPLETED`: challengeType: number, currentCount: number, maxCount: number, goldAwarded: number
- `GUILD_CHALLENGE_UPDATED`
- `GUILD_EVENT_LOG_UPDATE`
- `GUILD_INVITE_CANCEL`
- `GUILD_INVITE_REQUEST`: inviter: cstring, guildName: cstring, guildAchievementPoints: number, oldGuildName: cstring, isNewGuild: bool?, tabardInfo: GuildTabardInfo?
- `GUILD_MOTD`: motdText: cstring
- `GUILD_NEWS_UPDATE`
- `GUILD_PARTY_STATE_UPDATED`: inGuildParty: bool
- `GUILD_PREFERRED_PLAY_SETTINGS_UPDATED`: status: PreferredPlaySettingsStatus, preferredLocaleID: number, preferredDatacenterLocalityID: number, lastPreferredLocaleChangeDate: time_t, lastPreferredDatacenterLocalityChangeDate: time_t
- `GUILD_RANKS_UPDATE`
- `GUILD_RANKS_UPDATE_ACTIVE_PLAYER`
- `GUILD_RECIPE_KNOWN_BY_MEMBERS`
- `GUILD_REGISTRAR_CLOSED`
- `GUILD_REGISTRAR_SHOW`
- `GUILD_RENAME_NAME_CHECK`: desiredName: cstring, status: GuildErrorType, nameErrorToken: cstring?
- `GUILD_RENAME_REFUND_RESULT`: guildName: cstring, status: GuildErrorType
- `GUILD_RENAME_REQUIRED`: flagSet: bool
- `GUILD_RENAME_STATUS_UPDATE`: status: GuildRenameStatus
- `GUILD_REWARDS_LIST`
- `GUILD_REWARDS_LIST_UPDATE`
- `GUILD_ROSTER_UPDATE`: canRequestRosterUpdate: bool
- `GUILD_TRADESKILL_UPDATE`
- `OPEN_TABARD_FRAME`
- `PLAYER_GUILD_UPDATE`: unitTarget: UnitTokenVariant
- `REQUESTED_GUILD_RENAME_RESULT`: newName: cstring, status: GuildErrorType
- `REQUIRED_GUILD_RENAME_RESULT`: success: bool
- `TABARD_CANSAVE_CHANGED`
- `TABARD_SAVE_PENDING`
- `UNIT_GUILD_LEVEL`: newLevel: number

## HeirloomInfo

See [HeirloomInfo](systems/HeirloomInfo.md).

- `HEIRLOOMS_UPDATED`: itemID: number?, updateReason: cstring?, hideUntilLearned: bool?
- `HEIRLOOM_UPGRADE_TARGETING_CHANGED`: pendingHeirloomUpgradeSpellcast: bool

## HouseEditorUI

See [HouseEditorUI](systems/HouseEditorUI.md).

- `HOUSE_EDITOR_AVAILABILITY_CHANGED`
- `HOUSE_EDITOR_MODE_CHANGED`: currentEditMode: HouseEditorMode
- `HOUSE_EDITOR_MODE_CHANGE_FAILURE`: result: HousingResult

## HouseExteriorUI

See [HouseExteriorUI](systems/HouseExteriorUI.md).

- `HOUSE_EXTERIOR_DECOR_HIDDEN_CHANGED`: isDecorHidden: bool
- `HOUSE_EXTERIOR_TYPE_UNLOCKED`: fixtureID: number
- `HOUSING_CORE_FIXTURE_CHANGED`: coreFixtureType: HousingFixtureType
- `HOUSING_FIXTURE_HOVER_CHANGED`: anyHovered: bool
- `HOUSING_FIXTURE_POINT_FRAMES_RELEASED`
- `HOUSING_FIXTURE_POINT_FRAME_ADDED`: pointFrame: HousingFixturePointFrame
- `HOUSING_FIXTURE_POINT_FRAME_RELEASED`: pointFrame: HousingFixturePointFrame
- `HOUSING_FIXTURE_POINT_SELECTION_CHANGED`: hasSelection: bool
- `HOUSING_FIXTURE_UNLOCKED`: fixtureID: number
- `HOUSING_SET_EXTERIOR_HOUSE_SIZE_RESPONSE`: result: HousingResult
- `HOUSING_SET_EXTERIOR_HOUSE_TYPE_RESPONSE`: result: HousingResult
- `HOUSING_SET_FIXTURE_RESPONSE`: result: HousingResult

## HousingBasicModeUI

See [HousingBasicModeUI](systems/HousingBasicModeUI.md).

- `HOUSING_BASIC_MODE_HOVERED_TARGET_CHANGED`: hasHoveredTarget: bool, targetType: HousingBasicModeTargetType
- `HOUSING_BASIC_MODE_PLACEMENT_FLAGS_UPDATED`: targetType: HousingBasicModeTargetType, activeFlags: HousingDecorPlacementRestriction
- `HOUSING_BASIC_MODE_SELECTED_TARGET_CHANGED`: hasSelectedTarget: bool, targetType: HousingBasicModeTargetType, isPreview: bool
- `HOUSING_DECOR_FREE_PLACE_STATUS_CHANGED`: isFreePlaceEnabled: bool
- `HOUSING_DECOR_GRID_SNAP_OCCURRED`
- `HOUSING_DECOR_GRID_SNAP_STATUS_CHANGED`: isGridSnapEnabled: bool

## HousingBlueprintUI

See [HousingBlueprintUI](systems/HousingBlueprintUI.md).

- `HOUSING_BLUEPRINTS_AVAILABILITY_CHANGED`
- `HOUSING_BLUEPRINT_COLLECTION_FAILURE`: result: HousingResult
- `HOUSING_BLUEPRINT_COLLECTION_RECEIVED`: collection: HousingBlueprintCollection
- `HOUSING_BLUEPRINT_CONTENTS_FAILURE`: blueprintShareCode: string, result: HousingResult
- `HOUSING_BLUEPRINT_CONTENTS_RECEIVED`: contentInfo: HousingBlueprintContentInfo
- `HOUSING_BLUEPRINT_DELETE_FAILURE`: blueprintID: BigUInteger, result: HousingResult
- `HOUSING_BLUEPRINT_DELETE_SUCCESS`: blueprintID: BigUInteger
- `HOUSING_BLUEPRINT_EXPORT_FAILURE`: result: HousingResult
- `HOUSING_BLUEPRINT_EXPORT_SUCCESS`: blueprintShareCode: string
- `HOUSING_BLUEPRINT_IMPORT_FAILURE`: result: HousingResult
- `HOUSING_BLUEPRINT_IMPORT_STARTED`
- `HOUSING_BLUEPRINT_IMPORT_SUCCESS`
- `HOUSING_BLUEPRINT_RENAME_FAILURE`: blueprintID: BigUInteger, result: HousingResult
- `HOUSING_BLUEPRINT_RENAME_SUCCESS`: blueprintID: BigUInteger, name: string

## HousingCatalogUI

See [HousingCatalogUI](systems/HousingCatalogUI.md).

- `HOUSING_CATALOG_CATEGORY_UPDATED`: categoryID: number
- `HOUSING_CATALOG_SUBCATEGORY_UPDATED`: subcategoryID: number
- `HOUSING_DECOR_ADD_TO_PREVIEW_LIST`: previewItemData: HousingPreviewItemData
- `HOUSING_DECOR_PREVIEW_LIST_REMOVE_FROM_WORLD`: decorGUID: WOWGUID
- `HOUSING_DECOR_PREVIEW_LIST_UPDATED`
- `HOUSING_REFUND_LIST_UPDATED`
- `HOUSING_STORAGE_ENTRY_UPDATED`: entryVariantID: HousingCatalogEntryVariantID
- `HOUSING_STORAGE_UPDATED`

## HousingCleanupModeUI

See [HousingCleanupModeUI](systems/HousingCleanupModeUI.md).

- `HOUSING_CLEANUP_MODE_HOVERED_TARGET_CHANGED`: hasHoveredTarget: bool, targetType: HousingCleanupModeTargetType
- `HOUSING_CLEANUP_MODE_TARGET_SELECTED`

## HousingCustomizeModeUI

See [HousingCustomizeModeUI](systems/HousingCustomizeModeUI.md).

- `HOUSING_CUSTOMIZE_MODE_HOVERED_TARGET_CHANGED`: hasHoveredTarget: bool, targetType: HousingCustomizeModeTargetType
- `HOUSING_CUSTOMIZE_MODE_SELECTED_TARGET_CHANGED`: hasSelectedTarget: bool, targetType: HousingCustomizeModeTargetType
- `HOUSING_DECOR_CUSTOMIZATION_CHANGED`: decorGUID: WOWGUID
- `HOUSING_DECOR_DYE_FAILURE`: decorGUID: WOWGUID, housingResult: HousingResult
- `HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGED`: roomGUID: WOWGUID, componentID: number
- `HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGE_FAILED`: roomGUID: WOWGUID, componentID: number, housingResult: HousingResult

## HousingDecorUI

See [HousingDecorUI](systems/HousingDecorUI.md).

- `HOUSE_DECOR_ADDED_TO_CHEST`: decorGUID: WOWGUID, decorID: number
- `HOUSE_EXTERIOR_POSITION_FAILURE`: housingResult: HousingResult
- `HOUSE_EXTERIOR_POSITION_SUCCESS`
- `HOUSING_DECOR_GRID_VISIBILITY_STATUS_CHANGED`: isGridVisible: bool
- `HOUSING_DECOR_PLACE_FAILURE`: housingResult: HousingResult
- `HOUSING_DECOR_PLACE_SUCCESS`: decorGUID: WOWGUID, size: HousingCatalogEntrySize, isNew: bool, isPreview: bool
- `HOUSING_DECOR_PREVIEW_STATE_CHANGED`: isPreviewState: bool
- `HOUSING_DECOR_REMOVED`: decorGUID: WOWGUID
- `HOUSING_DECOR_SELECT_RESPONSE`: result: HousingResult
- `HOUSING_NEW_DECOR_PLACE_COMPLETE`: decorGUID: WOWGUID
- `HOUSING_NUM_DECOR_PLACED_CHANGED`

## HousingExpertModeUI

See [HousingExpertModeUI](systems/HousingExpertModeUI.md).

- `HOUSING_DECOR_PRECISION_MANIPULATION_EVENT`: event: TransformManipulatorEvent
- `HOUSING_DECOR_PRECISION_MANIPULATION_STATUS_CHANGED`: isManipulatingSelection: bool
- `HOUSING_DECOR_PRECISION_SUBMODE_CHANGED`: activeSubmode: HousingPrecisionSubmode?
- `HOUSING_EXPERT_MODE_HOVERED_TARGET_CHANGED`: hasHoveredTarget: bool, targetType: HousingExpertModeTargetType
- `HOUSING_EXPERT_MODE_PLACEMENT_FLAGS_UPDATED`: targetType: HousingExpertModeTargetType, activeFlags: HousingDecorPlacementRestriction
- `HOUSING_EXPERT_MODE_SELECTED_TARGET_CHANGED`: hasSelectedTarget: bool, targetType: HousingExpertModeTargetType

## HousingInspectModeUI

See [HousingInspectModeUI](systems/HousingInspectModeUI.md).

- `HOUSING_INSPECT_MODE_DECOR_HOVERED_CHANGED`
- `HOUSING_INSPECT_MODE_STATE_UPDATED`

## HousingLayoutUI

See [HousingLayoutUI](systems/HousingLayoutUI.md).

- `HOUSING_LAYOUT_DOOR_SELECTED`: roomGUID: WOWGUID, componentID: number
- `HOUSING_LAYOUT_DOOR_SELECTION_CHANGED`: hasSelection: bool
- `HOUSING_LAYOUT_DRAG_TARGET_CHANGED`: isDraggingRoom: bool
- `HOUSING_LAYOUT_FLOORPLAN_SELECTION_CHANGED`: hasSelection: bool, roomID: number, blueprintShareCode: cstring?
- `HOUSING_LAYOUT_OCCUPIED_FLOOR_RANGE_CHANGED`: lowestFloor: number, highestFloor: number
- `HOUSING_LAYOUT_PIN_FRAMES_RELEASED`
- `HOUSING_LAYOUT_PIN_FRAME_ADDED`: pinFrame: HousingLayoutPinFrame
- `HOUSING_LAYOUT_PIN_FRAME_RELEASED`: pinFrame: HousingLayoutPinFrame
- `HOUSING_LAYOUT_ROOM_COMPONENT_THEME_SET_CHANGED`: roomGUID: WOWGUID, componentID: number, newThemeSet: number, result: HousingResult
- `HOUSING_LAYOUT_ROOM_MOVED`
- `HOUSING_LAYOUT_ROOM_MOVE_INVALID`
- `HOUSING_LAYOUT_ROOM_RECEIVED`: playAddedSound: bool
- `HOUSING_LAYOUT_ROOM_REMOVED`
- `HOUSING_LAYOUT_ROOM_RETURNED`
- `HOUSING_LAYOUT_ROOM_SELECTION_CHANGED`: hasSelection: bool
- `HOUSING_LAYOUT_ROOM_SNAPPED`
- `HOUSING_LAYOUT_VIEWED_FLOOR_CHANGED`: floor: number
- `SHOW_STAIR_DIRECTION_CONFIRMATION`

## HousingNeighborhoodUI

See [HousingNeighborhoodUI](systems/HousingNeighborhoodUI.md).

- `CANCEL_NEIGHBORHOOD_INVITE_RESPONSE`: result: NeighborhoodInviteResult, playerName: cstring?
- `CLOSE_PLOT_CORNERSTONE`
- `NEIGHBORHOOD_INFO_UPDATED`: neighborhoodInfo: NeighborhoodInfo
- `NEIGHBORHOOD_INVITE_RESPONSE`: result: NeighborhoodInviteResult
- `NEIGHBORHOOD_MAP_DATA_UPDATED`
- `NEIGHBORHOOD_NAME_UPDATED`: neighborhoodGuid: WOWGUID, neighborhoodName: cstring
- `OPEN_PLOT_CORNERSTONE`
- `PENDING_NEIGHBORHOOD_INVITES_RECIEVED`: result: NeighborhoodInviteResult, pendingInviteList: string[]?
- `PURCHASE_PLOT_RESULT`: result: number
- `SHOW_PLAYER_EVICTED_DIALOG`
- `UPDATE_BULLETIN_BOARD_MEMBER_TYPE`: player: WOWGUID, residentType: ResidentType
- `UPDATE_BULLETIN_BOARD_ROSTER`: neighborhoodInfo: NeighborhoodInfo, rosterMemberList: NeighborhoodRosterMemberInfo[]
- `UPDATE_BULLETIN_BOARD_ROSTER_STATUSES`: rosterMemberList: NeighborhoodRosterMemberUpdateInfo[]

## HousingUI

See [HousingUI](systems/HousingUI.md).

- `ADD_NEIGHBORHOOD_CHARTER_SIGNATURE`: signature: cstring
- `B_NET_NEIGHBORHOOD_LIST_UPDATED`: result: HousingResult, neighborhoodInfos: NeighborhoodInfo[]?
- `CLOSE_CHARTER_CONFIRMATION_UI`
- `CLOSE_CREATE_CHARTER_NEIGHBORHOOD_UI`
- `CLOSE_CREATE_GUILD_NEIGHBORHOOD_UI`
- `CREATE_NEIGHBORHOOD_RESULT`: result: HousingResult, neighborhoodName: cstring?
- `CURRENT_HOUSE_INFO_RECIEVED`: houseInfo: HouseInfo
- `CURRENT_HOUSE_INFO_UPDATED`: houseInfo: HouseInfo
- `DECLINE_NEIGHBORHOOD_INVITATION_RESPONSE`: success: bool
- `FORCE_REFRESH_HOUSE_FINDER`
- `HOUSE_FINDER_NEIGHBORHOOD_DATA_RECIEVED`: neighborhoodPlots: NeighborhoodPlotMapInfo[]
- `HOUSE_INFO_UPDATED`
- `HOUSE_LEVEL_CHANGED`: newHouseLevelInfo: HouseLevelInfo?
- `HOUSE_LEVEL_FAVOR_UPDATED`: houseLevelFavor: HouseLevelFavor
- `HOUSE_PLOT_ENTERED`
- `HOUSE_PLOT_EXITED`
- `HOUSE_RESERVATION_RESPONSE_RECIEVED`: result: HousingResult
- `HOUSE_RESET_COMPLETED`
- `HOUSE_RESET_FAILED`: result: HousingResult
- `HOUSING_MARKET_AVAILABILITY_UPDATED`
- `HOUSING_SERVICES_AVAILABILITY_UPDATED`
- `IGNORE_NEIGHBORHOOD_RESPONSE`: success: bool, neighborhoodGuid: WOWGUID
- `MOVE_OUT_RESERVATION_UPDATED`
- `NEIGHBORHOOD_GUILD_SIZE_VALIDATED`: approved: bool
- `NEIGHBORHOOD_LIST_UPDATED`: result: HousingResult, neighborhoodInfos: NeighborhoodInfo[]?
- `NEIGHBORHOOD_NAME_VALIDATED`: approved: bool
- `NEW_HOUSING_ITEM_ACQUIRED`: itemType: HousingItemToastType, itemName: cstring, icon: fileID?
- `OPEN_CHARTER_CONFIRMATION_UI`: neighborhoodName: string, locationName: string
- `OPEN_CREATE_CHARTER_NEIGHBORHOOD_UI`: locationName: cstring
- `OPEN_CREATE_GUILD_NEIGHBORHOOD_UI`: locationName: cstring
- `OPEN_NEIGHBORHOOD_CHARTER`: neighborhoodInfo: NeighborhoodInfo, signatures: string[], requiredSignatures: number
- `OPEN_NEIGHBORHOOD_CHARTER_SIGNATURE_REQUEST`: neighborhoodInfo: NeighborhoodInfo
- `PLAYER_CHARACTER_LIST_UPDATED`: characterInfos: HouseOwnerCharacterInfo[], ownerListIndex: number
- `PLAYER_HOUSE_LIST_UPDATED`: houseInfos: HouseInfo[]
- `RECEIVED_HOUSE_LEVEL_REWARDS`: level: number, rewards: HouseLevelReward[]
- `REMOVE_NEIGHBORHOOD_CHARTER_SIGNATURE`: signature: cstring
- `SHOW_NEIGHBORHOOD_OWNERSHIP_TRANSFER_DIALOG`: neighborhoodName: cstring, cosmeticOwnerName: cstring
- `TRACKED_HOUSE_CHANGED`: trackedHouse: WOWGUID?
- `VIEW_HOUSES_LIST_RECIEVED`: houseInfos: HouseInfo[]

## ImmersiveInteraction

See [ImmersiveInteraction](systems/ImmersiveInteraction.md).

- `IMMERSIVE_INTERACTION_BEGIN`
- `IMMERSIVE_INTERACTION_END`

## InGameNavigation

See [InGameNavigation](systems/InGameNavigation.md).

- `NAVIGATION_DESTINATION_REACHED`: isWaypoint: bool
- `NAVIGATION_FRAME_CREATED`: region: ScriptRegion
- `NAVIGATION_FRAME_DESTROYED`

## Input

See [Input](systems/Input.md).

- `INPUT_DEVICE_INTERFACE_TRANSITION`: newMode: InputDeviceInterfaceType, oldMode: InputDeviceInterfaceType

## InstanceEncounter

See [InstanceEncounter](systems/InstanceEncounter.md).

- `ENCOUNTER_STATE_CHANGED`: isInProgress: bool
- `INSTANCE_ENCOUNTER_ADD_TIMER`: timeRemaining: number
- `INSTANCE_ENCOUNTER_ENGAGE_UNIT`
- `INSTANCE_ENCOUNTER_OBJECTIVE_COMPLETE`: objectiveID: number
- `INSTANCE_ENCOUNTER_OBJECTIVE_START`: objectiveID: number, objectiveProgress: number
- `INSTANCE_ENCOUNTER_OBJECTIVE_UPDATE`: objectiveID: number, objectiveProgress: number

## InstanceLeaverInfo

See [InstanceLeaverInfo](systems/InstanceLeaverInfo.md).

- `INSTANCE_LEAVER_STATUS_CHANGED`: isLeaver: bool

## IslandsInfo

See [IslandsInfo](systems/IslandsInfo.md).

- `ISLAND_AZERITE_GAIN`: amount: number, gainedByPlayer: bool, factionIndex: number, gainedBy: WOWGUID, gainedFrom: WOWGUID

## IslandsQueue

See [IslandsQueue](systems/IslandsQueue.md).

- `ISLANDS_QUEUE_CLOSE`
- `ISLANDS_QUEUE_OPEN`

## Item

See [Item](systems/Item.md).

- `ACTION_WILL_BIND_ITEM`
- `BIND_ENCHANT`
- `CHARACTER_ITEM_FIXUP_NOTIFICATION`: fixupVersion: number
- `CONFIRM_BEFORE_USE`
- `CONVERT_TO_BIND_TO_ACCOUNT_CONFIRM`
- `DELETE_ITEM_CONFIRM`: itemName: cstring, qualityID: number, bonding: number, questWarn: number, itemGUID: WOWGUID?
- `END_BOUND_TRADEABLE`: reason: cstring
- `GET_ITEM_INFO_RECEIVED`: itemID: number, success: bool
- `ITEM_CHANGED`: previousHyperlink: string, newHyperlink: string
- `ITEM_CONVERSION_DATA_READY`: itemGUID: WOWGUID
- `ITEM_COUNT_CHANGED`: itemID: number
- `ITEM_DATA_LOAD_RESULT`: itemID: number, success: bool
- `MERCHANT_CONFIRM_TRADE_TIMER_REMOVAL`: itemLink: cstring
- `REPLACE_ENCHANT`: existingStr: cstring, replacementStr: cstring
- `REPLACE_TRADESKILL_ENCHANT`: existing: cstring, replacement: cstring
- `TRADE_REPLACE_ENCHANT`: existing: cstring, replacement: cstring
- `USE_BIND_CONFIRM`
- `USE_NO_REFUND_CONFIRM`
- `WEAPON_ENCHANT_CHANGED`

## ItemInteractionUI

See [ItemInteractionUI](systems/ItemInteractionUI.md).

- `ITEM_INTERACTION_CHARGE_INFO_UPDATED`
- `ITEM_INTERACTION_ITEM_SELECTION_UPDATED`: itemLocation: ItemLocation?

## ItemSocketInfo

See [ItemSocketInfo](systems/ItemSocketInfo.md).

- `SOCKET_INFO_ACCEPT`
- `SOCKET_INFO_BIND_CONFIRM`
- `SOCKET_INFO_CLOSE`
- `SOCKET_INFO_FAILURE`
- `SOCKET_INFO_REFUNDABLE_CONFIRM`
- `SOCKET_INFO_SUCCESS`
- `SOCKET_INFO_UI_EVENT_REGISTRATION_UPDATE`: uiType: ItemSocketInfoUIType
- `SOCKET_INFO_UPDATE`

## ItemText

See [ItemText](systems/ItemText.md).

- `ITEM_TEXT_BEGIN`
- `ITEM_TEXT_CLOSED`
- `ITEM_TEXT_READY`
- `ITEM_TEXT_TRANSLATION`: delay: number

## ItemUpgrade

See [ItemUpgrade](systems/ItemUpgrade.md).

- `ITEM_UPGRADE_FAILED`
- `ITEM_UPGRADE_MASTER_SET_ITEM`
- `ITEM_UPGRADE_MASTER_UPDATE`

## KeyBindings

See [KeyBindings](systems/KeyBindings.md).

- `BINDINGS_LOADED`
- `MODIFIER_STATE_CHANGED`: key: cstring, down: number
- `NOTIFY_TURN_STRAFE_CHANGE`
- `UPDATE_BINDINGS`

## LegendaryCrafting

See [LegendaryCrafting](systems/LegendaryCrafting.md).

- `NEW_RUNEFORGE_POWER_ADDED`: powerID: number
- `RUNEFORGE_LEGENDARY_CRAFTING_CLOSED`
- `RUNEFORGE_LEGENDARY_CRAFTING_OPENED`: isUpgrade: bool
- `RUNEFORGE_POWER_INFO_UPDATED`: powerID: number

## LFGInfo

See [LFGInfo](systems/LFGInfo.md).

- `ISLAND_COMPLETED`: mapID: number, winner: number
- `LFG_BOOT_PROPOSAL_UPDATE`
- `LFG_COMPLETION_REWARD`
- `LFG_COOLDOWNS_UPDATED`
- `LFG_ENABLED_STATE_CHANGED`
- `LFG_INVALID_ERROR_MESSAGE`: reason: number, subReason1: number, subReason2: number
- `LFG_LOCK_INFO_RECEIVED`
- `LFG_OFFER_CONTINUE`: name: cstring, lfgDungeonsID: number, typeID: number
- `LFG_OPEN_FROM_GOSSIP`: dungeonID: number
- `LFG_PROPOSAL_DONE`
- `LFG_PROPOSAL_FAILED`
- `LFG_PROPOSAL_SHOW`
- `LFG_PROPOSAL_SUCCEEDED`
- `LFG_PROPOSAL_UPDATE`
- `LFG_QUEUE_STATUS_UPDATE`
- `LFG_READY_CHECK_DECLINED`: name: cstring
- `LFG_READY_CHECK_HIDE`
- `LFG_READY_CHECK_PLAYER_IS_READY`: name: cstring
- `LFG_READY_CHECK_SHOW`: isRequeue: bool
- `LFG_READY_CHECK_UPDATE`
- `LFG_ROLE_CHECK_DECLINED`
- `LFG_ROLE_CHECK_HIDE`
- `LFG_ROLE_CHECK_ROLE_CHOSEN`: name: cstring, isTank: bool, isHealer: bool, isDamage: bool
- `LFG_ROLE_CHECK_SHOW`: isRequeue: bool
- `LFG_ROLE_CHECK_UPDATE`
- `LFG_ROLE_UPDATE`
- `LFG_UPDATE`
- `LFG_UPDATE_RANDOM_INFO`
- `SHOW_LFG_EXPAND_SEARCH_PROMPT`
- `UPDATE_LFG_LIST`
- `WARFRONT_COMPLETED`: mapID: number, winner: number

## LFGList

See [LFGList](systems/LFGList.md).

- `LFG_GROUP_DELISTED_LEADERSHIP_CHANGE`: listingName: string, automaticDelistTimeRemaining: number
- `LFG_LIST_ACTIVE_ENTRY_UPDATE`: created: bool?
- `LFG_LIST_APPLICANT_LIST_UPDATED`: newPendingEntry: bool?, newPendingEntryWithData: bool?
- `LFG_LIST_APPLICANT_UPDATED`: applicantID: number
- `LFG_LIST_APPLICATION_STATUS_UPDATED`: searchResultID: number, newStatus: cstring, oldStatus: cstring, groupName: kstringLfgListChat
- `LFG_LIST_AVAILABILITY_UPDATE`
- `LFG_LIST_CENSORED_ACTIVE_ENTRY_UPDATE`: isCensored: bool
- `LFG_LIST_ENTRY_CREATION_FAILED`
- `LFG_LIST_ENTRY_EXPIRED_TIMEOUT`
- `LFG_LIST_ENTRY_EXPIRED_TOO_MANY_PLAYERS`
- `LFG_LIST_JOINED_GROUP`: searchResultID: number, groupName: kstringLfgListChat
- `LFG_LIST_REVEALED_CENSORED_ACTIVE_ENTRY`
- `LFG_LIST_SEARCH_FAILED`: reason: cstring?
- `LFG_LIST_SEARCH_RESULTS_RECEIVED`
- `LFG_LIST_SEARCH_RESULT_UPDATED`: searchResultID: number
- `LFG_LIST_SHOW_SEARCH`: activityIDsFilter: number[]?, showAllLevelRanges: bool
- `LFG_LIST_UPDATE_SEARCH_RESULTS`

## LFGListRoles

See [LFGListRoles](systems/LFGListRoles.md).

- `LFG_LIST_ROLE_UPDATE`

## LoadingScreen

See [LoadingScreen](systems/LoadingScreen.md).

- `LOADING_SCREEN_DISABLED`
- `LOADING_SCREEN_ENABLED`

## LobbyMatchmakerInfo

See [LobbyMatchmakerInfo](systems/LobbyMatchmakerInfo.md).

- `LOBBY_MATCHMAKER_QUEUE_ABANDONED`
- `LOBBY_MATCHMAKER_QUEUE_ERROR`
- `LOBBY_MATCHMAKER_QUEUE_EXPIRED`
- `LOBBY_MATCHMAKER_QUEUE_POPPED`
- `LOBBY_MATCHMAKER_QUEUE_STATUS_UPDATE`

## Loot

See [Loot](systems/Loot.md).

- `AZERITE_EMPOWERED_ITEM_LOOTED`: itemLink: cstring
- `BONUS_ROLL_ACTIVATE`
- `BONUS_ROLL_DEACTIVATE`
- `BONUS_ROLL_FAILED`
- `BONUS_ROLL_RESULT`: typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, currencyID: number?, isSecondaryResult: bool, corrupted: bool
- `BONUS_ROLL_STARTED`
- `CANCEL_ALL_LOOT_ROLLS`
- `CANCEL_LOOT_ROLL`: rollID: number
- `CONFIRM_DISENCHANT_ROLL`: rollID: number, rollType: number
- `CONFIRM_LOOT_ROLL`: rollID: number, rollType: number, confirmReason: cstring
- `ENCOUNTER_LOOT_RECEIVED`: encounterID: number, itemID: number, itemLink: cstring, quantity: number, itemName: cstring, fileName: cstring
- `GARRISON_MISSION_BONUS_ROLL_LOOT`: itemID: number, quantity: number
- `ITEM_PUSH`: bagSlot: luaIndex, iconFileID: number
- `LEGACY_LOOT_RULES_CHANGED`: isLegacyLootModeEnabled: bool
- `LOOT_BIND_CONFIRM`: lootSlot: luaIndex
- `LOOT_CLOSED`
- `LOOT_ITEM_AVAILABLE`: itemTooltip: cstring, lootHandle: number
- `LOOT_ITEM_ROLL_WON`: itemLink: cstring, rollQuantity: number, rollType: number, roll: number, upgraded: bool
- `LOOT_OPENED`: autoLoot: bool, isFromItem: bool
- `LOOT_READY`: autoloot: bool
- `LOOT_ROLLS_COMPLETE`: lootHandle: number
- `LOOT_SLOT_CHANGED`: lootSlot: luaIndex
- `LOOT_SLOT_CLEARED`: lootSlot: luaIndex
- `MAIN_SPEC_NEED_ROLL`: rollID: number, roll: number, isWinning: bool
- `OPEN_MASTER_LOOT_LIST`
- `PET_BATTLE_LOOT_RECEIVED`: typeIdentifier: cstring, itemLink: cstring, quantity: number
- `PLAYER_LOOT_SPEC_UPDATED`
- `QUEST_CURRENCY_LOOT_RECEIVED`: questID: number, currencyId: number, quantity: number
- `QUEST_LOOT_RECEIVED`: questID: number, itemLink: cstring, quantity: number
- `SHOW_LOOT_TOAST`: typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, toastMethod: number, lessAwesome: bool, upgraded: bool, corrupted: bool
- `SHOW_LOOT_TOAST_LEGENDARY_LOOTED`: itemLink: cstring
- `SHOW_LOOT_TOAST_UPGRADE`: itemLink: cstring, quantity: number, specID: number, sex: number, baseQuality: number, personalLootToast: bool, lessAwesome: bool
- `SHOW_PVP_FACTION_LOOT_TOAST`: typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, lessAwesome: bool
- `SHOW_RATED_PVP_REWARD_TOAST`: typeIdentifier: cstring, itemLink: cstring, quantity: number, specID: number, sex: number, personalLootToast: bool, lessAwesome: bool
- `START_LOOT_ROLL`: rollID: number, rollTime: number, lootHandle: number?
- `TRIAL_CAP_REACHED_MONEY`
- `UPDATE_MASTER_LOOT_LIST`

## LootHistory

See [LootHistory](systems/LootHistory.md).

- `LOOT_HISTORY_CLEAR_HISTORY`
- `LOOT_HISTORY_GO_TO_ENCOUNTER`: encounterID: number
- `LOOT_HISTORY_ONE_HUNDRED_ROLL`: encounterID: number, lootListKey: number
- `LOOT_HISTORY_UPDATE_DROP`: encounterID: number, lootListKey: number
- `LOOT_HISTORY_UPDATE_ENCOUNTER`: encounterID: number

## LootJournal

See [LootJournal](systems/LootJournal.md).

- `LOOT_JOURNAL_ITEM_UPDATE`

## LoreText

See [LoreText](systems/LoreText.md).

- `LORE_TEXT_UPDATED_CAMPAIGN`: campaignID: number, textEntries: LoreTextEntry[]

## LossOfControl

See [LossOfControl](systems/LossOfControl.md).

- `LOSS_OF_CONTROL_ADDED`: unitTarget: UnitTokenVariant, effectIndex: luaIndex
- `LOSS_OF_CONTROL_COMMENTATOR_ADDED`: victim: WOWGUID, effectIndex: luaIndex
- `LOSS_OF_CONTROL_COMMENTATOR_UPDATE`: victim: WOWGUID
- `LOSS_OF_CONTROL_UPDATE`: unitTarget: UnitTokenVariant
- `PLAYER_CONTROL_GAINED`
- `PLAYER_CONTROL_LOST`

## MailInfo

See [MailInfo](systems/MailInfo.md).

- `CLOSE_INBOX_ITEM`: mailIndex: luaIndex
- `MAIL_CLOSED`
- `MAIL_FAILED`: itemID: number?
- `MAIL_INBOX_UPDATE`
- `MAIL_LOCK_SEND_ITEMS`: attachSlot: luaIndex, itemLink: cstring
- `MAIL_OPEN_ALL_CANCELED`
- `MAIL_SEND_INFO_UPDATE`
- `MAIL_SEND_SUCCESS`
- `MAIL_SHOW`
- `MAIL_SUCCESS`: itemID: number?
- `MAIL_UNLOCK_SEND_ITEMS`
- `SEND_MAIL_COD_CHANGED`
- `SEND_MAIL_MONEY_CHANGED`
- `UPDATE_PENDING_MAIL`

## MajorFactionsUI

See [MajorFactionsUI](systems/MajorFactionsUI.md).

- `MAJOR_FACTION_INTERACTION_ENDED`
- `MAJOR_FACTION_INTERACTION_STARTED`
- `MAJOR_FACTION_RENOWN_LEVEL_CHANGED`: majorFactionID: number, newRenownLevel: number, oldRenownLevel: number
- `MAJOR_FACTION_UNLOCKED`: majorFactionID: number

## MapExplorationInfo

See [MapExplorationInfo](systems/MapExplorationInfo.md).

- `MAP_EXPLORATION_UPDATED`

## MapUI

See [MapUI](systems/MapUI.md).

- `NEW_WMO_CHUNK`
- `PLAYER_MAP_CHANGED`: oldMapID: number, newMapID: number
- `USER_WAYPOINT_UPDATED`
- `WORLD_MAP_OPEN`: uiMapID: number?
- `ZONE_CHANGED`
- `ZONE_CHANGED_INDOORS`
- `ZONE_CHANGED_NEW_AREA`

## MerchantFrame

See [MerchantFrame](systems/MerchantFrame.md).

- `MERCHANT_CLOSED`
- `MERCHANT_FILTER_ITEM_UPDATE`: itemID: number
- `MERCHANT_SHOW`
- `MERCHANT_UPDATE`

## Minimap

See [Minimap](systems/Minimap.md).

- `MINIMAP_PING`: unitTarget: UnitTokenVariant, y: number, x: number
- `MINIMAP_UPDATE_TRACKING`
- `MINIMAP_UPDATE_ZOOM`
- `PLAYER_INSIDE_QUEST_BLOB_STATE_CHANGED`: questID: number, isInside: bool

## ModelInfo

See [ModelInfo](systems/ModelInfo.md).

- `UI_MODEL_SCENE_INFO_UPDATED`

## MountJournal

See [MountJournal](systems/MountJournal.md).

- `MOUNT_EQUIPMENT_APPLY_RESULT`: success: bool
- `MOUNT_JOURNAL_SEARCH_UPDATED`
- `MOUNT_JOURNAL_USABILITY_CHANGED`
- `NEW_MOUNT_ADDED`: mountID: number

## MythicPlusInfo

See [MythicPlusInfo](systems/MythicPlusInfo.md).

- `MYTHIC_PLUS_CURRENT_AFFIX_UPDATE`
- `MYTHIC_PLUS_NEW_WEEKLY_RECORD`: mapChallengeModeID: number, completionMilliseconds: number, level: number

## NamePlateManager

See [NamePlateManager](systems/NamePlateManager.md).

- `FORBIDDEN_NAME_PLATE_CREATED`: namePlateFrame: NamePlateFrame
- `FORBIDDEN_NAME_PLATE_UNIT_ADDED`: unitToken: UnitTokenType
- `FORBIDDEN_NAME_PLATE_UNIT_REMOVED`: unitToken: UnitTokenType
- `NAME_PLATE_CREATED`: namePlateFrame: NamePlateFrame
- `NAME_PLATE_UNIT_ADDED`: unitToken: UnitTokenType
- `NAME_PLATE_UNIT_BEHIND_CAMERA_CHANGED`: unitTarget: UnitTokenVariant, isBehindCamera: bool
- `NAME_PLATE_UNIT_REMOVED`: unitToken: UnitTokenType

## NeighborhoodInitiative

See [NeighborhoodInitiative](systems/NeighborhoodInitiative.md).

- `INITIATIVE_ACTIVITY_LOG_UPDATED`
- `INITIATIVE_COMPLETED`: initiativeTitle: string
- `INITIATIVE_TASKS_TRACKED_LIST_CHANGED`: initiativeTaskID: number, added: bool
- `INITIATIVE_TASKS_TRACKED_UPDATED`
- `INITIATIVE_TASK_COMPLETED`: taskName: string
- `NEIGHBORHOOD_INITIATIVE_UPDATED`

## PaperDollInfo

See [PaperDollInfo](systems/PaperDollInfo.md).

- `AVOIDANCE_UPDATE`
- `CHARACTER_POINTS_CHANGED`: change: number
- `CHARACTER_UPGRADE_SPELL_TIER_SET`: tierIndex: number
- `COMBAT_RATING_UPDATE`
- `DISABLE_XP_GAIN`
- `ENABLE_XP_GAIN`
- `EQUIP_BIND_CONFIRM`: slot: number, itemLocation: ItemLocation
- `INSPECT_HONOR_UPDATE`
- `INSPECT_READY`: inspecteeGUID: WOWGUID
- `LIFESTEAL_UPDATE`
- `MASTERY_UPDATE`
- `PET_STATS_UPDATE`
- `PLAYER_AVG_ITEM_LEVEL_UPDATE`
- `PLAYER_EQUIPMENT_CHANGED`: equipmentSlot: number, hasCurrent: bool
- `PROFESSION_EQUIPMENT_CHANGED`: skillLineID: number, isTool: bool
- `PVP_POWER_UPDATE`
- `SPEED_UPDATE`
- `SPELL_POWER_CHANGED`
- `STURDINESS_UPDATE`
- `UPDATE_FACTION`
- `UPDATE_INVENTORY_ALERTS`
- `UPDATE_INVENTORY_DURABILITY`
- `WEAPON_SLOT_CHANGED`

## PartyInfo

See [PartyInfo](systems/PartyInfo.md).

- `BNET_REQUEST_INVITE_CONFIRMATION`: gameAccountID: number, questSessionActive: bool, tank: bool, healer: bool, dps: bool
- `CONVERT_TO_RAID_CONFIRMATION`
- `ENTERED_DIFFERENT_INSTANCE_FROM_PARTY`
- `GROUP_FORMED`: category: number, partyGUID: WOWGUID
- `GROUP_INVITE_CONFIRMATION`
- `GROUP_JOINED`: category: number, partyGUID: WOWGUID
- `GROUP_LEFT`: category: number, partyGUID: WOWGUID
- `GROUP_ROSTER_UPDATE`
- `INSTANCE_ABANDON_VOTE_FINISHED`: votePassed: bool
- `INSTANCE_ABANDON_VOTE_STARTED`
- `INSTANCE_ABANDON_VOTE_UPDATED`
- `INSTANCE_BOOT_START`
- `INSTANCE_BOOT_STOP`
- `INSTANCE_GROUP_SIZE_CHANGED`
- `INVITE_TO_PARTY_CONFIRMATION`: targetName: cstring, willConvertToRaid: bool, questSessionActive: bool
- `INVITE_TRAVEL_PASS_CONFIRMATION`: targetName: cstring, targetGUID: WOWGUID, willConvertToRaid: bool, questSessionActive: bool
- `LEAVE_PARTY_CONFIRMATION`: reason: LeavePartyConfirmReason
- `PARTY_INVITE_CANCEL`
- `PARTY_INVITE_REQUEST`: name: cstring, isTank: bool, isHealer: bool, isDamage: bool, isNativeRealm: bool, allowMultipleRoles: bool, inviterGUID: WOWGUID, questSessionActive: bool
- `PARTY_LEADER_CHANGED`
- `PARTY_LFG_RESTRICTED`
- `PARTY_LOOT_METHOD_CHANGED`
- `PARTY_MEMBER_DISABLE`: unitTarget: UnitTokenVariant
- `PARTY_MEMBER_ENABLE`: unitTarget: UnitTokenVariant
- `PLAYER_DIFFICULTY_CHANGED`
- `PLAYER_ROLES_ASSIGNED`
- `RAID_ROSTER_UPDATE`
- `READY_CHECK`: initiatorName: cstring, readyCheckTimeLeft: time_t
- `READY_CHECK_CONFIRM`: unitTarget: UnitTokenVariant, isReady: bool
- `READY_CHECK_FINISHED`: preempted: bool
- `REQUEST_INVITE_CONFIRMATION`: targetName: cstring, partyLevelLink: number, questSessionActive: bool, tank: bool?, healer: bool?, dps: bool?
- `VOTE_KICK_REASON_NEEDED`: name: cstring, resultGUID: WOWGUID

## PartyInfoSystemStatus

See [PartyInfoSystemStatus](systems/PartyInfoSystemStatus.md).

- `SOCIAL_UI_RAID_LIST_SYSTEM_STATUS_UPDATED`

## PartyPose

See [PartyPose](systems/PartyPose.md).

- `SHOW_PARTY_POSE_UI`: mapID: number, won: bool

## PerksActivities

See [PerksActivities](systems/PerksActivities.md).

- `PERKS_ACTIVITIES_TRACKED_LIST_CHANGED`: perksActivityID: number, added: bool
- `PERKS_ACTIVITIES_TRACKED_UPDATED`
- `PERKS_ACTIVITIES_UPDATED`
- `PERKS_ACTIVITY_COMPLETED`: perksActivityID: number

## PerksProgram

See [PerksProgram](systems/PerksProgram.md).

- `CHEST_REWARDS_UPDATED_FROM_SERVER`
- `PERKS_PROGRAM_ADD_PENDING_SHOP_ITEM`: vendorItemID: number
- `PERKS_PROGRAM_CLOSE`
- `PERKS_PROGRAM_CURRENCY_AWARDED`: value: number
- `PERKS_PROGRAM_CURRENCY_REFRESH`: oldValue: number, newValue: number
- `PERKS_PROGRAM_DATA_REFRESH`
- `PERKS_PROGRAM_DATA_SPECIFIC_ITEM_REFRESH`: vendorItemID: number
- `PERKS_PROGRAM_DISABLED`
- `PERKS_PROGRAM_OPEN`
- `PERKS_PROGRAM_PURCHASE_CART_SUCCESS`: vendorItemIDs: number[]
- `PERKS_PROGRAM_PURCHASE_SUCCESS`: vendorItemID: number
- `PERKS_PROGRAM_REFUND_SUCCESS`: vendorItemID: number
- `PERKS_PROGRAM_REMOVE_PENDING_SHOP_ITEM`: vendorItemID: number
- `PERKS_PROGRAM_RESULT_ERROR`
- `PERKS_PROGRAM_SET_FROZEN_ITEM`: vendorItemID: number

## PetInfo

See [PetInfo](systems/PetInfo.md).

- `PET_ATTACK_START`
- `PET_ATTACK_STOP`
- `PET_BAR_HIDEGRID`
- `PET_BAR_SHOWGRID`
- `PET_BAR_UPDATE_COOLDOWN`
- `PET_DISMISS_START`: delay: number
- `PET_FORCE_NAME_DECLENSION`: name: cstring, petNumber: number?, declinedName1: cstring?, declinedName2: cstring?, declinedName3: cstring?, declinedName4: cstring?, declinedName5: cstring?
- `PET_UI_CLOSE`
- `RAISED_AS_GHOUL`
- `UPDATE_POSSESS_BAR`
- `UPDATE_VEHICLE_ACTIONBAR`

## PetJournalInfo

See [PetJournalInfo](systems/PetJournalInfo.md).

- `BATTLEPET_FORCE_NAME_DECLENSION`: name: cstring, battlePetGUID: WOWGUID
- `COMPANION_LEARNED`
- `COMPANION_UNLEARNED`
- `COMPANION_UPDATE`: companionType: cstring?
- `NEW_PET_ADDED`: battlePetGUID: WOWGUID
- `PET_JOURNAL_AUTO_SLOTTED_PET`: slotIndex: number, battlePetGUID: WOWGUID
- `PET_JOURNAL_CAGE_FAILED`
- `PET_JOURNAL_LIST_UPDATE`
- `PET_JOURNAL_NEW_BATTLE_SLOT`
- `PET_JOURNAL_PETS_HEALED`
- `PET_JOURNAL_PET_DELETED`: battlePetGUID: WOWGUID
- `PET_JOURNAL_PET_RESTORED`: battlePetGUID: WOWGUID
- `PET_JOURNAL_PET_REVOKED`: battlePetGUID: WOWGUID
- `PET_JOURNAL_TRAP_LEVEL_SET`: trapLevel: number
- `UPDATE_SUMMONPETS_ACTION`

## PhotoSharingUI

See [PhotoSharingUI](systems/PhotoSharingUI.md).

- `PHOTO_SHARING_AUTHORIZATION_NEEDED`
- `PHOTO_SHARING_AUTHORIZATION_UPDATED`: showNotification: bool
- `PHOTO_SHARING_PHOTO_UPLOAD_STATUS`: uploadStatus: PhotoSharingUploadStatus
- `PHOTO_SHARING_SCREENSHOT_READY`
- `PHOTO_SHARING_THIRD_PARTY_AUTHORIZATION_NEEDED`: authUrl: string

## PingManager

See [PingManager](systems/PingManager.md).

- `PING_SYSTEM_ERROR`: error: cstring

## PingManagerSecure

See [PingManagerSecure](systems/PingManagerSecure.md).

- `UNIT_PING_PIN_ADDED`: guid: WOWGUID, uiTextureKit: textureKit
- `UNIT_PING_PIN_REMOVED`: guid: WOWGUID

## PlayerChoice

See [PlayerChoice](systems/PlayerChoice.md).

- `PLAYER_CHOICE_CLOSE`
- `PLAYER_CHOICE_UPDATE`

## PlayerInteractionManager

See [PlayerInteractionManager](systems/PlayerInteractionManager.md).

- `PLAYER_INTERACTION_MANAGER_FRAME_HIDE`: type: PlayerInteractionType
- `PLAYER_INTERACTION_MANAGER_FRAME_SHOW`: type: PlayerInteractionType

## PlayerMentorship

See [PlayerMentorship](systems/PlayerMentorship.md).

- `MENTORSHIP_STATUS_CHANGED`
- `NEWCOMER_GRADUATION`

## PlayerScript

See [PlayerScript](systems/PlayerScript.md).

- `PLAYER_IN_COMBAT_CHANGED`: inCombat: bool
- `PLAYER_TARGET_DIED`

## ProfessionSpecUI

See [ProfessionSpecUI](systems/ProfessionSpecUI.md).

- `SKILL_LINE_SPECS_RANKS_CHANGED`
- `SKILL_LINE_SPECS_UNLOCKED`: skillLineID: number, tradeSkillID: number

## PvpInfo

See [PvpInfo](systems/PvpInfo.md).

- `ARENA_OPPONENT_UPDATE`: unitToken: cstring, updateReason: cstring
- `ARENA_PREP_OPPONENT_SPECIALIZATIONS`
- `ARENA_SEASON_WORLD_STATE`
- `BATTLEFIELDS_CLOSED`
- `BATTLEFIELDS_SHOW`: isArena: bool?, battleMasterListID: number?
- `BATTLEFIELD_AUTO_QUEUE`
- `BATTLEFIELD_AUTO_QUEUE_EJECT`
- `BATTLEFIELD_QUEUE_TIMEOUT`
- `BATTLEGROUND_OBJECTIVES_UPDATE`
- `BATTLEGROUND_POINTS_UPDATE`
- `GDF_SIM_COMPLETE`
- `HONOR_LEVEL_UPDATE`: isHigherLevel: bool
- `NOTIFY_PVP_AFK_RESULT`: offender: cstring, numBlackMarksOnOffender: number, numPlayersIHaveReported: number
- `PLAYER_ENTERING_BATTLEGROUND`
- `PLAYER_JOINED_PVP_MATCH`
- `PLAYER_PVP_FLAG_CHANGED`: isPvpFlagged: bool
- `POST_MATCH_CURRENCY_REWARD_UPDATE`: reward: PVPPostMatchCurrencyReward
- `POST_MATCH_ITEM_REWARD_UPDATE`
- `PVPQUEUE_ANYWHERE_SHOW`
- `PVPQUEUE_ANYWHERE_UPDATE_AVAILABLE`
- `PVP_BRAWL_INFO_UPDATED`
- `PVP_MATCH_ACTIVE`
- `PVP_MATCH_COMPLETE`: winner: number, duration: time_t
- `PVP_MATCH_INACTIVE`
- `PVP_MATCH_STATE_CHANGED`
- `PVP_RATED_STATS_UPDATE`
- `PVP_REWARDS_UPDATE`
- `PVP_ROLE_POPUP_HIDE`: readyCheckInfo: PvpReadyCheckInfo?
- `PVP_ROLE_POPUP_SHOW`: readyCheckInfo: PvpReadyCheckInfo
- `PVP_ROLE_UPDATE`
- `PVP_SPECIAL_EVENT_INFO_UPDATED`
- `PVP_TYPES_ENABLED`: wargameBattlegrounds: bool, ratedBattlegrounds: bool, ratedArenas: bool, ratedSoloShuffle: bool, ratedBGBlitz: bool
- `PVP_VEHICLE_INFO_UPDATED`
- `PVP_WORLDSTATE_UPDATE`
- `TRAINING_GROUNDS_ENABLED_STATUS_UPDATED`
- `UPDATE_ACTIVE_BATTLEFIELD`
- `UPDATE_BATTLEFIELD_SCORE`
- `UPDATE_BATTLEFIELD_STATUS`: battleFieldIndex: number
- `WARGAME_INVITE_SENT`
- `WARGAME_REQUESTED`: opposingPartyMemberName: cstring, battlegroundName: cstring, timeoutSeconds: time_t, tournamentRules: bool
- `WARGAME_REQUEST_RESPONSE`: responderGUID: WOWGUID, responderName: cstring?, accepted: bool
- `WAR_MODE_STATUS_UPDATE`: warModeEnabled: bool
- `WORLD_PVP_QUEUE`

## QuestLog

See [QuestLog](systems/QuestLog.md).

- `QUESTLINE_UPDATE`: requestRequired: bool
- `QUEST_ACCEPTED`: questId: number
- `QUEST_AUTOCOMPLETE`: questId: number
- `QUEST_COMPLETE`
- `QUEST_DATA_LOAD_RESULT`: questID: number, success: bool
- `QUEST_DETAIL`: questStartItemID: number?
- `QUEST_LOG_CRITERIA_UPDATE`: questID: number, specificTreeID: number, description: cstring, numFulfilled: number, numRequired: number
- `QUEST_LOG_UPDATE`
- `QUEST_POI_UPDATE`
- `QUEST_REMOVED`: questID: number, wasReplayQuest: bool
- `QUEST_TURNED_IN`: questID: number, xpReward: number, moneyReward: number
- `QUEST_WATCH_LIST_CHANGED`: questID: number?, added: bool?
- `QUEST_WATCH_UPDATE`: questID: number
- `TASK_PROGRESS_UPDATE`
- `TREASURE_PICKER_CACHE_FLUSH`
- `WAYPOINT_UPDATE`
- `WORLD_QUEST_COMPLETED_BY_SPELL`: questID: number

## QuestOffer

See [QuestOffer](systems/QuestOffer.md).

- `QUEST_ACCEPT_CONFIRM`: name: cstring, questTitle: cstring, questID: number
- `QUEST_FINISHED`
- `QUEST_GREETING`
- `QUEST_ITEM_UPDATE`
- `QUEST_PROGRESS`

## QuestSession

See [QuestSession](systems/QuestSession.md).

- `QUEST_SESSION_CREATED`
- `QUEST_SESSION_DESTROYED`
- `QUEST_SESSION_ENABLED_STATE_CHANGED`: enabled: bool
- `QUEST_SESSION_JOINED`
- `QUEST_SESSION_LEFT`
- `QUEST_SESSION_MEMBER_CONFIRM`
- `QUEST_SESSION_MEMBER_START_RESPONSE`: guid: WOWGUID, response: bool
- `QUEST_SESSION_NOTIFICATION`: result: QuestSessionResult, guid: WOWGUID

## RecentAllies

See [RecentAllies](systems/RecentAllies.md).

- `LET_RECENT_ALLIES_SEE_LOCATION_SETTING_UPDATED`
- `RECENT_ALLIES_CACHE_UPDATE`
- `RECENT_ALLIES_DATA_READY`
- `RECENT_ALLIES_SYSTEM_STATUS_UPDATED`
- `RECENT_ALLY_DATA_UPDATED`: characterGUID: WOWGUID

## RecruitAFriend

See [RecruitAFriend](systems/RecruitAFriend.md).

- `RAF_INFO_UPDATED`: info: RafInfo
- `RAF_RECRUITING_ENABLED_STATUS`: enabled: bool
- `RAF_REWARD_CLAIM_FAILED`
- `RAF_SYSTEM_ENABLED_STATUS`: enabled: bool
- `RAF_SYSTEM_INFO_UPDATED`: systemInfo: RafSystemInfo

## RemixArtifactUI

See [RemixArtifactUI](systems/RemixArtifactUI.md).

- `REMIX_ARTIFACT_ITEM_SPECS_LOADED`: success: bool
- `REMIX_ARTIFACT_UPDATE`

## ReportSystem

See [ReportSystem](systems/ReportSystem.md).

- `REPORT_PLAYER_RESULT`: result: SendReportResult, reportType: ReportType
- `REPORT_SCREENSHOT_READY`

## ReputationInfo

See [ReputationInfo](systems/ReputationInfo.md).

- `FACTION_STANDING_CHANGED`: factionID: number, updatedStanding: number

## ResearchInfo

See [ResearchInfo](systems/ResearchInfo.md).

- `ARCHAEOLOGY_CLOSED`
- `ARCHAEOLOGY_FIND_COMPLETE`: numFindsCompleted: number, totalFinds: number, researchBranchID: number
- `ARCHAEOLOGY_SURVEY_CAST`: numFindsCompleted: number, totalFinds: number, researchBranchID: number, successfulFind: number
- `ARCHAEOLOGY_TOGGLE`
- `ARTIFACT_DIGSITE_COMPLETE`: researchBranchID: number
- `RESEARCH_ARTIFACT_COMPLETE`: name: cstring
- `RESEARCH_ARTIFACT_DIG_SITE_UPDATED`
- `RESEARCH_ARTIFACT_UPDATE`

## RestrictedActions

See [RestrictedActions](systems/RestrictedActions.md).

- `ADDON_ACTION_BLOCKED`: isTainted: cstring, function: cstring
- `ADDON_ACTION_FORBIDDEN`: isTainted: cstring, function: cstring
- `ADDON_RESTRICTION_STATE_CHANGED`: type: AddOnRestrictionType, state: AddOnRestrictionState
- `MACRO_ACTION_BLOCKED`: function: cstring
- `MACRO_ACTION_FORBIDDEN`: function: cstring

## ScenarioInfo

See [ScenarioInfo](systems/ScenarioInfo.md).

- `JAILERS_TOWER_LEVEL_UPDATE`: level: number, type: JailersTowerType
- `SCENARIO_BONUS_OBJECTIVE_COMPLETE`: bonusObjectiveID: number
- `SCENARIO_BONUS_VISIBILITY_UPDATE`
- `SCENARIO_COMPLETED`: questID: number?, xp: number?, money: number?
- `SCENARIO_CRITERIA_SHOW_STATE_UPDATE`: show: bool
- `SCENARIO_CRITERIA_UPDATE`: criteriaID: number
- `SCENARIO_POI_UPDATE`
- `SCENARIO_SPELL_UPDATE`
- `SCENARIO_UPDATE`: newStep: bool?

## ScrappingMachineUI

See [ScrappingMachineUI](systems/ScrappingMachineUI.md).

- `SCRAPPING_MACHINE_ITEM_ADDED`: index: number
- `SCRAPPING_MACHINE_ITEM_REMOVED`: index: number
- `SCRAPPING_MACHINE_PENDING_ITEM_CHANGED`
- `SCRAPPING_MACHINE_SCRAPPING_FINISHED`

## ScriptedAnimations

See [ScriptedAnimations](systems/ScriptedAnimations.md).

- `SCRIPTED_ANIMATIONS_UPDATE`

## ScriptWarnings

See [ScriptWarnings](systems/ScriptWarnings.md).

- `LUA_WARNING`: warningText: cstring

## SecureTransfer

See [SecureTransfer](systems/SecureTransfer.md).

- `SECURE_TRANSFER_CANCEL`
- `SECURE_TRANSFER_CONFIRM_HOUSING_PURCHASE`
- `SECURE_TRANSFER_CONFIRM_SEND_MAIL`
- `SECURE_TRANSFER_CONFIRM_TAKE_MAIL_MONEY`
- `SECURE_TRANSFER_CONFIRM_TRADE_ACCEPT`
- `SECURE_TRANSFER_HOUSING_CURRENCY_PURCHASE_CONFIRMATION`

## SettingsUtil

See [SettingsUtil](systems/SettingsUtil.md).

- `SETTINGS_LOADED`
- `SETTINGS_PANEL_OPEN`: openToCategoryID: number?, scrollToElementName: stringView?

## SharedTraits

See [SharedTraits](systems/SharedTraits.md).

- `CONFIG_COMMIT_FAILED`: configID: number
- `TRAIT_COND_INFO_CHANGED`: condID: number
- `TRAIT_CONFIG_CREATED`: configInfo: TraitConfigInfo
- `TRAIT_CONFIG_DELETED`: configID: number
- `TRAIT_CONFIG_LIST_UPDATED`
- `TRAIT_CONFIG_UPDATED`: configID: number
- `TRAIT_NODE_CHANGED`: nodeID: number
- `TRAIT_NODE_CHANGED_PARTIAL`: ID: number, info: TraitNodeInfoPartial
- `TRAIT_NODE_ENTRY_UPDATED`: nodeEntryID: number
- `TRAIT_SUB_TREE_CHANGED`: subTreeID: number
- `TRAIT_SYSTEM_INTERACTION_STARTED`: treeID: number
- `TRAIT_SYSTEM_NPC_CLOSED`
- `TRAIT_TREE_CHANGED`: treeID: number
- `TRAIT_TREE_CURRENCY_INFO_UPDATED`: treeID: number
- `TRY_PURCHASE_TO_NODE_PARTIAL_SUCCESS`: nodeFinishedOn: number

## SkillInfo

See [SkillInfo](systems/SkillInfo.md).

- `SKILL_LINES_CHANGED`

## SocialQueue

See [SocialQueue](systems/SocialQueue.md).

- `SOCIAL_QUEUE_CONFIG_UPDATED`
- `SOCIAL_QUEUE_UPDATE`: groupGUID: WOWGUID, numAddedItems: number?

## SocialQueueSystemStatus

See [SocialQueueSystemStatus](systems/SocialQueueSystemStatus.md).

- `SOCIAL_UI_SOCIAL_QUEUE_SYSTEM_STATUS_UPDATED`

## SocialRestrictions

See [SocialRestrictions](systems/SocialRestrictions.md).

- `ALERT_AGE_VERIFICATION_RESTRICTED`
- `ALERT_REGIONAL_CHAT_DISABLED`
- `CHAT_DISABLED_CHANGED`: disabled: bool
- `CHAT_DISABLED_CHANGE_FAILED`: disabled: bool

## SocialUI

See [SocialUI](systems/SocialUI.md).

- `SOCIAL_UI_SYSTEM_STATUS_UPDATED`

## Soulbinds

See [Soulbinds](systems/Soulbinds.md).

- `SOULBIND_ACTIVATED`: soulbindID: number
- `SOULBIND_CONDUIT_COLLECTION_CLEARED`
- `SOULBIND_CONDUIT_COLLECTION_REMOVED`: conduitID: number
- `SOULBIND_CONDUIT_COLLECTION_UPDATED`: collectionData: ConduitCollectionData
- `SOULBIND_CONDUIT_INSTALLED`: nodeID: number, data: SoulbindConduitData
- `SOULBIND_CONDUIT_UNINSTALLED`: nodeID: number, data: SoulbindConduitData
- `SOULBIND_FORGE_INTERACTION_ENDED`
- `SOULBIND_FORGE_INTERACTION_STARTED`
- `SOULBIND_NODE_LEARNED`: nodeID: number
- `SOULBIND_NODE_UNLEARNED`: nodeID: number
- `SOULBIND_NODE_UPDATED`: nodeID: number
- `SOULBIND_PATH_CHANGED`
- `SOULBIND_PENDING_CONDUIT_CHANGED`: nodeID: number, conduitID: number

## Sound

See [Sound](systems/Sound.md).

- `SOUNDKIT_FINISHED`: soundHandle: number
- `SOUND_DEVICE_UPDATE`

## SpecializationInfo

See [SpecializationInfo](systems/SpecializationInfo.md).

- `ACTIVE_TALENT_GROUP_CHANGED`: curr: number, prev: number
- `CONFIRM_PET_UNLEARN`: cost: number
- `CONFIRM_TALENT_WIPE`: cost: number, respecType: number
- `PET_SPECIALIZATION_CHANGED`
- `PLAYER_LEARN_PVP_TALENT_FAILED`
- `PLAYER_LEARN_TALENT_FAILED`
- `PLAYER_PVP_TALENT_UPDATE`
- `PLAYER_TALENT_UPDATE`
- `SPEC_INVOLUNTARILY_CHANGED`: isPet: bool
- `TALENTS_INVOLUNTARILY_RESET`: isPetTalents: bool

## Spell

See [Spell](systems/Spell.md).

- `ENCHANT_SPELL_COMPLETED`: successful: bool, enchantedItem: ItemLocation?
- `ENCHANT_SPELL_SELECTED`
- `SPELL_DATA_LOAD_RESULT`: spellID: number, success: bool
- `SPELL_RANGE_CHECK_UPDATE`: spellIdentifier: SpellIdentifier, isInRange: bool, checksRange: bool
- `SPELL_TEXT_UPDATE`: spellID: number
- `UPDATE_SPELL_TARGET_ITEM_CONTEXT`

## SpellActivationOverlay

See [SpellActivationOverlay](systems/SpellActivationOverlay.md).

- `SPELL_ACTIVATION_OVERLAY_GLOW_HIDE`: spellID: number
- `SPELL_ACTIVATION_OVERLAY_GLOW_SHOW`: spellID: number
- `SPELL_ACTIVATION_OVERLAY_HIDE`: spellID: number?
- `SPELL_ACTIVATION_OVERLAY_SHOW`: spellID: number, overlayFileDataID: number, locationType: ScreenLocationType, scale: number, r: number, g: number, b: number

## SpellBook

See [SpellBook](systems/SpellBook.md).

- `CURRENT_SPELL_CAST_CHANGED`: cancelledCast: bool
- `LEARNED_SPELL_IN_SKILL_LINE`: spellID: number, skillLineIndex: luaIndex, isGuildPerkSpell: bool
- `MAX_SPELL_START_RECOVERY_OFFSET_CHANGED`: clampedNewQueueWindowMs: number
- `PLAYER_TOTEM_UPDATE`: totemSlot: luaIndex
- `SPELLS_CHANGED`
- `SPELL_FLYOUT_UPDATE`: flyoutID: number?, spellID: number?, isLearned: bool?
- `SPELL_PUSHED_TO_ACTIONBAR`: spellID: number, slot: luaIndex, page: luaIndex
- `SPELL_PUSHED_TO_FLYOUT_ON_ACTIONBAR`: spellID: number, flyoutSlot: luaIndex, flyoutPage: luaIndex
- `SPELL_UPDATE_CHARGES`
- `SPELL_UPDATE_COOLDOWN`: spellID: number?, baseSpellID: number?, category: number?, startRecoveryCategory: number?, itemID: number?
- `SPELL_UPDATE_ICON`: spellID: number?
- `SPELL_UPDATE_USABLE`
- `SPELL_UPDATE_USES`: spellID: number, baseSpellID: number?
- `START_AUTOREPEAT_SPELL`
- `STOP_AUTOREPEAT_SPELL`
- `UPDATE_SHAPESHIFT_COOLDOWN`
- `UPDATE_SHAPESHIFT_FORM`
- `UPDATE_SHAPESHIFT_FORMS`
- `UPDATE_SHAPESHIFT_USABLE`

## SpellDiminishUI

See [SpellDiminishUI](systems/SpellDiminishUI.md).

- `UNIT_SPELL_DIMINISH_CATEGORY_STATE_UPDATED`: unitTarget: UnitTokenVariant, trackerInfo: SpellDiminishTrackerInfo

## SplashScreen

See [SplashScreen](systems/SplashScreen.md).

- `OPEN_SPLASH_SCREEN`: info: SplashScreenInfo?

## StableInfo

See [StableInfo](systems/StableInfo.md).

- `PET_INFO_UPDATE`
- `PET_STABLE_CLOSED`
- `PET_STABLE_FAVORITES_UPDATED`
- `PET_STABLE_SHOW`
- `PET_STABLE_UPDATE`

## SuperTrackManager

See [SuperTrackManager](systems/SuperTrackManager.md).

- `SUPER_TRACKING_CHANGED`
- `SUPER_TRACKING_PATH_UPDATED`

## SwingTimer

See [SwingTimer](systems/SwingTimer.md).

- `PLAYER_SWING`: swingDuration: number, swingType: PlayerSwingType
- `PLAYER_SWING_RANGE_UPDATE`: swingType: PlayerSwingType, isInRange: bool, checksRange: bool

## SystemInfo

See [SystemInfo](systems/SystemInfo.md).

- `CAPTUREFRAMES_FAILED`
- `CAPTUREFRAMES_SUCCEEDED`
- `DISABLE_TAXI_BENCHMARK`
- `ENABLE_TAXI_BENCHMARK`
- `FIRST_FRAME_RENDERED`
- `GENERIC_ERROR`: errorMessage: cstring
- `GLOBAL_MOUSE_DOWN`: button: cstring
- `GLOBAL_MOUSE_UP`: button: cstring
- `GLOBAL_REGION_MOUSE_DOWN`: region: ScriptRegion, button: cstring
- `GLOBAL_REGION_MOUSE_UP`: region: ScriptRegion, button: cstring
- `INITIAL_HOTFIXES_APPLIED`
- `LOC_RESULT`: result: cstring
- `LOGOUT_CANCEL`
- `PLAYER_CAMPING`
- `PLAYER_ENTERING_WORLD`: isInitialLogin: bool, isReloadingUi: bool
- `PLAYER_LEAVING_WORLD`
- `PLAYER_LOGIN`
- `PLAYER_LOGOUT`
- `PLAYER_QUITING`
- `SEARCH_DB_LOADED`
- `SHARD_TRANSFER`
- `SHARD_TRANSFER_CANCELLED`
- `SHARD_TRANSFER_IMMINENT`
- `STREAMING_ICON`: streamingStatus: number
- `SYSMSG`: string: cstring, r: number, g: number, b: number
- `TIME_PLAYED_MSG`: totalTimePlayed: number, timePlayedThisLevel: number
- `UI_ERROR_MESSAGE`: errorType: luaIndex, message: string
- `UI_ERROR_POPUP`: errorType: luaIndex, message: string
- `UI_INFO_MESSAGE`: errorType: luaIndex, message: string
- `VARIABLES_LOADED`
- `WOW_MOUSE_NOT_FOUND`

## TalkingHead

See [TalkingHead](systems/TalkingHead.md).

- `TALKINGHEAD_CLOSE`
- `TALKINGHEAD_REQUESTED`

## TaxiMap

See [TaxiMap](systems/TaxiMap.md).

- `TAXIMAP_CLOSED`
- `TAXIMAP_OPENED`: system: number
- `TAXI_NODE_STATUS_CHANGED`

## TextureUtils

See [TextureUtils](systems/TextureUtils.md).

- `URL_TEXTURE_REQUEST_RESULT`: texture: SimpleTexture, result: UrlTextureResult

## TimerunningUI

See [TimerunningUI](systems/TimerunningUI.md).

- `REMIX_END_OF_EVENT`

## TooltipComparison

See [TooltipComparison](systems/TooltipComparison.md).

- `TOOLTIP_SHOW_ITEM_COMPARISON`: comparisonItem: TooltipComparisonItem, tooltip: Tooltip, anchorFrame: SimpleFrame?

## TooltipInfo

See [TooltipInfo](systems/TooltipInfo.md).

- `HIDE_HYPERLINK_TOOLTIP`
- `SHOW_HYPERLINK_TOOLTIP`: hyperlink: string
- `TOOLTIP_DATA_UPDATE`: dataInstanceID: number?

## ToyBoxInfo

See [ToyBoxInfo](systems/ToyBoxInfo.md).

- `NEW_TOY_ADDED`: itemID: number
- `TOYS_UPDATED`: itemID: number?, isNew: bool?, hasFanfare: bool?

## TradeInfo

See [TradeInfo](systems/TradeInfo.md).

- `PLAYER_TRADE_CURRENCY`
- `PLAYER_TRADE_MONEY`
- `TRADE_ACCEPT_UPDATE`: playerAccepted: number, targetAccepted: number
- `TRADE_CLOSED`
- `TRADE_CURRENCY_CHANGED`
- `TRADE_MONEY_CHANGED`
- `TRADE_PLAYER_ITEM_CHANGED`: tradeSlotIndex: number
- `TRADE_POTENTIAL_BIND_ENCHANT`: canBecomeBoundForTrade: bool
- `TRADE_POTENTIAL_REMOVE_TRANSMOG`: itemLink: cstring, tradeSlotIndex: number
- `TRADE_REQUEST`: name: cstring
- `TRADE_REQUEST_CANCEL`
- `TRADE_SHOW`
- `TRADE_TARGET_ITEM_CHANGED`: tradeSlotIndex: number
- `TRADE_UPDATE`
- `TRADE_UPDATE_WARNINGS`

## TradeSkillUI

See [TradeSkillUI](systems/TradeSkillUI.md).

- `CRAFTING_DETAILS_UPDATE`
- `NEW_RECIPE_LEARNED`: recipeID: number, recipeLevel: luaIndex?, baseRecipeID: number?
- `OBLITERUM_FORGE_PENDING_ITEM_CHANGED`
- `OPEN_RECIPE_RESPONSE`: recipeID: number, skillLineID: number, expansionSkillLineID: number
- `PROFESSION_RESPEC_CONFIRMATION`: skillName: cstring
- `TRACKED_RECIPE_UPDATE`: recipeID: number, tracked: bool
- `TRADE_SKILL_CLOSE`
- `TRADE_SKILL_CRAFTING_REAGENT_BONUS_TEXT_UPDATED`: itemID: number
- `TRADE_SKILL_CRAFT_BEGIN`: recipeSpellID: number
- `TRADE_SKILL_CURRENCY_REWARD_RESULT`: data: CraftingCurrencyResultData
- `TRADE_SKILL_DATA_SOURCE_CHANGED`
- `TRADE_SKILL_DATA_SOURCE_CHANGING`
- `TRADE_SKILL_DETAILS_UPDATE`
- `TRADE_SKILL_FAVORITES_CHANGED`: isFavorite: bool, recipeSpellID: number
- `TRADE_SKILL_ITEM_CRAFTED_RESULT`: data: CraftingItemResultData
- `TRADE_SKILL_ITEM_UPDATE`: itemGUID: WOWGUID
- `TRADE_SKILL_LIST_UPDATE`
- `TRADE_SKILL_NAME_UPDATE`
- `TRADE_SKILL_SHOW`
- `UPDATE_TRADESKILL_CAST_STOPPED`: isScrapping: bool

## Trainer

See [Trainer](systems/Trainer.md).

- `TRAINER_CLOSED`
- `TRAINER_DESCRIPTION_UPDATE`
- `TRAINER_SERVICE_INFO_NAME_UPDATE`
- `TRAINER_SHOW`
- `TRAINER_UPDATE`

## TransmogOutfitInfo

See [TransmogOutfitInfo](systems/TransmogOutfitInfo.md).

- `TRANSMOG_DISPLAYED_OUTFIT_CHANGED`
- `TRANSMOG_OUTFITS_CHANGED`: newOutfitID: number?
- `VIEWED_TRANSMOG_OUTFIT_CHANGED`
- `VIEWED_TRANSMOG_OUTFIT_SECONDARY_SLOTS_CHANGED`
- `VIEWED_TRANSMOG_OUTFIT_SITUATIONS_CHANGED`
- `VIEWED_TRANSMOG_OUTFIT_SLOT_OPTION_CHANGED`: slot: TransmogOutfitSlot, option: TransmogOutfitSlotOption
- `VIEWED_TRANSMOG_OUTFIT_SLOT_REFRESH`
- `VIEWED_TRANSMOG_OUTFIT_SLOT_SAVE_SUCCESS`: slot: TransmogOutfitSlot, type: TransmogType, option: TransmogOutfitSlotOption

## Transmogrify

See [Transmogrify](systems/Transmogrify.md).

- `TRANSMOGRIFY_CLOSE`
- `TRANSMOGRIFY_ITEM_UPDATE`
- `TRANSMOGRIFY_OPEN`
- `TRANSMOGRIFY_SUCCESS`: transmogLocation: TransmogLocation
- `TRANSMOGRIFY_UPDATE`: transmogLocation: TransmogLocation?, action: cstring?
- `TRANSMOG_COLLECTION_CAMERA_UPDATE`
- `TRANSMOG_COLLECTION_ITEM_FAVORITE_UPDATE`: itemAppearanceID: number, isFavorite: bool
- `TRANSMOG_COLLECTION_ITEM_UPDATE`
- `TRANSMOG_COLLECTION_SOURCE_ADDED`: itemModifiedAppearanceID: number
- `TRANSMOG_COLLECTION_SOURCE_REMOVED`: itemModifiedAppearanceID: number
- `TRANSMOG_COLLECTION_UPDATED`: collectionIndex: luaIndex?, modID: number?, itemAppearanceID: number?, reason: cstring?
- `TRANSMOG_COSMETIC_COLLECTION_SOURCE_ADDED`: itemModifiedAppearanceID: number
- `TRANSMOG_SEARCH_UPDATED`: searchType: TransmogSearchType, collectionType: TransmogCollectionType?
- `TRANSMOG_SETS_UPDATE_FAVORITE`
- `TRANSMOG_SOURCE_COLLECTABILITY_UPDATE`: itemModifiedAppearanceID: number, collectable: bool

## Tutorial

See [Tutorial](systems/Tutorial.md).

- `LEAVING_TUTORIAL_AREA`
- `NPE_TUTORIAL_UPDATE`
- `TUTORIAL_COMBAT_EVENT`
- `TUTORIAL_HIGHLIGHT_SPELL`: spellID: number, tutorialGlobalStringTag: cstring
- `TUTORIAL_TRIGGER`: tutorialIndex: number, forceShow: bool
- `TUTORIAL_UNHIGHLIGHT_SPELL`

## UI

See [UI](systems/UI.md).

- `NOTCHED_DISPLAY_MODE_CHANGED`
- `UI_SCALE_CHANGED`

## UIActionHandlerSystem

See [UIActionHandlerSystem](systems/UIActionHandlerSystem.md).

- `HANDLE_UI_ACTION`: actionType: UIActionType

## UIEventToastManagerInfo

See [UIEventToastManagerInfo](systems/UIEventToastManagerInfo.md).

- `DISPLAY_EVENT_TOASTS`
- `DISPLAY_EVENT_TOAST_LINK`: link: string

## UIFrameManager

See [UIFrameManager](systems/UIFrameManager.md).

- `FRAME_MANAGER_UPDATE_ALL`
- `FRAME_MANAGER_UPDATE_FRAME`: type: UIFrameType, show: bool

## UIMacros

See [UIMacros](systems/UIMacros.md).

- `UPDATE_MACROS`

## UISystemVisibilityManager

See [UISystemVisibilityManager](systems/UISystemVisibilityManager.md).

- `SYSTEM_VISIBILITY_CHANGED`

## UIWidgetManager

See [UIWidgetManager](systems/UIWidgetManager.md).

- `UPDATE_ALL_UI_WIDGETS`
- `UPDATE_UI_WIDGET`: widgetInfo: UIWidgetInfo

## Unit

See [Unit](systems/Unit.md).

- `ACTIVE_PLAYER_SPECIALIZATION_CHANGED`
- `ARENA_COOLDOWNS_UPDATE`
- `ARENA_CROWD_CONTROL_SPELL_UPDATE`: unitTarget: UnitTokenVariant, spellID: number
- `AUTOFOLLOW_BEGIN`: name: cstring
- `AUTOFOLLOW_END`
- `CANCEL_SUMMON`
- `COMBO_TARGET_CHANGED`
- `CONFIRM_BINDER`: areaName: cstring
- `CONFIRM_SUMMON`: summonReason: number, skippingStartExperience: bool
- `ECLIPSE_DIRECTION_CHANGE`: direction: cstring
- `HEARTHSTONE_BOUND`
- `HONOR_XP_UPDATE`: unitTarget: UnitTokenVariant
- `INCOMING_RESURRECT_CHANGED`: unitTarget: UnitTokenVariant
- `INCOMING_SUMMON_CHANGED`: unitTarget: UnitTokenVariant
- `KNOWN_TITLES_UPDATE`: unitTarget: UnitTokenVariant
- `LOCALPLAYER_PET_RENAMED`
- `MIRROR_TIMER_PAUSE`: timerName: cstring, paused: number
- `MIRROR_TIMER_START`: timerName: cstring, value: number, maxValue: number, scale: number, paused: number, timerLabel: cstring
- `MIRROR_TIMER_STOP`: timerName: cstring
- `NEUTRAL_FACTION_SELECT_RESULT`: success: bool
- `OBJECT_ENTERED_AOI`: guid: WOWGUID
- `OBJECT_LEFT_AOI`: guid: WOWGUID
- `PARTY_KILL`: attackerGUID: WOWGUID, targetGUID: WOWGUID
- `PET_BAR_UPDATE_USABLE`
- `PET_UI_UPDATE`
- `PLAYER_CAN_GLIDE_CHANGED`: canGlide: bool
- `PLAYER_DAMAGE_DONE_MODS`: unitTarget: UnitTokenVariant
- `PLAYER_ENTER_COMBAT`
- `PLAYER_FARSIGHT_FOCUS_CHANGED`
- `PLAYER_FLAGS_CHANGED`: unitTarget: UnitTokenVariant
- `PLAYER_FOCUS_CHANGED`
- `PLAYER_IMPULSE_APPLIED`
- `PLAYER_IS_GLIDING_CHANGED`: isGliding: bool
- `PLAYER_LEAVE_COMBAT`
- `PLAYER_LEVEL_CHANGED`: oldLevel: number, newLevel: number, real: bool
- `PLAYER_LEVEL_UP`: level: number, healthDelta: number, powerDelta: number, numNewTalents: number, numNewPvpTalentSlots: number, strengthDelta: number, agilityDelta: number, staminaDelta: number, intellectDelta: number, spiritDelta: number
- `PLAYER_MAX_LEVEL_UPDATE`: unitTarget: UnitTokenVariant
- `PLAYER_MOUNT_DISPLAY_CHANGED`
- `PLAYER_PVP_KILLS_CHANGED`: unitTarget: UnitTokenVariant
- `PLAYER_PVP_RANK_CHANGED`: unitTarget: UnitTokenVariant
- `PLAYER_REGEN_DISABLED`
- `PLAYER_REGEN_ENABLED`
- `PLAYER_SOFT_ENEMY_CHANGED`
- `PLAYER_SOFT_FRIEND_CHANGED`
- `PLAYER_SOFT_INTERACT_CHANGED`: oldTarget: WOWGUID, newTarget: WOWGUID
- `PLAYER_SOFT_TARGET_INTERACTION`
- `PLAYER_SPECIALIZATION_CHANGED`: unitTarget: UnitTokenVariant
- `PLAYER_STARTED_LOOKING`
- `PLAYER_STARTED_MOVING`
- `PLAYER_STARTED_TURNING`
- `PLAYER_STOPPED_LOOKING`
- `PLAYER_STOPPED_MOVING`
- `PLAYER_STOPPED_TURNING`
- `PLAYER_TARGET_CHANGED`
- `PLAYER_TRIAL_XP_UPDATE`: unitTarget: UnitTokenVariant
- `PLAYER_UPDATE_RESTING`
- `PLAYER_XP_UPDATE`: unitTarget: UnitTokenVariant
- `PORTRAITS_UPDATED`
- `PROVING_GROUNDS_SCORE_UPDATE`: points: number
- `PVP_TIMER_UPDATE`: unitTarget: UnitTokenVariant
- `RUNE_POWER_UPDATE`: runeIndex: number, added: bool?
- `RUNE_TYPE_UPDATE`: runeIndex: number
- `SHOW_FACTION_SELECT_UI`
- `SPELL_CONFIRMATION_PROMPT`: spellID: number, effectValue: number, message: cstring, duration: number, currencyTypesID: number, currencyCost: number, currentDifficulty: number, displayItemID: number, itemContext: number, treasureContextLevel: number
- `SPELL_CONFIRMATION_TIMEOUT`: spellID: number, effectValue: number
- `UNIT_ABSORB_AMOUNT_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_AREA_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_ARENA_COOLDOWNS_UPDATE`: unitTarget: UnitTokenVariant
- `UNIT_ATTACK`: unitTarget: UnitTokenVariant
- `UNIT_ATTACK_POWER`: unitTarget: UnitTokenVariant
- `UNIT_ATTACK_SPEED`: unitTarget: UnitTokenVariant
- `UNIT_CHEAT_TOGGLE_EVENT`
- `UNIT_CLASSIFICATION_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_COMBAT`: unitTarget: UnitTokenVariant, event: cstring, flagText: cstring, amount: number, schoolMask: number
- `UNIT_CONNECTION`: unitTarget: UnitTokenVariant, isConnected: bool
- `UNIT_CTR_OPTIONS`: unitTarget: UnitTokenVariant
- `UNIT_DAMAGE`: unitTarget: UnitTokenVariant
- `UNIT_DEFENSE`: unitTarget: UnitTokenVariant
- `UNIT_DIED`: unitGUID: WOWGUID
- `UNIT_DISPLAYPOWER`: unitTarget: UnitTokenVariant
- `UNIT_DISTANCE_CHECK_UPDATE`: unitTarget: UnitTokenVariant, isInDistance: bool
- `UNIT_FACTION`: unitTarget: UnitTokenVariant
- `UNIT_FLAGS`: unitTarget: UnitTokenVariant
- `UNIT_FORM_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_HAPPINESS`: unitTarget: UnitTokenVariant
- `UNIT_HEALTH`: unitTarget: UnitTokenVariant
- `UNIT_HEAL_ABSORB_AMOUNT_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_HEAL_PREDICTION`: unitTarget: UnitTokenVariant
- `UNIT_INVENTORY_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_IN_RANGE_UPDATE`: unitTarget: UnitTokenVariant, isInRange: bool
- `UNIT_LEVEL`: unitTarget: UnitTokenVariant
- `UNIT_LOOT`: unitGUID: WOWGUID, hasLoot: bool
- `UNIT_MANA`: unitTarget: UnitTokenVariant
- `UNIT_MAXHEALTH`: unitTarget: UnitTokenVariant
- `UNIT_MAXPOWER`: unitTarget: UnitTokenVariant, powerType: cstring
- `UNIT_MAX_HEALTH_MODIFIERS_CHANGED`: unitTarget: UnitTokenVariant, percentMaxHealthAdjusted: number
- `UNIT_MODEL_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_NAME_UPDATE`: unitTarget: UnitTokenVariant
- `UNIT_OTHER_PARTY_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_PET`: unitTarget: UnitTokenVariant
- `UNIT_PET_EXPERIENCE`: unitTarget: UnitTokenVariant
- `UNIT_PET_TRAINING_POINTS`: unitTarget: UnitTokenVariant
- `UNIT_PHASE`: unitTarget: UnitTokenVariant
- `UNIT_PORTRAIT_UPDATE`: unitTarget: UnitTokenVariant
- `UNIT_POWER_BAR_HIDE`: unitTarget: UnitTokenVariant
- `UNIT_POWER_BAR_SHOW`: unitTarget: UnitTokenVariant
- `UNIT_POWER_BAR_TIMER_UPDATE`: unitTarget: UnitTokenVariant
- `UNIT_POWER_FREQUENT`: unitTarget: UnitTokenVariant, powerType: cstring
- `UNIT_POWER_POINT_CHARGE`: unitTarget: UnitTokenVariant
- `UNIT_POWER_UPDATE`: unitTarget: UnitTokenVariant, powerType: cstring
- `UNIT_QUEST_LOG_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_RANGEDDAMAGE`: unitTarget: UnitTokenVariant
- `UNIT_RANGED_ATTACK_POWER`: unitTarget: UnitTokenVariant
- `UNIT_RESISTANCES`: unitTarget: UnitTokenVariant
- `UNIT_SPELLCAST_CHANNEL_START`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_CHANNEL_STOP`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, interruptedBy: WOWGUID, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_CHANNEL_UPDATE`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_DELAYED`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_EMPOWER_START`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_EMPOWER_STOP`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, complete: bool, interruptedBy: WOWGUID, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_EMPOWER_UPDATE`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_FAILED`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_FAILED_QUIET`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_INTERRUPTED`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, interruptedBy: WOWGUID, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_INTERRUPTIBLE`: unitTarget: UnitTokenVariant
- `UNIT_SPELLCAST_NOT_INTERRUPTIBLE`: unitTarget: UnitTokenVariant
- `UNIT_SPELLCAST_RETICLE_CLEAR`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number
- `UNIT_SPELLCAST_RETICLE_TARGET`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number
- `UNIT_SPELLCAST_SENT`: unitTarget: UnitTokenVariant, target: cstring, castGUID: WOWGUID, spellID: number
- `UNIT_SPELLCAST_START`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_STOP`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELLCAST_SUCCEEDED`: unitTarget: UnitTokenVariant, castGUID: WOWGUID, spellID: number, castBarID: UnitCastBarID?
- `UNIT_SPELL_HASTE`: unitTarget: UnitTokenVariant
- `UNIT_STATS`: unitTarget: UnitTokenVariant
- `UNIT_TARGET`: unitTarget: UnitTokenVariant
- `UNIT_TARGETABLE_CHANGED`: unitTarget: UnitTokenVariant
- `UNIT_THREAT_LIST_UPDATE`: unitTarget: UnitTokenVariant
- `UNIT_THREAT_SITUATION_UPDATE`: unitTarget: UnitTokenVariant
- `UPDATE_EXHAUSTION`
- `UPDATE_MOUSEOVER_UNIT`
- `UPDATE_STEALTH`
- `VEHICLE_ANGLE_UPDATE`: normalizedPitch: number, radians: number

## UnitAuras

See [UnitAuras](systems/UnitAuras.md).

- `AURA_DATA_PROVIDER_SWITCH`: useRealDataProvider: bool
- `GROUP_BUFF_VISUAL_ALERTS_CHANGED`: visualAlerts: GroupBuffVisualAlertInfo[]
- `HIDDEN_GROUP_BUFFS_CHANGED`: spellIDs: number[]
- `UNIT_AURA`: unitTarget: UnitTokenVariant, updateInfo: UnitAuraUpdateInfo
- `UNIT_AURA_BLOCKED`: unitTarget: UnitTokenVariant, auraInstanceID: number
- `UNIT_AURA_BLOCK_LIST_CLEARED`: unitTarget: UnitTokenVariant

## UnitRole

See [UnitRole](systems/UnitRole.md).

- `ROLE_CHANGED_INFORM`: changedName: cstring, fromName: cstring, oldRole: cstring, newRole: cstring
- `ROLE_POLL_BEGIN`: fromName: cstring

## Vehicle

See [Vehicle](systems/Vehicle.md).

- `PLAYER_GAINS_VEHICLE_DATA`: unitTarget: UnitTokenVariant, vehicleUIIndicatorID: number
- `PLAYER_LOSES_VEHICLE_DATA`: unitTarget: UnitTokenVariant
- `UNIT_ENTERED_VEHICLE`: unitTarget: UnitTokenVariant, showVehicleFrame: bool, isControlSeat: bool, vehicleUIIndicatorID: number, vehicleGUID: WOWGUID, mayChooseExit: bool, hasPitch: bool
- `UNIT_ENTERING_VEHICLE`: unitTarget: UnitTokenVariant, showVehicleFrame: bool, isControlSeat: bool, vehicleUIIndicatorID: number, vehicleGUID: WOWGUID, mayChooseExit: bool, hasPitch: bool
- `UNIT_EXITED_VEHICLE`: unitTarget: UnitTokenVariant
- `UNIT_EXITING_VEHICLE`: unitTarget: UnitTokenVariant
- `VEHICLE_ANGLE_SHOW`: shouldShow: number?
- `VEHICLE_PASSENGERS_CHANGED`
- `VEHICLE_POWER_SHOW`: shouldShow: number?
- `VEHICLE_UPDATE`

## Video

See [Video](systems/Video.md).

- `ADAPTER_LIST_CHANGED`
- `DISPLAY_SIZE_CHANGED`
- `GLUE_SCREENSHOT_FAILED`
- `GLUE_SCREENSHOT_STARTED`
- `GLUE_SCREENSHOT_SUCCEEDED`
- `GX_RESTARTED`
- `SCREENSHOT_FAILED`
- `SCREENSHOT_STARTED`
- `SCREENSHOT_SUCCEEDED`

## Vignette

See [Vignette](systems/Vignette.md).

- `VIGNETTES_UPDATED`
- `VIGNETTE_MINIMAP_UPDATED`: vignetteGUID: WOWGUID, onMinimap: bool

## VoiceChat

See [VoiceChat](systems/VoiceChat.md).

- `VOICE_CHAT_ACTIVE_INPUT_DEVICE_UPDATED`
- `VOICE_CHAT_ACTIVE_OUTPUT_DEVICE_UPDATED`
- `VOICE_CHAT_ACTIVE_VOICE_PROVIDER_CHANGED`: voiceProviderID: VoiceProviderID
- `VOICE_CHAT_AUDIO_CAPTURE_ENERGY`: isSpeaking: bool, energy: number
- `VOICE_CHAT_AUDIO_CAPTURE_STARTED`
- `VOICE_CHAT_AUDIO_CAPTURE_STOPPED`
- `VOICE_CHAT_CHANNEL_ACTIVATED`: channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_DEACTIVATED`: channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_DISPLAY_NAME_CHANGED`: channelID: VoiceChatID, channelDisplayName: cstring
- `VOICE_CHAT_CHANNEL_JOINED`: status: VoiceChatStatusCode, channelID: VoiceChatID, channelType: ChatChannelType, clubId: ClubId?, streamId: ClubStreamId?
- `VOICE_CHAT_CHANNEL_MEMBER_ACTIVE_STATE_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, isActive: bool
- `VOICE_CHAT_CHANNEL_MEMBER_ADDED`: memberID: VoiceChatID, channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_MEMBER_ENERGY_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, speakingEnergy: number
- `VOICE_CHAT_CHANNEL_MEMBER_GUID_UPDATED`: memberID: VoiceChatID, channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ALL_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, isMutedForAll: bool
- `VOICE_CHAT_CHANNEL_MEMBER_MUTE_FOR_ME_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, isMutedForMe: bool
- `VOICE_CHAT_CHANNEL_MEMBER_REMOVED`: memberID: VoiceChatID, channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_MEMBER_SILENCED_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, isSilenced: bool
- `VOICE_CHAT_CHANNEL_MEMBER_SPEAKING_STATE_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, isSpeaking: bool
- `VOICE_CHAT_CHANNEL_MEMBER_STT_MESSAGE`: memberID: VoiceChatID, channelID: VoiceChatID, message: string, language: string
- `VOICE_CHAT_CHANNEL_MEMBER_VOLUME_CHANGED`: memberID: VoiceChatID, channelID: VoiceChatID, volume: number
- `VOICE_CHAT_CHANNEL_MUTE_STATE_CHANGED`: channelID: VoiceChatID, isMuted: bool
- `VOICE_CHAT_CHANNEL_PTT_CHANGED`: channelID: VoiceChatID, pushToTalkSetting: cstring
- `VOICE_CHAT_CHANNEL_REMOVED`: channelID: VoiceChatID
- `VOICE_CHAT_CHANNEL_TRANSCRIBING_CHANGED`: channelID: VoiceChatID, isTranscribing: bool
- `VOICE_CHAT_CHANNEL_TRANSMIT_CHANGED`: channelID: VoiceChatID, isTransmitting: bool
- `VOICE_CHAT_CHANNEL_VOLUME_CHANGED`: channelID: VoiceChatID, volume: number
- `VOICE_CHAT_COMMUNICATION_MODE_CHANGED`: communicationMode: CommunicationMode
- `VOICE_CHAT_CONNECTION_SUCCESS`
- `VOICE_CHAT_DEAFENED_CHANGED`: isDeafened: bool
- `VOICE_CHAT_DISCORD_SETTINGS_UPDATED`
- `VOICE_CHAT_ERROR`: platformCode: number, statusCode: VoiceChatStatusCode
- `VOICE_CHAT_INPUT_DEVICES_UPDATED`
- `VOICE_CHAT_LOGIN`: status: VoiceChatStatusCode
- `VOICE_CHAT_LOGOUT`: status: VoiceChatStatusCode
- `VOICE_CHAT_MUTED_CHANGED`: isMuted: bool
- `VOICE_CHAT_OUTPUT_DEVICES_UPDATED`
- `VOICE_CHAT_PENDING_CHANNEL_JOIN_STATE`: channelType: ChatChannelType, clubId: ClubId?, streamId: ClubStreamId?, pendingJoin: bool
- `VOICE_CHAT_PTT_BUTTON_PRESSED_STATE_CHANGED`: isPressed: bool
- `VOICE_CHAT_SILENCED_CHANGED`: isSilenced: bool
- `VOICE_CHAT_SPEAK_FOR_ME_ACTIVE_STATUS_UPDATED`
- `VOICE_CHAT_SPEAK_FOR_ME_FEATURE_STATUS_UPDATED`
- `VOICE_CHAT_TTS_PLAYBACK_BOOKMARK`: utteranceID: number, bookmarkName: cstring
- `VOICE_CHAT_TTS_PLAYBACK_FAILED`: utteranceID: number, status: VoiceTtsStatusCode
- `VOICE_CHAT_TTS_PLAYBACK_FINISHED`: utteranceID: number
- `VOICE_CHAT_TTS_PLAYBACK_STARTED`: utteranceID: number
- `VOICE_CHAT_TTS_SPEAK_TEXT_UPDATE`: status: VoiceTtsStatusCode, utteranceID: number
- `VOICE_CHAT_TTS_VOICES_UPDATE`
- `VOICE_CHAT_VAD_SETTINGS_UPDATED`
- `VOICE_CHAT_VOICE_PROVIDERS_AVAILABLE_CHANGED`
- `VOICE_CHAT_VOICE_PROVIDER_CHANGED`: voiceProviderID: VoiceProviderID

## WarbandSceneInfo

See [WarbandSceneInfo](systems/WarbandSceneInfo.md).

- `NEW_WARBAND_SCENE_ADDED`: warbandScenID: number
- `WARBAND_SCENE_FAVORITES_UPDATED`

## WeatherScript

See [WeatherScript](systems/WeatherScript.md).

- `WEATHER_CHANGED`

## WeeklyRewards

See [WeeklyRewards](systems/WeeklyRewards.md).

- `WEEKLY_REWARDS_ITEM_CHANGED`
- `WEEKLY_REWARDS_UPDATE`

## WorldLootObject

See [WorldLootObject](systems/WorldLootObject.md).

- `WORLD_LOOT_OBJECT_INFO_UPDATED`: guid: WOWGUID

## WorldStateInfo

See [WorldStateInfo](systems/WorldStateInfo.md).

- `CANCEL_PLAYER_COUNTDOWN`: initiatedBy: WOWGUID, informChat: bool, initiatedByName: string?
- `START_PLAYER_COUNTDOWN`: initiatedBy: WOWGUID, timeRemaining: time_t, totalTime: time_t, informChat: bool, initiatedByName: string?
- `START_TIMER`: timerType: StartTimerType, timeRemaining: time_t, totalTime: time_t
- `STOP_TIMER_OF_TYPE`: timerType: StartTimerType
- `WORLD_STATE_TIMER_START`: timerID: number
- `WORLD_STATE_TIMER_STOP`: timerID: number

## WowEntitlementInfo

See [WowEntitlementInfo](systems/WowEntitlementInfo.md).

- `ENTITLEMENT_DELIVERED`: entitlementType: WoWEntitlementType, textureID: number, name: string, payloadID: number?, showFancyToast: bool
- `RAF_ENTITLEMENT_DELIVERED`: entitlementType: WoWEntitlementType, textureID: number, name: string, payloadID: number?, showFancyToast: bool, rafVersion: RecruitAFriendRewardsVersion

## WowSurvey

See [WowSurvey](systems/WowSurvey.md).

- `SURVEY_DELIVERED`

## WowTokenUI

See [WowTokenUI](systems/WowTokenUI.md).

- `TOKEN_AUCTION_SOLD`
- `TOKEN_BUY_CONFIRM_REQUIRED`
- `TOKEN_BUY_RESULT`: result: number
- `TOKEN_CAN_VETERAN_BUY_UPDATE`: result: number
- `TOKEN_DISTRIBUTIONS_UPDATED`: result: number
- `TOKEN_MARKET_PRICE_UPDATED`: result: number
- `TOKEN_REDEEM_BALANCE_UPDATED`
- `TOKEN_REDEEM_CONFIRM_REQUIRED`: choiceType: luaIndex
- `TOKEN_REDEEM_FRAME_SHOW`
- `TOKEN_REDEEM_GAME_TIME_UPDATED`
- `TOKEN_REDEEM_RESULT`: result: luaIndex, choiceType: luaIndex
- `TOKEN_SELL_CONFIRMED`
- `TOKEN_SELL_CONFIRM_REQUIRED`
- `TOKEN_SELL_RESULT`: result: number
- `TOKEN_STATUS_CHANGED`
