# Details! CoA v1.1.12 — CoA-Research v2.0.1 evidence-safe summon tracking

- Integrates the source-confidence distinction from CoA-Research v2.0.1. Archived class/spec/spell/NPC associations remain research-only; runtime damage attribution comes only from observed GUID ownership.
- Improves nested summon ownership resolution using a bounded 8-link traversal of existing observed summon cache, protecting against cycles.
- Prevents duplicate/incomplete summon events from erasing a confirmed owner or attributing a creature to itself.
- Retains Mechanics guardian first-hit combat handling, Demolition fixes, and Timeline standalone display fix.
- Does not load bulk SQL/JSON research into the addon or guess spell-to-NPC relationships.
- Live Mechanics combat logs and Timeline end-to-end UI testing remain outstanding.

Install all Details* folders under Interface/AddOns; preserve WTF/SavedVariables. Enable Timeline and use /timeline when needed.

Source research: https://github.com/uncle-bone/CoA-Research/releases/tag/shared-database-v2.0.1
Maintainer: Uncle Bone — https://github.com/uncle-bone/Details
Third-party licenses and attribution remain intact.
