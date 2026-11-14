# FollowDiff

[![Version](https://img.shields.io/badge/version-0.0.37-2f8f6f)](https://github.com/yetilukoss/followdiff/releases)
[![Chrome Web Store](https://img.shields.io/badge/Chrome%20Web%20Store-coming%20soon-lightgrey)](https://github.com/yetilukoss/followdiff)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Privacy](https://img.shields.io/badge/privacy-local--only-brightgreen)](PRIVACY.md)

> See who follows you back, who doesn't, and what changed — without sending a single byte off your machine.

**FollowDiff** is a read-only Chrome/Brave extension for Instagram. It snapshots your followers and following lists locally, diffs them, and shows you the truth: who doesn't follow back, who your fans are, mutuals, and what changed since last time.

---

## ✨ Features

- **Not back** — people you follow who don't follow you back
- **Fans** — people who follow you but you don't follow back
- **Mutual** — accounts you both follow each other
- **Changes** — new followers, lost followers, new follows, unfollows since your last sync
- **Overlap** — compare two accounts' follower/following lists
- **Keep list** — whitelist accounts so they never show up in diffs
- **Avatars** — real profile pictures, loaded locally
- **Side panel + full tab** — use it in Brave/Chrome's side panel or open it as a full tab
- **100% local** — nothing leaves your browser. No accounts, no analytics, no telemetry

---

## 📸 Screenshots

<!-- Replace with real screenshots -->
| Panel | Full tab |
|---|---|
| ![panel](docs/screenshots/panel.png) | ![tab](docs/screenshots/tab.png) |

---

## 🚀 Installation

### Chrome Web Store (recommended)
> Coming soon. Submission in progress.

### Manual (developer mode)
1. Download the latest release from [Releases](https://github.com/yetilukoss/followdiff/releases)
2. Unzip
3. Open `brave://extensions` (or `chrome://extensions`)
4. Enable **Developer mode**
5. Click **Load unpacked** → select the unzipped folder

---

## 🧠 How it works

FollowDiff talks to Instagram's own web API using your existing session cookies — the same way the Instagram website does. It never asks for your password.

- **Read-only.** It only reads your follower/following lists. It never follows, unfollows, likes, or messages anyone.
- **Local storage only.** Snapshots are stored in `chrome.storage.local` on your device. Up to 12 snapshots per account.
- **No network calls to third parties.** The only network requests are to `instagram.com` and its CDN for avatars.
- **No account required.** No sign-up, no email, no tracking.

See [PRIVACY.md](PRIVACY.md) for the full privacy policy.

---

## 🎮 Usage

1. Log in to Instagram in your browser
2. Open the FollowDiff side panel (click the extension icon)
3. Press **Sync** — FollowDiff reads your lists and saves a snapshot
4. Switch between tabs: **Not back**, **Fans**, **Mutual**, **Changes**, **Overlap**
5. Use **Scan** to sync any other public account (type `@username`)
6. Use **Mine** to sync your own account again
7. **Pin** (★) accounts to keep them out of every diff
8. **Clear all** to wipe history

### Keyboard shortcuts
| Key | Action |
|---|---|
| `/` | Focus search |
| `1`–`5` | Switch tabs |
| `r` | Sync |
| `Esc` | Clear search |

---

## 🔒 Privacy

- No data collection. No analytics. No telemetry.
- All data stays in `chrome.storage.local` on your device.
- Instagram's session cookies are used only to read your lists, never transmitted elsewhere.
- Full policy: [PRIVACY.md](PRIVACY.md)

---

## 🐛 Bug reports

Found a bug? Open an issue:

- [Report a bug](https://github.com/yetilukoss/followdiff/issues/new?template=bug_report.yml)
- [Request a feature](https://github.com/yetilukoss/followdiff/issues/new?template=feature_request.yml)

Please include your browser, extension version, and steps to reproduce. **Do not include your Instagram username or account data in public issues.**

---

## 📋 Changelog

See [CHANGELOG.md](CHANGELOG.md) for version history.

---

## 🤝 Contributing

Source code is maintained in a private repository. Bug reports and feature requests are welcome via [Issues](https://github.com/yetilukoss/followdiff/issues).

---

## 📜 License

MIT — see [LICENSE](LICENSE).

---

## 🙏 Credits

Built by **@!yeti**.

---

<p align="center">
  <sub>FollowDiff is not affiliated with, endorsed by, or sponsored by Meta or Instagram.</sub>
</p>
