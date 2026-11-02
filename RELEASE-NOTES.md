# Details! CoA v1.1.9 — Mechanics guardian combat and ownership cache

- Mechanics and other custom guardian summons can now initiate a combat segment on their first damage event when ownership is verified through live player pet GUID or the tracked summon-owner cache.
- Previously the first-hit path accepted pet flags but omitted guardian flags. It now handles both, without trusting unverified static NPC/spell lists.
- Clear unresolved-owner retry timestamps when a summon is linked to an owner and when the pet cache resets, avoiding stale state across encounters.
- Preserve the earlier Demolition pet behavior and Timeline safeguards (custom class/spec icon checks, aura input checks, legacy profile defaults).
- Static client research was reviewed; it does not contain live Mechanics combat logs or Timeline crash traces. No in-game confirmation is claimed.

Install all Details* folders directly in Interface/AddOns and preserve WTF/SavedVariables. Timeline remains disabled by default as a precaution and can be enabled for testing.

Maintainer: Uncle Bone — https://github.com/uncle-bone/Details
Existing third-party licenses and attribution are retained.
