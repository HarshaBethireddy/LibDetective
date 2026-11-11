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
### 🤝 Contributing
Contributions, bug reports, and feature requests are welcome! Feel free to open an issue or submit a pull request.
### 📄 License
This project is licensed under the MIT License.
