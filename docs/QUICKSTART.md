# ARISE Protocol — Quick Start & Setup Guide
> **Published by ArionLabs**

This guide provides step-by-step instructions for integrating the **ARISE Protocol** into your favorite AI developer tools.

---

## 1. Google Antigravity

Google Antigravity provides powerful agentic capabilities and native pair-programming workflows.

### Global Setup
1. Open your Antigravity configuration directory (`~/.gemini/antigravity` or Settings).
2. Add the complete content of [`ARISE_PROTOCOL.md`](../ARISE_PROTOCOL.md) into your global system prompt or custom instructions.

### Workspace Setup
1. In your active project root, place the protocol in `.antigravity/system_prompt.md`.
2. Antigravity will automatically load the rules upon project initialization.

---

## 2. Claude Code & Anthropic Projects

### In Claude Code CLI
Create or update `CLAUDE.md` in your project root:
```bash
# Copy ARISE Protocol into your project's CLAUDE.md
cp path/to/ARISE_PROTOCOL.md ./CLAUDE.md
```
Claude Code automatically parses `CLAUDE.md` at the beginning of each session.

### In Claude Desktop / Claude Projects
1. Create a Project in Claude.ai.
2. In **Project Instructions**, paste the full contents of `ARISE_PROTOCOL.md`.
3. Add `ARISE_PROTOCOL.md` to the Project Knowledge files for instant cross-referencing.

---

## 3. Cursor IDE

Cursor supports system instructions via `.cursorrules` or the `.cursor/rules/` directory.

### Single File Rule
Place the contents of `ARISE_PROTOCOL.md` directly into a `.cursorrules` file at the root of your project:
```bash
cp ARISE_PROTOCOL.md .cursorrules
```

### Modular Rule (`.cursor/rules/arise.mdc`)
Create `.cursor/rules/arise.mdc`:
```markdown
---
description: ARISE Protocol Autonomous Governance
globs: *
alwaysApply: true
---

[Paste contents of ARISE_PROTOCOL.md here]
```

---

## 4. GitHub Copilot Workspace / Windsurf / Cline

### GitHub Copilot
Add to `.github/copilot-instructions.md` in your repository.

### Windsurf (Codeium)
Add to `.windsurfrules` in your workspace root.

### Cline / Roo Code
Paste into the **Custom Instructions** field in the extension settings.

---

## 5. Daily Usage Workflow

Once configured, your agent will operate under the ARISE protocol:

1. **Ask questions / explore:** The agent will answer directly and accurately.
2. **Execute simple direct commands:**
   ```text
   User: Jalankan pytest sekarang.
   Agent: [Runs pytest immediately and shows output]
   ```
3. **Request complex features or refactors:**
   ```text
   User: Refactor database client to use connection pooling.
   Agent: [Analyzes codebase -> Creates Build Plan -> Locks Scope -> Requests ARISE]
   ```
4. **Authorize execution:**
   ```text
   User: ARISE
   Agent: [Executes locked scope -> Runs tests -> Verifies results -> Reports outcome]
   ```
