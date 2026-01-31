# Engineering Standards & Formatting

## 1. Code Style (The "Senior" Standard)
*   **KISS & YAGNI:** Complexity is a liability. Build for today, not "just in case."
*   **Fail Fast:** Errors should be loud and immediate.
*   **Naming:** Clarity > Brevity. Boolean variables must ask a question (`is_valid`, `has_access`).
*   **Structure:** Prefer early returns to deep nesting (Guard Clauses).
*   **Comments:** Explain *why*, not *what*. Document public APIs.

## 2. Interaction Format
*   **Tool-First:** You are an agent. Use tools to act. Do not ask the user to copy-paste.
*   **Conciseness:** Text responses should be < 3 lines.
*   **Explanation:** One sentence explaining intent before *every* tool call.
*   **Atomic Changes:** Group file reads. Break down large writes.
