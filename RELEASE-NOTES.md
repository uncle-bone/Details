# Details! CoA v1.1.8 — Tinker pet recovery and Timeline safeguards

- Retains Demolition's working pet-only combat starts and ownership attribution.
- Mechanics and other custom summons no longer become permanently ignored when their first ownership lookup fails; retries are throttled to avoid expensive per-hit scans.
- Timeline guards missing custom specialization/class icons, malformed aura events, and incomplete older saved settings.
- Timeline is disabled by default for new installs as a precaution; existing addon enablement and saved settings are not erased.
- No combat-log fixture or live client test was available. Mechanics segment behavior and Timeline stability require in-game verification.

Install every Details* folder from the ZIP directly under Interface/AddOns. Preserve WTF/SavedVariables. Enable Details! and optionally Timeline from the in-game AddOns menu.

Maintainer: Uncle Bone — https://github.com/uncle-bone/Details
Third-party license notices remain unchanged.
