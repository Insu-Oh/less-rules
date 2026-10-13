# Less rules

Filter rules for the Less app, served at <https://rules.insu-lab.com/rules.json>.

Data only: CSS selectors, same-origin path rules and named params, checked by the app's schema
before use. The source of truth is `rules/rules.json` in the Less repository; publish from
there with `npm run rules:publish` (it validates the file, then commits it here). Don't edit
this repository by hand.

The app takes a ruleset only when its `rulesVersion` is newer than the one it has, so every
change bumps it (e.g. `2026-10-13.2`). To roll back, publish the old rules with a newer version.
