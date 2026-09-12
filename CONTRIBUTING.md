# Contributing to ARISE Protocol

Thank you for your interest in enhancing the **ARISE Protocol**! This project is maintained by **ArionLabs** and thrives on contributions from engineers, researchers, and AI practitioners worldwide.

---

## How to Contribute

### 1. Propose Protocol Refinements
If you discover an edge case where an AI coding agent misinterprets instructions, creates unintended hallucinations, or bypasses a scope lock:
1. Check existing [Issues](https://github.com/Huyt2612/arise-protocol/issues) to see if it has been reported.
2. Open an issue with a concrete reproduction transcript (Few-Shot format).
3. Propose a targeted refinement to the relevant directive.

### 2. Add New Platform Presets
We welcome pre-configured presets for emerging developer agents (e.g., Windsurf, Roo Code, Aider, OpenHands):
* Add the configuration file into the `templates/` directory.
* Update `docs/QUICKSTART.md` with verification steps.

### 3. Submitting a Pull Request
1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/refine-scope-lock`).
3. Commit your changes with clear, semantic commit messages (`git commit -m "docs: refine direct-action triggers"`).
4. Push to the branch (`git push origin feature/refine-scope-lock`).
5. Open a Pull Request using our standard PR template.

---

## Core Principles to Preserve
All contributions must honor the fundamental ARISE tenets:
* **Evidence Over Confidence:** Avoid subjective rules that cannot be verified.
* **YAGNI:** Do not introduce bureaucratic complexity for trivial tasks.
* **Exact Token Invariance:** The authorization token `ARISE` must remain universal and untranslated.

---

## Code of Conduct
Please be respectful, collaborative, and constructive in all discussions and code reviews.
