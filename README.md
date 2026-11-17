# Agent Top

[![CI](https://github.com/MattFor/agent-top/actions/workflows/ci.yml/badge.svg)](https://github.com/MattFor/agent-top/actions/workflows/ci.yml)
[![Release](https://img.shields.io/github/v/release/MattFor/agent-top)](https://github.com/MattFor/agent-top/releases)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

A Super+Z popup listing the Claude Code, Codex, Copilot and local model sessions open right now.

## Features

- One row per live session with its state (working, waiting, idle), model, effort, ultracode, run time and topic; subagents and Codex workers nest under the session that spawned them.
- Local model servers (Ollama, llama-server) show only while they compute.
- Plan limits for Claude, Codex and Copilot on demand.
- Enter or a click on the selected row jumps to that session's tmux pane or window.

## Requirements

Python 3.11+ (stdlib only), XFCE with xfce4-terminal, `wmctrl`, `xdotool`, `xprop`, `xrandr`.

## Install

`./install` copies `agent-top` and `agent-top-toggle` into `~/.local/bin` and binds Super+Z.

## Usage

Super+Z shows or hides the popup. `agent-top --once` prints one snapshot, `--no-color` drops colour and `--selftest` runs the checks.

### Keys

| Key              | Action                            |
| ---------------- | --------------------------------- |
| t                | topic instead of the session name |
| m                | model and effort                  |
| c                | run time                          |
| a                | current tool call                 |
| i                | tokens                            |
| s                | plan limits                       |
| ?                | key help                          |
| ↑↓ / j k / wheel | select                            |
| Enter / click    | jump to the session               |

Toggles persist in `~/.config/agent-top/config.json`.

## License

MIT, see [LICENSE](LICENSE). By [MattFor](https://github.com/MattFor).
