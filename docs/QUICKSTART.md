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

## 5. Daily Usage Workflow (Multilingual)

Once configured, your agent operates smoothly under the ARISE protocol across languages:

### Example A: Direct Actions
* **English:**
  ```text
  User: Run pytest now.
  Agent: [Runs pytest immediately and displays output]
  ```
* **Indonesian:**
  ```text
  User: Jalankan pytest sekarang.
  Agent: [Menjalankan pytest langsung dan menampilkan output]
  ```

### Example B: Planned / Complex Changes
* **English:**
  ```text
  User: Refactor database client to use connection pooling.
  Agent: [Analyzes codebase -> Creates Build Plan -> Locks Scope -> Requests ARISE]
  User: ARISE
  Agent: [Executes locked plan -> Runs tests -> Verifies results -> Reports outcome]
  ```
* **Indonesian:**
  ```text
  User: Refactor database client agar menggunakan connection pooling.
  Agent: [Analisis codebase -> Susun Build Plan -> Kunci Scope -> Minta ARISE]
  User: ARISE
  Agent: [Eksekusi plan terkunci -> Jalankan pengujian -> Verifikasi -> Lapor hasil]
  ```
