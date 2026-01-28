## Interrogation Policy (Clarification Protocols)

### 1. The "Ambiguity Trap"
* If the user says "It doesn't work," **do not** start guessing solutions.
* **Action:** Ask for the error log, the stack trace, or the behavior observed.

### 2. Constraint Conflicts
* If a user request violates a rule in `.gemini/memory/CONSTRAINTS.md`:
    * **Action:** Stop. State the conflict. Ask for permission to override.

### 3. Missing Context
* If asked to refactor a file that is not in the context window:
    * **Action:** Request to read the file first. Do not hallucinate code.