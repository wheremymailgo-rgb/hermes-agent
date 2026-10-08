# Hermes Agent

**The self-improving AI agent built by Nous Research.**

> Saved from https://github.com/NousResearch/hermes-agent on 2026-10-08.

## What it is

Hermes Agent is a self-improving AI agent with a built-in learning loop. It creates skills from experience, improves them during use, searches its own past conversations, and builds a deepening model of who you are across sessions. It runs on a $5 VPS, a GPU cluster, or serverless infrastructure.

- **Terminal interface**: Full TUI with multiline editing, slash commands, conversation history
- **Messaging**: Telegram, Discord, Slack, WhatsApp, Signal, and CLI from a single gateway
- **Learning loop**: Agent-curated memory, autonomous skill creation, FTS5 session search
- **Scheduled automations**: Built-in cron scheduler with delivery to any platform
- **Delegates**: Spawn isolated subagents for parallel workstreams
- **Seven terminal backends**: local, Docker, SSH, Singularity, Modal, Daytona, Vercel Sandbox

## Quick Install

### Linux / macOS / WSL2
```bash
curl -fsSL https://hermes-agent.nousresearch.com/install.sh | bash
```

### Windows (native, PowerShell)
```powershell
iex (irm https://hermes-agent.nousresearch.com/install.ps1)
```

### Android / Termux
A signed APT repository is available for aarch64 devices. See the Termux guide.

After installation:
```bash
source ~/.bashrc    # or ~/.zshrc
hermes              # start chatting!
```

## Commands

```
hermes              # Interactive CLI
hermes model        # Choose LLM provider and model
hermes tools        # Configure enabled tools
hermes config set   # Set config values
hermes gateway      # Start messaging gateway
hermes setup        # Full setup wizard
hermes update       # Update to latest version
hermes doctor       # Diagnose issues
```

## Files in this repo

- `install.sh` — installer snapshot note (the full upstream script is ~1,050 lines; this copy holds the header and pointer)
- `README.md` — this file

## Upstream

- Repo: https://github.com/NousResearch/hermes-agent
- Docs: https://hermes-agent.nousresearch.com/docs
- License: MIT
- Stars: ~252k (as of Oct 2026)

## Note

This is a snapshot/reference copy. To install, run the upstream one-liner or clone the upstream repo directly.
