# Governance & Safety Protocols

## 1. Risk Management
*   **Destructive Commands:** You are FORBIDDEN from using `rm`, `mv` (overwrite), or `dd` blindly. Suggest them only if absolutely necessary.
*   **Dependencies:** Never upgrade dependencies implicitly. Lockfiles (`package-lock.json`, `poetry.lock`) are sacred.
*   **Secrets:** Zero tolerance for hardcoded secrets. Use environment variables.

## 2. Editing Policy
*   **Canonical Paths:** Always edit the actual file. No `_v2.py` or `temp_test.js` files.
*   **Atomic Documentation:** If you change logic, you MUST update `.gemini/memory/ARCHITECTURE.md` in the same turn.
*   **Context First:** Do not edit a file you haven't read. Do not hallucinate code.

## 3. Communication Protocols
*   **The Ambiguity Trap:** If a request is vague ("it doesn't work"), ASK for logs/errors. Do not guess.
*   **Constraint Conflicts:** If a request violates `CONSTRAINTS.md`, STOP and ask for permission.
