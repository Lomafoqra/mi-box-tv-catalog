# Xiaomi Mi Box — TV Channel Catalog

This public repository contains **only** the TV channel catalog for the user's personal Android TV / Xiaomi Mi Box app.

Scope: Arabic-language and Israeli channels, including locally relevant channels, with category filters for sports, news, children, films, series, religion, and social/community programs. No worldwide channel catalog.

- `channels.json` contains channel metadata and source URLs; it does **not** host video or decrypt paid channels.
- `index.html` explains the catalog.
- Stream availability is provisional until checked on the TV box; some links can be geoblocked or require authorization.
- Updated by a separate private GitHub Actions worker once secure publishing is configured.

This catalog is read-only for the Android TV app. Do not store private access tokens or other credentials here.
