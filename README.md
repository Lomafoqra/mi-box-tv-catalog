# Xiaomi Mi Box — TV Channel Catalog

This public repository contains **only** the TV channel catalog for the user's personal Android TV / Xiaomi Mi Box app.

Scope: Arabic-language and Israeli channels, including locally relevant channels, with category filters for sports, news, children, films, series, religion, and social/community programs. No worldwide channel catalog.

- `channels.json` contains channel metadata and source URLs; it does **not** host video or decrypt paid channels.
- `index.html` explains the catalog.
- Stream availability is provisional until checked on the TV box; some links can be geoblocked or require authorization.
- Updated by a separate private GitHub Actions worker once secure publishing is configured.

This catalog is read-only for the Android TV app. Do not store private access tokens or other credentials here.


## Expanded channel directory (Arabic + Israeli only)

- [expanded-channel-directory.json](expanded-channel-directory.json) — a curated list of 101 specific channels reviewed from official/public provider listings, including ART, OSN, MBC, Rotana, beIN, Alkass, SSC, Israeli sports, and Ehna TV.
- 24 of these have exact/alias matches in the existing `channels.json` streams list.
- 77 are **metadata-only records** without a matching playable entry; they must not be shown as working live streams.
- This is not a worldwide channel list. International movie titles within Arabic/Israeli TV packages do not add global providers.
- The existing `channels.json` scanning and publishing cycle every 6 hours is **unchanged**.
- Orbit is a historical brand merged into OSN. Only current verified channel names are listed.
- Names and lineups can change. Source pages and a review date are stored for follow-up checking. A successful HTTP response is not proof that video playback works on Android TV.

The TV app may eventually read both files, treating the expanded directory as a *discovery/coverage backlog* and `channels.json` as the stream candidates. Never silently turn a metadata-only record into a playable stream.
