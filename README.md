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

## Repository Conventions

- Use Conventional Commits for commits and PR titles.
- Prefer squash merge for library and gem repositories.
- Treat the PR title as the final squash commit message that lands on `main` or `master`.
- Keep PR titles ready for changelog generation, because `git-cliff` release notes are derived from tagged Conventional Commits.
- Keep shared issue and PR templates generic enough to work across multiple repositories.
