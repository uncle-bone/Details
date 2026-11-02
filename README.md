# Details! CoA v1.1.12 — Tinker Mechanics and Timeline fixes

> **[⬇ Download the latest stable release — v1.1.12](https://github.com/uncle-bone/Details/releases/download/v1.1.12/Details-v1.1.12.zip)**  
> [GitHub release and changelog](https://github.com/uncle-bone/Details/releases/tag/v1.1.12)

Details! CoA is a modified Details! combat meter for **Ascension Conquest Reborn**, targeting **World of Warcraft 3.3.5a (Lua 5.1)**.

## What's included in v1.1.12

- **CoA-Research v2.0.1:** evidence-safe integration of summon-owner chaining; no speculative historical NPC/spell aliases imported into runtime attribution.
- **Summon reliability:** prevents self-owner loops and preserves confirmed owners when duplicate or incomplete summon events arrive.

- **Tinker Mechanics:** recognizes owned guardian-type summons as well as ordinary pets when determining first-hit combat starts; preserves existing Demolition fixes.
- **Summon attribution:** retries unresolved ownership lookups without permanently ignoring summons, and clears stale retry state when ownership resolves or encounters reset.
- **Timeline:** `/timeline` now opens its standalone Timeline frame instead of the transparent Tools/API/Macros/Scripts panel. Includes nil-frame, aura-event, custom-class icon and saved-profile safeguards.
- **Class/spec tooltips:** retains custom class-scoped specialization mapping, equipment-level handling and combat history fixes from earlier versions.
- **Compatibility:** 13 Details* addon folders packaged together; existing saved preferences are not intentionally reset.

## Installation and testing

1. Download the ZIP above and extract **all Details* folders** directly into `World of Warcraft/Interface/AddOns/`.
2. Enable **Details! Damage Meter** at the character-selection AddOns screen.
3. To use Timeline, also enable **Details!: Time Line (plugin)**, restart the client and type `/timeline`.
4. Preserve and back up `WTF/SavedVariables` when updating.

**Testing note:** GitHub packaging passed. Mechanics summon behavior and Timeline stability have not yet been exhaustively verified in the live Conquest Reborn client. Report any errors with the complete `/crerrors copy` traceback.

Maintainer: **Uncle Bone** — https://github.com/uncle-bone  
Original Details! and third-party license notices are retained.

## Earlier combat changes

### v1.1.0 — Expanded combat

- Pet-only hostile damage starts a combat segment for confirmed owned pets, including group pets.
- Resolves ownership on the first damage event through pet GUIDs, cached ownership or party/raid pet scans when SPELL_SUMMON is absent.
- Preserves Primalist focus/synergy attribution from the supplied Conquest Reborn combat log.
- Retains summon-name/nil safeguards, combat-segment persistence, a default 50-segment history for new profiles, maintainer metadata and the Demolition label.
- Keeps combat parsing dynamic for client-reported spell IDs; no giant unvalidated SQL database is loaded into addon memory.

This is the complete supplied multi-folder package. Some optional legacy plugins ship disabled TOCs; they remain disabled. Install all Details* folders side by side, then enable Details in the AddOns menu (its TOC defaults to disabled). Keep existing SavedVariables.

Full live-client validation and exhaustive Tinker pet/turret mappings remain pending. Original Details! attribution and bundled licenses are retained.

Maintainer: Uncle Bone — https://github.com/uncle-bone

## Support and attribution

Report errors with your addon version, UI addons and full Lua traceback at https://github.com/uncle-bone/Details/issues. Target: Ascension Conquest Reborn / WoW 3.3.5a (Interface 30300). Original source notices and bundled third-party licenses are preserved.

