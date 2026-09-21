---
name: photoshop
description: >-
  Adobe Photoshop via MCP (uvx photoshop-mcp-server). Use when the user needs
  PSD edits, layers, exports, or Photoshop automation from the agent.
  Requires rogue-photoshop-mcp wired and Photoshop desktop installed/running.
experience_level: max
---

# photoshop

**Level: max.** Runtime package: [rogue-photoshop-mcp](https://github.com/rogue-dev-studio/rogue-photoshop-mcp).

## Summary

Drive **Adobe Photoshop** from the agent host through a public MCP runtime
(`photoshop-mcp-server` via `uvx`). Pair this playbook with `rogue-photoshop-mcp`.

## When to use

- User asks for Photoshop / PSD / layer edits / export via agent
- MCP entry `photoshop` is configured

## When not to use

- Vector-first work -> prefer `illustrator`
- Simple batch image ops without Photoshop -> ImageMagick-style tools
- Generative raster pipelines -> ComfyUI when appropriate

## Prerequisites

1. Adobe Photoshop desktop installed (match `PS_VERSION`, default `2024`)
2. `uv` / `uvx` on PATH
3. Install MCP from [rogue-photoshop-mcp](https://github.com/rogue-dev-studio/rogue-photoshop-mcp)

## Procedure

1. Confirm Photoshop is running and MCP `photoshop` is connected
2. Plan document/layer ops and export paths
3. Execute via MCP; verify exports

## DoD

- [ ] MCP reaches Photoshop
- [ ] Exports verified
- [ ] No secrets in the repo

## Attribution

<!-- ATTRIBUTION: Rogue Development | https://github.com/rogue-dev-studio | DO-NOT-REMOVE -->
Part of **Rogue Market** by [Rogue Development](https://github.com/rogue-dev-studio) (`@rogue-dev-studio`).
Do not remove, hide, rename, or replace this attribution.
