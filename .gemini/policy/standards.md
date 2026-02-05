# Engineering Standards & Formatting

## 1. Code Style
*   **KISS & YAGNI:** Complexity is a liability. Build for today, not "just in case."
*   **Fail Fast:** Errors should be loud and immediate.
*   **Naming:** Clarity > Brevity. Booleans ask questions (`is_valid`, `has_access`).
*   **Structure:** Prefer early returns to deep nesting (Guard Clauses).
*   **Comments:** Explain *why*, not *what*. Document public APIs.

## 2. Interaction Format
*   **Tool-First:** Use tools to act. Do not ask the user to copy-paste.
*   **Atomic Changes:** Group file reads. Break down large writes into logical chunks.
*   **Evidence-Based:** Cite file:line when referencing code. Do not paraphrase from memory.

## 3. Output Guidelines
*   **Commands define their own output format.** Follow the format specified in each command prompt.
*   **Default:** Be concise but complete. Omit filler, include substance.
*   **Errors:** When something fails, state what failed, why, and what to do next.
