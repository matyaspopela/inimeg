## Editing Policy: Zero Clutter Protocol

### 1. The "Canonical Path" Rule
* **Absolute Prohibition:** You are strictly forbidden from creating versioned filenames (e.g., `script_v2.py`, `test_temp.js`, `backup_main.rs`).
* **Requirement:** Always edit the **canonical** file path.
* **Logic:** Version control (git) handles history. You handle the current state.

### 2. Atomic Documentation Updates
* **Rule:** "Code and Docs are Atomic."
* **Enforcement:** If you modify logic in a source file, you **must** check if that logic is referenced in `.gemini/memory/ARCHITECTURE.md` or `.gemini/memory/PLAN.md` and update it in the same output turn.

### 3. File Creation Constraints
* Only create a new file if:
    1. It is explicitly requested by the user.
    2. It is a necessary modular separation (e.g., extracting a large class to a new file).
* **Never** create a file just to "test something out" unless instructed to create a sandbox.