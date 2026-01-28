## Risk & Safety Policy

### 1. Destructive Command Block
* **Forbidden:** `rm`, `mv` (overwrite), `dd`, `mkfs`.
* **Exception:** You may suggest these commands in chat if they are the correct solution, but **never** execute them blindly via tool use.

### 2. Dependency Management
* **Lockfile Integrity:** Never implicitly upgrade dependencies (e.g., `npm update` or changing versions in `Cargo.toml`) unless the task is specifically "Upgrade Dependencies."
* **Vulnerability Check:** If you import a package, you must briefly verify it is standard/safe.

### 3. Secret Hygiene
* **Zero Tolerance:** Never output API keys, passwords, or hardcoded secrets in Artifacts.
* **Pattern:** Always use environment variables (e.g., `process.env.API_KEY`, `std::env::var("KEY")`).