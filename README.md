# macos-setup

Personal macOS setup and configuration.

This repository supports two different approaches to setting up a Mac:

1. **State-based configuration (recommended)**
2. **Command-based setup (manual / documented)**

---

## Two Approaches to macOS Setup

### 1. State-Based Setup (Preferred)

This approach treats your system configuration as **state**:
- Configuration is stored in files (dotfiles, scripts, workflows)
- The repository becomes the source of truth
- Setup is reproducible and version-controlled

👉 [View State-Based Setup](docs/setup/state-based.md)

---

### 2. Command-Based Setup

This approach documents setup as a sequence of **terminal commands**:
- Steps are executed manually
- Useful for learning and initial setup
- Less reproducible over time

👉 [View Command-Based Setup](docs/setup/command-based.md)

---

## Repository Structure

```text
macos-setup/
├── dotfiles/        # Source-of-truth configuration
├── install/         # Scripts that apply configuration
├── services/        # Automator workflows (UI layer)
├── scripts/         # Shell scripts (logic layer)
├── docs/            # Documentation
└── bootstrap.sh     # Entry point for full setup
```

