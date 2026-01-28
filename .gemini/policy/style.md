# Engineering Standards & Style Guide

> **Core Philosophy:** "Code is read 10x more than it is written. Optimize for the reader, not the writer."

## 1. Universal Principles
* **KISS (Keep It Simple, Stupid):** Complexity is a liability. If a junior developer cannot understand your code in 5 minutes, rewrite it.
* **YAGNI (You Ain't Gonna Need It):** Do not implement features "just in case." Build for today's requirements only.
* **Fail Fast:** Errors should happen loudly and immediately at the source, not silently propagate to cause weird behavior later.

## 2. Naming Conventions
* **Clarity > Brevity:**
    * *Bad:* `u`, `dt`, `f()`
    * *Good:* `user`, `datetime_iso`, `fetch_user_data()`
* **Boolean Predicates:** Variables holding boolean values must imply a question.
    * Use prefixes: `is_`, `has_`, `should_`, `can_` (e.g., `is_valid`, `has_access`).
* **Constants:** Use `SCREAMING_SNAKE_CASE` for fixed configuration values.

## 3. Code Structure & Flow
* **Early Returns:** Avoid deep nesting (arrow code). Check for failure conditions first and return immediately.
    ```text
    // Bad
    if (user) {
        if (valid) {
            save();
        }
    }
    // Good
    if (!user || !valid) return;
    save();
    ```
* **Function Size:** A function should do **one** thing. If you need `and` in the function name, it is likely doing too much.
* **Magic Numbers:** No raw numbers or strings in logic. Extract them to named constants or configuration.

## 4. Documentation & Comments
* **The "Why" Rule:** Comments must explain *why* code exists (business logic, workarounds), not *what* the syntax is doing.
* **Public API:** Any function or class accessible outside its module must have a docstring/summary.
* **TODOs:** Do not leave empty TODOs. They must include context or an owner: `TODO(fix): Handle edge case X`.
