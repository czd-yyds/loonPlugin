# Loon Kelee Plugins for 3.2.4

Source mirror: https://github.com/Moli-X/Tool/tree/X/Loon/Plugin/Kelee
Original upstream path requested: https://kelee.one/Tool/Loon/Plugin/

All usable plugin files have `#!loon_version=3.2.4`. Existing version headers were rewritten, and missing version headers were inserted into the metadata block.

Counts:
- Source plugin entries: 171
- Windows-visible files in `plugins/`: 170
- Rewritten version headers: 153
- Inserted missing version headers: 17
- Files missing or using another `#!loon_version`: 0

Note: the source contains both `BoxJs.plugin` and `Boxjs.plugin`. Windows cannot keep both in one directory because paths are case-insensitive, so the two normalized copies are preserved under `case-conflicts/BoxJs/` and `case-conflicts/Boxjs/`. The `plugins/` directory keeps one local importable BoxJs file.

Private GitHub access caveat: Loon cannot normally fetch a private repository with a plain `raw.githubusercontent.com` URL because it cannot send your GitHub `Authorization` header. GitHub's REST API supports authenticated content reads, but a Loon plugin URL usually needs a directly fetchable URL. For phone use, either use a public-but-unlisted repo, or use a private repo plus a small authenticated proxy that injects the GitHub token server-side.
