# Ethos Link GitHub defaults

## Shared GitHub Defaults

This repository holds the shared GitHub templates we reuse across Ethos Link projects.

## Organisation profile

The public [Ethos Link](https://www.ethos-link.com) organisation profile lives in
[profile/README.md](profile/README.md). It introduces the company and founder,
links to Reviato, Nuntio and EthosPlaces, and lists our public engineering tools.

Keep product names, descriptions and article links aligned with the product
sites. Nuntio's articles are published under `/guides`; EthosPlaces does not yet
have an articles section.

## Repository social preview

The [PNG preview](.github/social-preview.png) is ready to upload. Its
[editable SVG source](.github/social-preview.svg) embeds the website's Manrope
and DM Sans fonts; their licence notices are in [docs/fonts](docs/fonts).
The design uses the website's navy, teal, paper and mint palette.

Upload the PNG through **Repository → Settings → Social preview → Edit →
Upload an image**. Committing it does not activate the preview. This setting
controls previews of this repository's URL, rather than the organisation URL
or its profile banner.

The image is 1280 × 640 pixels and must remain under 1 MB. After editing the
SVG, render it with Chromium from the repository root:

```sh
chromium --headless --disable-gpu --hide-scrollbars \
  --force-device-scale-factor=1 --window-size=1280,640 \
  --virtual-time-budget=2000 --screenshot="$PWD/.github/social-preview.png" \
  "file://$PWD/.github/social-preview.svg"
```

The executable may be named `chromium-browser` or `google-chrome` on your
system. Inspect the exported PNG at full and half size before uploading it.

## Repository Conventions

- Use Conventional Commits for commits and PR titles.
- Prefer squash merge for library and gem repositories.
- Treat the PR title as the final squash commit message that lands on `main` or `master`.
- Keep PR titles ready for changelog generation, because `git-cliff` release notes are derived from tagged Conventional Commits.
- Keep shared issue and PR templates generic enough to work across multiple repositories.
