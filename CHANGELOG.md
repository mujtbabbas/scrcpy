# Changelog

All notable changes to this standalone edition of scrcpy are documented in this file.

## v1.1.0 — Standalone enhancements (2026-10-20)

- Converted the repository from a fork into a standalone edition with its own history, keeping full upstream credit.
- Added an "About This Standalone Edition" section to `README.md` with the upstream link, base-version provenance, and credit.
- Added `ENHANCEMENTS.md` documenting everything changed in this edition.
- Added `.github/dependabot.yml` for weekly GitHub Actions updates, plus Gradle updates for the Android server build (root `settings.gradle` / `server/build.gradle`).
- Added markdown linting automation (`.markdownlint.json` and the Markdown check workflow) for the extensive documentation under `doc/`; the check was later scoped via `.markdownlint-cli2.yaml` so it covers this edition's own documentation instead of failing on upstream content. Upstream's `release.yml` workflow was kept as-is.
- Added `.editorconfig` (standard editor settings, with a 4-space indent section for C and Java sources, matching the dominant indentation of this codebase).
- No build CI was added: building scrcpy genuinely requires the Meson/Ninja toolchain, SDL2/FFmpeg development libraries and the Android SDK, so a generic build workflow would fail rather than verify anything — noted here instead of shipping a broken workflow.

## v1.0.0 — Upstream baseline (2026-10-20)

- Clean standalone baseline of [Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) at upstream release v5.0.1 (snapshot commit `a60891aea193d92e7e5c3942700eca63f9d19a5f`, upstream HEAD dated 2026-10-08).
- Fork history severed; all files and the Apache-2.0 licence (`LICENSE`) preserved as-is, including the small binary assets (app/data icons, assets screenshot and the Gradle wrapper jar).
