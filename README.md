# geosweeper-pages

The public privacy policy and support site for **GeoSweeper**, served by GitHub Pages from
`docs/`. This repo holds nothing but that site — the app's source stays in its own, private
repo.

- https://ivnsjdev.github.io/geosweeper/
- https://ivnsjdev.github.io/geosweeper/privacy/
- https://ivnsjdev.github.io/geosweeper/support/

Every build of GeoSweeper links the privacy and support URLs above from inside the app
(paywalls, and Settings). Once a build ships carrying them, this site — or a redirect from
it — must keep serving those two paths for as long as any copy of that build is installed.
See `~/.claude/skills/ivan-app-store-pages/references/hosting.md` for the full rules before
moving or renaming anything here.
