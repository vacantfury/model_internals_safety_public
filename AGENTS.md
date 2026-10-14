# AGENTS.md

Instructions for coding agents. Codex reads this file; Claude Code reads CLAUDE.md, which imports it.

## What this repository is

The public side of a research line on safety inside model parameters: how safety behavior is
carried in the weights and activations of open language models, and how training-time and
activation-level interventions can strengthen it. README.md lists what is released: papers
with a public version, and their code.

This repository is a generated render target. Its files are written by a renderer in a separate
source repository, and a fail-closed leak check runs before anything is written here.

## Rules

- Do not author, edit or fix tracked files here by hand. A change belongs in the source
  repository and arrives with the next render; a hand edit would be overwritten and would
  bypass the leak check.
- Everything here is public. Never add personal data, private notes, credentials, API keys or
  any file the renderer did not produce.
- When code is released here, running it is fine (README.md gives the commands). Outputs, logs
  and caches stay untracked (see .gitignore).
- A commit here records one render; its message says what was rendered.
