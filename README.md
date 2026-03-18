# macos-setup

Personal macOS setup and configuration.

This repository is designed to support **two different approaches** to setting up a Mac:

1. **State-based configuration (recommended)**
2. **Command-based setup (manual / documented)**

---

## Two Approaches to macOS Setup

### 1. State-Based Setup (Preferred)

This approach treats your system configuration as **state**:

- Configuration is stored in files (dotfiles, scripts, workflows)
- The repository is the **source of truth**
- Setup is applied via install/bootstrap scripts
- Changes are version-controlled and reproducible

Examples:
- `.gitconfig`
- `.zshrc`
- Automator workflows
- Shell scripts

👉 See full guide:  
[State-Based Setup](docs/setup/state-based.md)

---

### 2. Command-Based Setup

This approach documents setup as a sequence of **terminal commands**:

<<<<<<< HEAD
- Manual execution of setup steps
- Useful for understanding and bootstrapping
- Less reproducible over time
- Harder to maintain consistency across machines

Examples:
- `git config --global ...`
- `ssh-keygen`
- manual app installs

👉 See full guide:  
[Command-Based Setup](docs/setup/command-based.md)
=======
- Set up as a new device
- Log in to Apple account
- Connect to wifi
- Set local user (e.g., `your-username`)
- Disable analytics and data sharing (no crash reporting, no system analytics)
>>>>>>> cd85311cd21774a1b5a5dfc566841c400d27dad1

---

## Repository Structure

<<<<<<< HEAD
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
