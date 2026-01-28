<div align="center">

<!-- Header with gradient border and dark theme -->
<img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/main/icons/gemini.svg" width="120" height="120" alt="Gemini CLI">

<h1 style="margin-top: 20px; font-size: 3em; font-weight: 800; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">
Gemini CLI: Engineering Excellence Kit
</h1>

<p style="font-size: 1.2em; color: #64748b; max-width: 600px; margin: 20px auto;">
A configuration suite that transforms the Gemini CLI into a <strong>Principal Technical Consultant</strong>, enforcing architectural rigor and automating quality assurance.
</p>

<p>
  <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" alt="MIT License">
  <img src="https://img.shields.io/badge/Status-Production%20Ready-success.svg?style=for-the-badge" alt="Production Ready">
  <img src="https://img.shields.io/badge/Type-Configuration%20Kit-orange.svg?style=for-the-badge" alt="Configuration Kit">
</p>

---

</div>

<br>

## ✨ What It Does

<table>
<tr>
<td width="50%">

### 🛡️ **Governance First**
Implements a strict "No Code Without Specs" policy. Every feature starts with architecture planning, ensuring decisions are documented before implementation.

### 🧪 **TDD Automation**
Built-in Red-Green-Refactor cycles for Django and React. Automated test generation and execution keep quality high and regressions low.

### 🔍 **Deep Auditing**
Specialized agents perform security, performance, and style reviews with surgical precision—catching issues before they reach production.

</td>
<td width="50%">

### 🧠 **Persistent Memory**
Multi-layered memory system tracks architecture decisions, technical constraints, and past failures to prevent repeated mistakes.

### 🏫 **Integrated Mentorship**
Reviews don't just fix code—they explain the "why" behind best practices, elevating your entire team's technical understanding.

### ⚡ **Intelligent Caching**
Auto-detects frameworks, entry points, and dependencies to build a real-time map of your codebase for faster, smarter suggestions.

</td>
</tr>
</table>

<br>

---

<br>

## 🚀 Quick Start

<details open>
<summary><strong>1. Installation</strong></summary>

<br>

Clone this kit or copy the `.gemini/` folder into your project root:

```bash
git clone https://github.com/your-username/gemini-engineering-kit.git
cp -r gemini-engineering-kit/.gemini /your/project/path/
```

</details>

<details open>
<summary><strong>2. Initialization</strong></summary>

<br>

Launch the Gemini CLI in your project root and trigger the re-indexing command:

```bash
/setrepo
```

This command performs a deep scan of your codebase, auto-detecting frameworks, entry points, and dependencies to populate the internal knowledge cache.

</details>

<br>

---

<br>

## 🛠️ The Command Suite

Each command activates a specialized agent with a focused mission:

<table>
<thead>
<tr>
<th width="15%">Command</th>
<th width="20%">Specialized Agent</th>
<th width="65%">Mission</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>/plan</code></td>
<td><strong>Architect</strong></td>
<td>Requirements analysis & technical specification generation. <em>Run this before coding!</em></td>
</tr>
<tr>
<td><code>/tdd</code></td>
<td><strong>Engineer</strong></td>
<td>Test-Driven Development cycles (Red-Green-Refactor) with automated test generation.</td>
</tr>
<tr>
<td><code>/audit</code></td>
<td><strong>Auditor</strong></td>
<td>Deep-dive security, architecture, and code quality reviews with actionable findings.</td>
</tr>
<tr>
<td><code>/refactor</code></td>
<td><strong>Specialist</strong></td>
<td>Code modernization and complexity reduction while preserving functionality.</td>
</tr>
<tr>
<td><code>/mentor</code></td>
<td><strong>Staff Lead</strong></td>
<td>Educational reviews focused on senior-level principles (SOLID, DRY, design patterns).</td>
</tr>
<tr>
<td><code>/docit</code></td>
<td><strong>Historian</strong></td>
<td>Synchronizes code changes with system documentation and architectural records.</td>
</tr>
</tbody>
</table>

<br>

---

<br>

## 🏗️ System Architecture

The kit organizes the agent's knowledge into three distinct layers:

<br>

<table>
<tr>
<td width="33%" valign="top">

### 📋 **Directives**
`.gemini/rules/` & `.gemini/policy/`

The foundational "Laws of Behavior":
- **Zero Clutter Protocol**: Keep suggestions focused and actionable
- **Interrogation Protocols**: Ask for logs instead of guessing
- **Security Hygiene**: Enforce secure coding standards

</td>
<td width="33%" valign="top">

### 🧠 **Memory**
`.gemini/memory/`

Living documentation that evolves with your project:
- **ARCHITECTURE.md**: Source of truth for system design
- **CONSTRAINTS.md**: Hard guardrails (languages, frameworks, databases)
- **FAILURES.md**: Learning journal of past technical mistakes

</td>
<td width="33%" valign="top">

### 💾 **Cache**
`.gemini/cache/`

Transient data generated by `/setrepo`:
- Real-time codebase symbol map
- Entry point detection
- Dependency graph
- Framework configuration

</td>
</tr>
</table>

<br>

---

<br>

## ⚙️ Customization

<details>
<summary><strong>1. Define Your Constraints</strong></summary>

<br>

Update `.gemini/memory/CONSTRAINTS.md` with project-specific rules:

```markdown
## Hard Constraints
- Must use TypeScript (no JavaScript)
- Postgres-only (no other databases)
- All API endpoints must be versioned
- Maximum function complexity: 10 cyclomatic
```

</details>

<details>
<summary><strong>2. Set the Persona</strong></summary>

<br>

Modify `.gemini/rules/persona.md` to adjust the tone:

```markdown
# Persona: Senior Staff Engineer

Tone: Direct, technical, assumes high competence
Communication: Focus on trade-offs and second-order effects
Teaching: Socratic method—ask questions before providing answers
```

</details>

<details>
<summary><strong>3. Add Custom Commands</strong></summary>

<br>

Drop new `.toml` files into `.gemini/commands/` to create specialized agents:

```toml
[command]
name = "deploy"
agent = "DevOps Lead"
mission = "Pre-deployment checklist and infrastructure validation"
context = ["ARCHITECTURE.md", "deployment/*.yaml"]
```

</details>

<br>

---

<br>

<div align="center">

## 🎯 Design Philosophy

> **"Fail fast in planning, succeed confidently in execution."**

This kit enforces architectural discipline without sacrificing speed. Front-load design decisions, automate quality checks, and maintain documentation as you build.

<br>

### Core Principles

**Specification Before Implementation** • **Test Before Code** • **Review Before Merge** • **Document As You Build**

<br>

---

<br>

## 📄 License

Released under the **MIT License** — free to use, modify, and distribute.

<br>

<sub>For teams that care about code quality.</sub>

</div>
