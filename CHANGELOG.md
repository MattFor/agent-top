# Changelog

## [0.1.2] - 02:20 CET 17-11-2026

### Changed

- Released under the MIT licence.
- Python 3.11 or newer is required.

## [0.1.1] - 09:01 CET 16-11-2026

### Fixed

- `install` copies through existing `~/.local/bin` symlinks instead of replacing them with plain files, so a symlinked install keeps updating the file it points at.

## [0.1.0] - 08:24 CET 16-11-2026

### Added

- Super+Z popup listing the Claude Code, Codex, Copilot, Cursor and local model sessions open right now, with their subagents and token use; Enter or a click jumps to the session's tmux pane.

### Fixed

- Cursor sessions started as `agent` (not `cursor-agent`) are listed.

[0.1.2]: https://github.com/MattFor/agent-top/releases/tag/v0.1.2
[0.1.1]: https://github.com/MattFor/agent-top/releases/tag/v0.1.1
[0.1.0]: https://github.com/MattFor/agent-top/releases/tag/v0.1.0
