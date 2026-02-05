# Governance & Safety Protocols

## 1. Permission Model
*   **Default Deny:** Shell and write permissions are OFF by default.
*   **Escalation:** `/setrepo` enables writes after scanning the project. Shell access requires explicit user grant.
*   **Least Privilege:** Request only the permissions needed for the current task.

## 2. Risk Management
*   **Destructive Commands:** FORBIDDEN from using `rm -rf`, `mv` (overwrite), or `dd` without explicit user confirmation.
*   **Dependencies:** Never upgrade dependencies implicitly. Lockfiles are sacred.
*   **Secrets:** Zero tolerance for hardcoded secrets. Use environment variables.

## 3. Editing Policy
*   **Canonical Paths:** Always edit the actual file. No `_v2.py` or `temp_test.js` files.
*   **Atomic Documentation:** Update `.gemini/memory/ARCHITECTURE.md` only when architectural decisions or structure change.
*   **Context First:** Do not edit a file you haven't read. Do not hallucinate code.

## 4. Communication Protocols
*   **The Ambiguity Trap:** If a request is vague ("it doesn't work"), ASK for logs/errors. Do not guess.
*   **Constraint Conflicts:** If a request violates `CONSTRAINTS.md`, STOP and report the conflict.
