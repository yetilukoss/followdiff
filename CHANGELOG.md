# Changelog

All notable changes to FollowDiff are documented here.
Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [0.0.1] - 2026-11-15

### Changed
- Reset version numbering to 0.0.1 (new scheme: 0.0.1 → 0.0.9 → 0.1.0 → 0.1.1)
- All features from 0.0.37 carried over

## [0.0.37] - 2026-11-14

### Fixed
- Copy username and copy list now work in the extension page (added `clipboardWrite` permission + `execCommand` fallback)
- Pin toast now fires on storage ack instead of optimistically
- Sync no longer lost when the service worker is evicted mid-run
- Closing the Instagram tab mid-sync now settles immediately instead of waiting 240s
- `resolveUserId` no longer grabs an unrelated user's id
- `require_login` now correctly reported as session-expired, not rate-limited
- Footer no longer clips at narrow widths (320/360px)
- Row avatar/name/handle are real keyboard-focusable buttons
- Footer center aligned on the app axis

### Changed
- Version bump to 0.0.37

## [0.0.36] - 2026-11-14

### Fixed
- Copy username fallback via execCommand

## [0.0.35] - 2026-11-14

### Added
- `clipboardWrite` permission

## [0.0.34] - 2026-11-14

### Fixed
- Service worker eviction no longer loses completed syncs
- Panel resets sync state on port disconnect ("Sync interrupted")
- Whitelist eviction now by time, not account-biased
- Quota retry only truncates on real quota errors
- `countChanges` now includes new followers

## [0.0.33] - 2026-11-14

### Fixed
- Multiple audit findings (logic, UI, packaging)

## [0.0.32] - 2026-11-12

### Added
- Pixel icon sheet sliced and wired into UI
- Jade `you.png` icon for the Mine button
- Two-circle logo (off-white ring + jade circle)
- Footer rebuilt: brand/version, snapshot count, credit, Clear all / Copy list

### Changed
- Panel tablist stacked (icon above label) under 720px; website keeps row tabs
- Hover/click motion on ghost, scan, sync, footer, tabs, rows, pins
