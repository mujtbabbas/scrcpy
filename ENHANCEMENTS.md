# Enhancements — Standalone Edition Changelog

Upstream: <https://github.com/Genymobile/scrcpy>
Maintainer of this edition: Syed Mujtaba Abbas (@mujtbabbas)

## v1.1.0 — Enhancement release (2026-10-20)

- Added "About This Standalone Edition" section to README.md with upstream link, base version provenance, and credit.
- Added this changelog (ENHANCEMENTS.md).
- Added .github/dependabot.yml (weekly GitHub Actions updates, plus Gradle for the Android server build defined by the root settings.gradle / server/build.gradle).
- Added .markdownlint.json and .github/workflows/markdown-check.yml (markdown linting automation for the extensive documentation under doc/; upstream release.yml workflow kept as-is).
- Added .editorconfig (standard editor settings, with a 4-space indent section for C and Java sources, matching the dominant indentation of this codebase).
- No build CI was added: building scrcpy genuinely requires the Meson/Ninja toolchain, SDL2/FFmpeg development libraries and the Android SDK, so a generic build workflow would fail rather than verify anything — this is noted here instead of shipping a broken workflow.

## v1.0.0 — Baseline (2026-10-20)

- Clean standalone baseline of Genymobile/scrcpy at upstream release v5.0.1 (snapshot commit a60891aea193d92e7e5c3942700eca63f9d19a5f, upstream HEAD dated 2026-10-08).
- Fork history severed; all files and the Apache-2.0 licence (LICENSE) preserved as-is, including the small binary assets (app/data icons, assets screenshot and the Gradle wrapper jar).
