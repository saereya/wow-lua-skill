# GossipConstants

source `interface/addons/blizzard_apidocumentationgenerated/gossipconstantsdocumentation.lua` (FileDataID 4686646)

## Types

### GossipNpcOption

*Enumeration* · 71 values, 0..70

Access values as `Enum.GossipNpcOption.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `GossipNpcOption` | = 0 |
| `Vendor` | `GossipNpcOption` | = 1 |
| `Taxinode` | `GossipNpcOption` | = 2 |
| `Trainer` | `GossipNpcOption` | = 3 |
| `SpiritHealer` | `GossipNpcOption` | = 4 |
| `Binder` | `GossipNpcOption` | = 5 |
| `Banker` | `GossipNpcOption` | = 6 |
| `PetitionVendor` | `GossipNpcOption` | = 7 |
| `GuildTabardVendor` | `GossipNpcOption` | = 8 |
| `Battlemaster` | `GossipNpcOption` | = 9 |
| `Auctioneer` | `GossipNpcOption` | = 10 |
| `TalentMaster` | `GossipNpcOption` | = 11 |
| `Stablemaster` | `GossipNpcOption` | = 12 |
| `PetSpecializationMaster` | `GossipNpcOption` | = 13 |
| `GuildBanker` | `GossipNpcOption` | = 14 |
| `Spellclick` | `GossipNpcOption` | = 15 |
| `DisableXPGain` | `GossipNpcOption` | = 16 |
| `EnableXPGain` | `GossipNpcOption` | = 17 |
| `Mailbox` | `GossipNpcOption` | = 18 |
| `WorldPvPQueue` | `GossipNpcOption` | = 19 |
| `LFGDungeon` | `GossipNpcOption` | = 20 |
| `ArtifactRespec` | `GossipNpcOption` | = 21 |
| `CemeterySelect` | `GossipNpcOption` | = 22 |
| `SpecializationMaster` | `GossipNpcOption` | = 23 |
| `GlyphMaster` | `GossipNpcOption` | = 24 |
| `QueueScenario` | `GossipNpcOption` | = 25 |
| `GarrisonArchitect` | `GossipNpcOption` | = 26 |
| `GarrisonMissionNpc` | `GossipNpcOption` | = 27 |
| `ShipmentCrafter` | `GossipNpcOption` | = 28 |
| `GarrisonTradeskillNpc` | `GossipNpcOption` | = 29 |
| `GarrisonRecruitment` | `GossipNpcOption` | = 30 |
| `AdventureMap` | `GossipNpcOption` | = 31 |
| `GarrisonTalent` | `GossipNpcOption` | = 32 |
| `ContributionCollector` | `GossipNpcOption` | = 33 |
| `Transmogrify` | `GossipNpcOption` | = 34 |
| `AzeriteRespec` | `GossipNpcOption` | = 35 |
| `IslandsMissionNpc` | `GossipNpcOption` | = 36 |
| `UIItemInteraction` | `GossipNpcOption` | = 37 |
| `WorldMap` | `GossipNpcOption` | = 38 |
| `Soulbind` | `GossipNpcOption` | = 39 |
| `ChromieTimeNpc` | `GossipNpcOption` | = 40 |
| `CovenantPreviewNpc` | `GossipNpcOption` | = 41 |
| `RuneforgeLegendaryCrafting` | `GossipNpcOption` | = 42 |
| `NewPlayerGuide` | `GossipNpcOption` | = 43 |
| `RuneforgeLegendaryUpgrade` | `GossipNpcOption` | = 44 |
| `CovenantRenownNpc` | `GossipNpcOption` | = 45 |
| `BlackMarketAuctionHouse` | `GossipNpcOption` | = 46 |
| `PerksProgramVendor` | `GossipNpcOption` | = 47 |
| `ProfessionsCraftingOrder` | `GossipNpcOption` | = 48 |
| `ProfessionsOpen` | `GossipNpcOption` | = 49 |
| `ProfessionsCustomerOrder` | `GossipNpcOption` | = 50 |
| `TraitSystem` | `GossipNpcOption` | = 51 |
| `BarbersChoice` | `GossipNpcOption` | = 52 |
| `MajorFactionRenown` | `GossipNpcOption` | = 53 |
| `PersonalTabardVendor` | `GossipNpcOption` | = 54 |
| `ForgeMaster` | `GossipNpcOption` | = 55 |
| `CharacterBanker` | `GossipNpcOption` | = 56 |
| `AccountBanker` | `GossipNpcOption` | = 57 |
| `ProfessionRespec` | `GossipNpcOption` | = 58 |
| `RenameNeighborhood` | `GossipNpcOption` | = 59 |
| `HousingCreateGuildNeighborhood` | `GossipNpcOption` | = 60 |
| `HousingGetNeighborhoodCharter` | `GossipNpcOption` | = 61 |
| `GuildRename` | `GossipNpcOption` | = 62 |
| `HousingOpenCharterConfirmation` | `GossipNpcOption` | = 63 |
| `ItemUpgrade` | `GossipNpcOption` | = 64 |
| `HouseFinder` | `GossipNpcOption` | = 65 |
| `TieredEntrance` | `GossipNpcOption` | = 66 |
| `PetUntrainer` | `GossipNpcOption` | = 67 |
| `TransmogOptIn` | `GossipNpcOption` | = 68 |
| `TransmogOptOut` | `GossipNpcOption` | = 69 |
| `RewardsShop` | `GossipNpcOption` | = 70 |

### GossipNpcOptionDisplayFlags

*Enumeration* · 1 values, 1..1

Access values as `Enum.GossipNpcOptionDisplayFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `ForceInteractionOnSingleChoice` | `GossipNpcOptionDisplayFlags` | = 1 |

### GossipOptionRecFlags

*Enumeration* · 3 values, 1..4

Access values as `Enum.GossipOptionRecFlags.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `QuestLabelPrepend` | `GossipOptionRecFlags` | = 1 |
| `HideOptionIDFromClient` | `GossipOptionRecFlags` | = 2 |
| `PlayMovieLabelPrepend` | `GossipOptionRecFlags` | = 4 |
