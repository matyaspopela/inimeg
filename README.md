# 🚀 Gemini CLI Engineering Kit

A drop-in configuration suite that transforms the Gemini CLI into a specialized **Senior Software Engineering Partner**.

This kit provides a structured set of commands, roles, and memory files designed to enforce architectural standards, automate best practices (TDD, Auditing), and provide high-level mentorship.

---

## 📦 Installation & Setup

1.  **Drop it in:** Copy the `.gemini` folder into the root of your software project.
2.  **Initialize:** Open the Gemini CLI and run the setup command to scan your project and populate the context:
    ```bash
    /setrepo
    ```
    *This will auto-detect your frameworks (React, Django, etc.), project structure, and dependencies.*

---

## 🛠️ Command Suite

This kit comes with specialized agents activated by specific commands.

### 🧠 Strategic & Architectural
| Command | Role | Use Case |
| :--- | :--- | :--- |
| **`/plan <request>`** | **Technical Architect** | **Start here.** Analyzes requirements against your architecture. Generates specifications and execution plans *before* you write code. |
| **`/setrepo`** | **System Scanner** | Re-indexes the codebase. Run this when switching projects or after major file structure changes. |

### 💻 Development & Quality
| Command | Role | Use Case |
| :--- | :--- | :--- |
| **`/tdd <feature>`** | **TDD Specialist** | Implements features using the **Red-Green-Refactor** cycle. Writes tests first, then implementation, then optimizes. |
| **`/refactor`** | **Tech Debt Specialist** | Cleans up code, reduces complexity, and modernizes syntax *without* changing behavior. |

### 🛡️ Review & Security
| Command | Role | Use Case |
| :--- | :--- | :--- |
| **`/audit`** | **Security Auditor** | Performs a deep scan for OWASP vulnerabilities, anti-patterns, and architectural flaws. |
| **`/mentor`** | **Staff Engineer** | detailed code review focused on *teaching*. Explains the "why" behind best practices. |

---

## ⚙️ Configuration

The brain of the agent is located in `.gemini/`. You can customize it to fit your team's style.

### Core Files
*   **`.gemini/GEMINI.md`**: The "Master Prompt". Defines the agent's core directives and active rules.
*   **`.gemini/settings.json`**: Configures tool permissions and manually overrides project context (e.g., preferred frameworks).
*   **`.gemini/memory/CONSTRAINTS.md`**: **Critical.** Define your project's "Laws". (e.g., "Must use Postgres", "No raw SQL", "Deploy to Railway").

### Policies & Rules (`.gemini/rules/` & `.gemini/policy/`)
*   **`persona.md`**: Defines the agent's personality (currently set to "Senior Technical Consultant").
*   **`style.md`**: Coding standards (Naming conventions, KISS, YAGNI).
*   **`risk.md`**: Safety protocols (Forbidden commands, secret handling).

---

## 🧩 Workflow Example

1.  **Idea:** You want to add a new user profile page.
2.  **Plan:** Run `/plan "Add user profile page with avatar upload"`.
    *   *Result:* Agent checks `CONSTRAINTS.md`, drafts a spec file, and lists necessary tests.
3.  **Code:** Run `/tdd "Implement user profile model and view based on the plan"`.
    *   *Result:* Agent writes a failing test, implements the model, and passes the test.
4.  **Review:** Run `/audit` on the new file.
    *   *Result:* Agent checks for file upload vulnerabilities and permission issues.

---

## 🤝 Contributing

Feel free to modify the `.toml` files in `.gemini/commands/` to create your own specialized agents!
