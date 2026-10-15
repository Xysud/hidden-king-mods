# Hidden King Mods

Release feed and compiled VPKs for Hidden King’s own Deadlock mods. This repository contains mod releases, not the desktop application source.

## Automatic updates

Hidden King checks `feed.json` after Deadlock build changes and every 15 minutes while open. It updates only mods you already installed, waits for the game to close, and preserves enabled state, priority and saved settings.

Releases name specific supported game builds and required stock-resource hashes. Downloads are checked against their SHA-256, VPK resource CRCs and the app’s reviewed resource allowlist. Unknown mods are ignored.

A game patch can still require a rebuilt mod. Automatic updates install published fixes; they cannot create those fixes. If the relevant stock assets are unchanged, the existing release may remain compatible.

## Publishing

Add a new, increasing revision to `feed.json` after reviewing a compiled package against the intended build. Keep previous entries for older game builds. Publish the package under a content-addressed filename, alongside the feed. Never replace a published package or reuse a revision for changed content or compatibility metadata.

Current release: **Hidden King Extras**, revision **2026101501**, Deadlock build **6785**. The required stock UI roots match this build; this is not a guarantee against all gameplay issues.
