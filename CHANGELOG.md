# Changelog

All notable changes to Cove are documented in this file.

The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

## [0.1.0] - 2026-09-10

### Added

- Cove can open your library to an agent on your Mac. Turn on the MCP Server in Settings under Advanced. An agent that speaks MCP can then list your feeds and folders, read unread and starred articles, open one article, mark articles read, and add, rename, move, or remove a feed. The server is off until you turn it on, it listens only on this Mac, and it needs the token Cove gives you. Choose HTTP or the bundled stdio bridge, and copy the configuration block Cove shows you. Cove ships no agent of its own; the agent is yours.

### Changed

- Cove starts faster. It no longer prepares the audio system or searches for its data model before it needs them, so Now Playing stays free until you listen.
- Listen begins speaking sooner.
- About is now the last tab in Settings, after Advanced.

### Fixed

- Links in an article that did nothing when you clicked them now open. Cove resolves a link against the article's own address, and discards a destination it cannot make sense of instead of trying to open it.

## [0.0.10] - 2026-08-28

### Changed

- Archived feeds now keep article state, including read, starred, and set-aside status.

### Fixed

- Space now scrolls WebKit-rendered articles correctly, then moves to the next article at the end.
- User-renamed feeds now keep their custom titles after refreshes and feed metadata updates.

## [0.0.9] - 2026-08-25

### Changed

- Cove can replace short feed previews with a clearly better full article when it is available.
- The upgrade runs safely in the background and does not replace archived articles.

## [0.0.8] - 2026-08-17

### Added

- Cove now has its own appearance setting. Pick System, Light, or Dark in Settings under Reading, and it applies to the whole app instead of the reading pane alone. Read dark while your Mac stays light, or the reverse.
- Article lists can show thumbnails. Turn on Show Article Thumbnails in Settings under Feeds, and Cove shows the image a feed provides beside each article. Images are cached on your Mac and appear offline. The setting is off by default, so the list stays text-first unless you ask for it.

### Fixed

- The toolbar no longer holds its old colors after you switch between light and dark.

## [0.0.7] - 2026-08-08

### Added

- Choose whether marking an article as read moves you to the next story.
- Choose how unread activity appears in the sidebar: a count, a subtle dot, or nothing.

### Changed

- Cove queues several feed subscriptions added in quick succession and keeps you informed as they finish.
- Articles now credit every listed author.
- Set-aside articles remain visible in Unread, with a clear way to restore them, while staying out of unread counts and Next Unread.

## [0.0.6] - 2026-08-02

### Added

- Clips — select any passage in an article and save it. Clips get their own place in the sidebar, hold your notes, stay highlighted in the original article, and copy out with the citation attached. Searchable, and removable in bulk.

### Changed

- Setting older unread articles aside is now just how the reader behaves — no separate destination, no timer, no archive. They stay unread and exactly where they were until you act on them, and the Unread list tells you how many are set aside.
- "Mark All as Read" and its Above/Below and per-feed variants now leave set-aside articles alone, and the command dims when there's nothing left to mark.
- A voice model you download starts narrating as soon as its files are verified — no second step.
- Settings now links to Cove's Discord.

### Fixed

- Feeds, full-text fetches, and article images stay on HTTPS when a site redirects, instead of quietly dropping to plain HTTP.
- The "couldn't prepare this article" message sits centered in the reader pane instead of hugging a corner.

## [0.0.5] - 2026-07-25

### Added

- Tide gives you a calm way to set older unread articles aside without marking them read. Choose an age globally or per feed; articles stay available in Tide before moving to Archive.
- Listen to articles aloud with built-in macOS voices or optional on-device voice models.
- Follow along as Cove highlights and scrolls the paragraph being read.
- Control Listen from Now Playing and your media keys, with play, pause, and paragraph navigation.
- Adjust reader text size with ⌘+, ⌘−, and ⌘0.

### Changed

- Listen has clearer voice choices, shared speed controls, smoother buffering, and a more polished floating player.
- Voice-model downloads and library management are more dependable.
- OPML import and export handle files more reliably.

### Fixed

- Articles with literal line breaks late in an RSS feed now retain their text correctly.
- Listen avoids stale scroll jumps and responds more reliably to playback and voice-setting changes.
- Tide and OPML messages are clearer in edge cases.

## [0.0.4] - 2026-07-18

### Changed

- Exporting your feed subscriptions is more reliable, with a clear confirmation when the export is ready.
- Nested quotes in articles are easier to read.
- Selected sidebar icons now match their labels, including empty folders.
- Settings are clearer and easier to scan.
- Cove handles feed identities and existing library data more reliably.

### Fixed

- Your “mark articles as read when opened” preference works again.
- Feeds served over plain HTTP and summary-only Atom articles load reliably.

## [0.0.3] - 2026-07-17

### Added

- Initial usable release of Cove.

[Unreleased]: https://github.com/latent-signal/cove/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/latent-signal/cove/compare/v0.0.10...v0.1.0
[0.0.10]: https://github.com/latent-signal/cove/compare/v0.0.9...v0.0.10
[0.0.9]: https://github.com/latent-signal/cove/compare/v0.0.8...v0.0.9
[0.0.8]: https://github.com/latent-signal/cove/compare/v0.0.7...v0.0.8
[0.0.7]: https://github.com/latent-signal/cove/compare/v0.0.6...v0.0.7
[0.0.6]: https://github.com/latent-signal/cove/compare/v0.0.5...v0.0.6
[0.0.5]: https://github.com/latent-signal/cove/compare/v0.0.4...v0.0.5
[0.0.4]: https://github.com/latent-signal/cove/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/latent-signal/cove/compare/v0.0.2...v0.0.3
