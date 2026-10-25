# SecretPredicates

source `interface/addons/blizzard_apidocumentationgenerated/secretpredicatesdocumentation.lua` (FileDataID 7552722)

## Predicates

Conditions referenced by the flags above.

- `RequiresComparableUnitTokens` *Precondition* (failure mode: ReturnNothing): Guarded APIs only accept unit token pairs that can be compared with one another. For example, comparisons where either unit is 'player' or 'target' are permitted, but comparisons between 'nameplate3' and 'boss1' are not.
- `RequiresDeclassifiedUnitIdentity` *Precondition* (failure mode: ReturnWithError): Guarded APIs and events require that callers have access to the identity of a supplied unit token.
- `RequiresFontStringTextAccess` *Precondition* (failure mode: ReturnNothing): Guarded APIs reject access for tainted callers if the object has the secret Text aspect assigned.
- `RequiresNonSecretAura` *Precondition*: Guarded APIs require that that the requested aura be non-secret at the time of the API call. This does not raise a blocked action error - instead, protected APIs will return no values.
- `RequiresScriptObjectAlphaAccess` *Precondition* (failure mode: ReturnWithError)
- `RequiresScriptObjectDesaturationAccess` *Precondition* (failure mode: ReturnWithError)
- `RequiresStatusBarDesaturationAccess` *Precondition* (failure mode: ReturnWithError)
- `RequiresUnitAuraAccess` *Precondition* (failure mode: Error): Guarded APIs and events require that callers have access to unit aura data.
- `RequiresUnitIdentityAccess` *Precondition* (failure mode: ReturnWithError): Guarded APIs and events require that callers have access to unit identity values. This does not raise a blocked action error - instead, protected APIs will return no values.
- `SecretInActivePvPMatch` *Secret*: Guarded APIs and events produce secret values when PvP match addon restrictions are in effect.
- `SecretInChatMessagingLockdown` *Secret*: Guarded APIs and events produce secret values when encounter, challenge mode, or PvP match addon restrictions are in effect, and when the player is on a communication-restricted map such as a dungeon or raid.
- `SecretOnRestrictedMaps` *Secret*: Guarded APIs and events produce secret values when the player is on an addon-restricted map such as a dungeon or raid.
- `SecretWhenAnchoringSecret` *Secret*: Guarded APIs and events produce secret values when an object has secret anchoring information.
- `SecretWhenUnitAuraRestricted` *Secret*: Guarded APIs and events produce secret values when combat, encounter, challenge mode, or PvP match addon restrictions are in effect. Individual spells may be flagged as never or always secret, which takes priority over restrictions.
- `SecretWhenAurasRestricted` *Secret*: Guarded APIs and events produce secret values when combat, encounter, challenge mode, or PvP match addon restrictions are in effect.
- `SecretWhenCooldownsRestricted` *Secret*: Guarded APIs and events produce secret values when combat, encounter, challenge mode, or PvP match addon restrictions are in effect. Individual spells may be flagged as never or always secret, which takes priority over restrictions.
- `SecretWhenInCombat` *Secret*: Guarded APIs and events produce secret values when combat addon restrictions are in effect.
- `SecretWhenLossOfControlInfoRestricted` *Secret*: Guarded APIs and events produce secret values if the subject unit is not the active player, unless they are an active spectator or commentator of a PvP match.
- `SecretWhenTotemSlotSecret` *Secret*: Guarded APIs and events produce secret values when combat, encounter, challenge mode, or PvP match addon restrictions are in effect. Individual totem spell auras may be flagged as never or always secret, which takes priority over restrictions.
- `SecretWhenUnitSpellCastRestricted` *Secret*: Guarded APIs and events produce secret values if the unit being queried for cast information is not the player or their pet. Individual spells may be flagged as never or always secret, which takes priority.
- `SecretWhenUnitComparisonRestricted` *Secret*: Guarded APIs and events produce secret values based upon supplied unit tokens. Comparisons involving compound unit tokens (eg. 'boss1target') are always secret. This restriction only applies when the player is on an addon-restricted map.
- `SecretWhenUnitHealthMaxRestricted` *Secret*: Guarded APIs and events produce secret values when the unit isn't player-controlled.
- `SecretWhenUnitIdentityRestricted` *Secret*: Guarded APIs and events produce secret values when the unit isn't player-controlled or in the party/raid. For compound tokens (eg. 'boss1target'), results are secret if any unit in the chain fails this.
- `SecretWhenUnitNameIdentityRestricted` *Secret*: Guarded APIs and events produce secret values under regular unit identity secrecy rules, except in PvP when the queried unit is a player.
- `SecretWhenUnitPossessionRestricted` *Secret*: Guarded APIs and events produce secret values based on aura secrecy, except for unit tokens under the player's direct control.
- `SecretWhenUnitPowerMaxRestricted` *Secret*: Guarded APIs and events produce secret values when the unit isn't player-controlled. Individual power types may be flagged as never or always secret, which takes priority.
- `SecretWhenUnitPowerRestricted` *Secret*: Guarded APIs and events produce secret values for power types not explicitly flagged as being never secret, unless the subject unit does not have a power of this type.
- `SecretWhenUnitStatsRestricted` *Secret*: Guarded APIs and events produce secret values when access to unit stats would generally produce secret values.
- `SecretWhenUnitThreatStateRestricted` *Secret*: Guarded APIs and events produce secret values based upon supplied unit tokens. Queries where only one unit token is specified, or where one unit token is the player, their pet, or an ally while the other is a nameplate, boss, target, etc., are generally not secret.
- `SecretWhenUnitThreatValuesRestricted` *Secret*: Guarded APIs and events produce secret values based upon supplied unit tokens. Queries where only one unit token is specified, or where one unit token is the player, their pet, or an ally while the other is a non-boss or nameplate target, are generally not secret.
