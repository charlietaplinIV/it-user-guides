# Contributing to IT User Guides

Thank you for your interest in improving these user guides! This document explains how to submit new content, fixes, or enhancements.

---

## 1. Getting Started

1. Fork this repository  
2. Clone your fork locally  
   ```bash
   git clone https://github.com/your-username/it-user-guides.git
    ```
3. Create a feature branch

git checkout -b feature/my-new-guide

---

## 2. Adding or Updating a Guide
- Add your Markdown file under guides/, following the naming pattern:
<topic-name>.md
- Use lowercase and hyphens (e.g., vpn-access.md).
- Add any screenshots or diagrams under assets/screenshots/ or assets/diagrams/.
- Update SUMMARY.md to include your new guide with a one-sentence description.
- If you modify repository structure or tooling, update README.md accordingly.

---

## 3. Style Guidelines
- Use UTF-8 encoding and Unix line endings (LF).
- Write clear step-by-step instructions with numbered lists.
- Include screenshots with descriptive alt text.
- Use fenced code blocks for commands:
ping 8.8.8.8 -n 4
- Keep paragraphs under 120 characters per line.
- Reference images with relative paths

---

## 4. Pull Request Process
- Push your branch to your fork
git push origin feature/my-new-guide
- Open a Pull Request against main in this repo
- Describe your changes clearly in the PR description
- Wait for review and respond to any feedback
- Once approved, your PR will be merged

---

## 5. Reporting Issues
If you find bugs or outdated instructions, please open an issue with:
- A clear title
- Steps to reproduce or observe the problem
- Affected guide or file path

Thank you for helping make these guides better! 🎉


