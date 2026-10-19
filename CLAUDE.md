# Artifact 03 Architecture & AI Model Boundaries

## System Architecture
This artifact implements an automated workflow pipeline delegating codebase security auditing and hygiene analysis to an active LLM agent loop using headless Claude Code (`claude -p`).

### 1. Plain Code Responsibilities
- **Cryptographic Randomness:** Generates password strings using `window.crypto.getRandomValues()` in the client-side UI.
- **Pipeline Orchestration:** Executes repository file discovery and manages execution status codes.
- **UI State & Layout:** Renders real-time interactive controls, clipboard utilities, and dark-mode styling via Tailwind CSS.

### 2. Model / AI Responsibilities (`claude -p`)
- **Codebase Comprehension:** Reads repository files and configuration scripts autonomously.
- **Security Reasoning & Decision Making:** Evaluates patterns for vulnerabilities, hardcoded secret leaks, or weak cryptographic hygiene.
- **Report Synthesis:** Writes structured qualitative security assessments and recommendations directly to project reports.