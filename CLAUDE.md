# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

This is a **GitHub profile README repository** (`OCharnyshevich/ocharnyshevich`). The `README.md` here renders on the GitHub profile page at github.com/OCharnyshevich.

## Repository Contents

- `README.md` — profile README (HTML + Markdown) with social links, project table, and GitHub stats widgets
- `devbox.json` — Devbox shell with `gh`, `go-task`, `bat`, `file`

## Development Environment

Uses [Devbox](https://www.jetpack.io/devbox/) with direnv integration (`.envrc`).

### Running Commands

**Always** run commands through Devbox:

```
devbox run -- <command>
```

For example: `devbox run -- gh repo view`, `devbox run -- task --list`.

### Installing Missing Tools

If a command is not available, install it via Devbox:

```
devbox add <package>
```

This updates `devbox.json` and makes the tool available for future `devbox run` calls. Do not install tools globally or via other package managers.

## Editing Guidelines

- The README uses raw HTML for layout (centered heading, text links, table, side-by-side stat cards). Preserve the HTML structure when editing.
- The project table should only list **public** repositories.
- External widget URLs use the GitHub username `OCharnyshevich` as a parameter — keep this consistent.
