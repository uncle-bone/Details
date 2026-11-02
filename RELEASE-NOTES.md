# Details! CoA v1.1.11 — Timeline standalone window fix

- Fixes /timeline opening the empty transparent Tools/API/Macros/Scripts/Statistics container instead of Timeline.
- Opens the Timeline plugin's own fully initialized window on the legacy 3.3.5a client and closes that window directly.
- Stops embedding Timeline in the incompatible modern plugin container.
- Preserves the previous plugin nil-frame guards and Mechanics guardian ownership/combat changes.
- GitHub package validation does not replace live client UI testing.

Install all Details* addon folders under Interface/AddOns. Preserve WTF/SavedVariables. Enable the Timeline addon at character selection, then use /timeline.

Maintainer: Uncle Bone — https://github.com/uncle-bone/Details
Third-party licenses and attribution remain intact.
