# macos-setup

Personal macOS setup and configuration.

This repository is designed to support **two different approaches** to setting up a Mac:

1. **State-based configuration (recommended)**
2. **Command-based setup (manual / documented)**

---

## Two Approaches to macOS Setup

### 1. State-Based Setup (Preferred)

This approach treats your system configuration as **state**:

👉 See full guide:  
[State-Based Setup](docs/setup/state-based.md)

---

### 2. Command-Based Setup

This approach documents setup as a sequence of **terminal commands**:
[Command-Based Setup](docs/setup/command-based.md)

---

## Repository Structure

```text
macos-setup/
├── dotfiles/        # Source-of-truth config files
├── install/         # Scripts to apply configuration
├── services/        # Automator workflows (UI layer)
├── scripts/         # Shell scripts (logic layer)
├── docs/            # Documentation and guides
└── bootstrap.sh     # Entry point for full setup
=======
Installed manually:

- Google Chrome (from website)
- Microsoft Word (from app store)
- Microsoft Excel (from app store)
- Microsoft PowerPoint (from app store)
- Microsoft OneNote (from app store)

---
