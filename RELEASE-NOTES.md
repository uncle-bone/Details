# Details! CoA v1.1.10 — Plugin container nil-frame crash guard

- Fixes the reported Details/core/plugins.lua nil-frame failure by validating plugin display frames before embedding or refreshing them.
- Keeps the v1.1.9 Mechanics guardian combat and ownership-cache fixes, and existing Timeline compatibility guards.
- The reported error is from Details core, not proof that Timeline itself was the crashing module. The fix prevents this specific nil-frame failure; further runtime testing is needed.

Install all Details* addon folders directly under Interface/AddOns. Preserve WTF/SavedVariables. Timeline remains disabled by default and can be enabled for testing.

Maintainer: Uncle Bone — https://github.com/uncle-bone/Details
Third-party license notices remain unchanged.
