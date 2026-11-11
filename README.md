# 🔍 LibDetective

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Go Report Card](https://goreportcard.com/badge/github.com/HarshaBethireddy/LibDetective)](https://goreportcard.com/report/github.com/HarshaBethireddy/LibDetective)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A fast static analysis and AI-powered dependency discovery engine that extracts, identifies, and resolves third-party libraries across orphaned code snippets and legacy codebases.

---

## 📌 The Problem
Modern package managers (`go.mod`, `package.json`, `requirements.txt`) require pre-configured manifest files. However, developers and security auditors frequently encounter:
* Orphaned code snippets from legacy microservices and migration scripts.
* Code copied from documentation, community forums, or LLM completions without dependency metadata.
* Unmaintained repositories lacking clear dependency definitions.

**LibDetective** solves this by analyzing syntax trees and applying contextual inference to detect upstream libraries without requiring pre-existing package manifests.

---

## 🚀 Key Features

* **Static AST Extraction:** Rapidly scans source code to isolate import paths, external package references, and namespace declarations.
* **Contextual Heuristic & LLM Parsing:** Disambiguates ambiguous imports and resolves internal vs. third-party dependencies.
* **CLI-First Workflow:** Lightweight command-line utility built in Go with minimal runtime overhead.
* **Multi-Language Support (Roadmap):** Native support for Go syntax, with Python and Java scanners currently under development.

---

## 🛠️ Installation & Quick Start

### Prerequisites
* Go 1.21 or higher

### Build from Source
```bash
# Clone the repository
git clone https://github.com/HarshaBethireddy/LibDetective.git
cd LibDetective

# Download dependencies
go mod tidy

# Build binary
go build -o libdetective main.go
```

# Usage
Run LibDetective against any code file or directory:
Bash
# Analyze a specific source file
./libdetective scan --file=example.go

# Output detected dependencies in JSON format
./libdetective scan --file=example.go --format=json
🗺️ Roadmap

Initial Go AST parser integration

Heuristic dependency mapping engine

Multi-ecosystem resolution (PyPI, crates.io, pkg.go.dev)

Automated synthetic test suite generation

GitHub Actions CI scanner for pull requests
🤝 Contributing
Contributions, bug reports, and feature requests are welcome! Feel free to open an issue or submit a pull request.
📄 License
This project is licensed under the MIT License.
Code
4. Click the green **Commit changes...** button at the top right.
5. Select *"Commit directly to the `main` branch"* and click **Commit changes**.

---

### Step 3: Polish the "About" Section and Tags

GitHub tags help reviewers index what your project does at a glance:

1. Go back to the **main page** of `HarshaBethireddy/LibDetective`.
2. On the right-hand sidebar, find the **About** header and click the **gear icon (⚙️)**.
3. Update the fields:
   * **Description:**
     ```text
     Fast static analysis and AI-driven dependency discovery tool for source code snippets and legacy repositories.
     ```
   * **Topics (type each and press Enter):**
     * `golang`
     * `static-analysis`
     * `ast`
     * `developer-tools`
     * `code-analysis`
     * `dependency-scanner`
     * `open-source`
4. Click **Save changes**.

---

### Step 4: Verify Your Primary GitHub Email

Anthropic matches your application with your GitHub account:

1. Open [GitHub Email Settings](https://github.com/settings/emails).
2. Check which email is set as your **Primary** verified email.
3. Make sure you use **that exact email address** in the **Email\*** field of the Claude application form.

---

### What this accomplishes:
* Adds an **OSI-approved license (MIT)** (mandatory program requirement).
* Generates **fresh public commits** within the 90-day activity window.
* Presents an **architected, active developer tool** that justifies discretionary approval under Anthropic's Ecosystem Impact Track.
