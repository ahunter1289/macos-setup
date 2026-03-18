# macos-setup

Personal macOS setup and configuration for a new machine.

This repository documents the baseline steps used to initialize a new MacBook and will evolve into a fully reproducible system setup (dotfiles, scripts, Automator workflows, etc.).

---

## Overview

This setup covers:

- Initial macOS configuration
- Core application installs
- Developer tooling (Xcode Command Line Tools)
- Git configuration
- SSH setup for GitHub

---

## Initial macOS Configuration

On first boot:

- Set up as a new device
- Log in to Apple account
- Connect to wifi
- Set local user (e.g., `your-username`)
- Disable analytics and data sharing (no crash reporting, no system analytics)

---

## Applications

Installed manually:

- Google Chrome (from website)
- Microsoft Word (from app store)
- Microsoft Excel (from app store)
- Microsoft PowerPoint (from app store)
- Microsoft OneNote (from app store)

---

## Developer Environment

### Xcode Command Line Tools

Installed via:

```bash
xcode-select --install
```

Provides Git, Clang, and core developer utilities.

---

### Git Configuration

Configured globally with:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
git config --global init.defaultBranch main
git config --global color.ui auto
git config --global pull.rebase false
```

This sets identity, default branch, CLI behavior, and pull strategy.

---

### SSH Setup (GitHub)

SSH is used for authentication instead of HTTPS.

Steps:

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
eval "$(ssh-agent -s)"
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
pbcopy < ~/.ssh/id_ed25519.pub
```

- Add the copied key to GitHub (Settings → SSH keys)
- Test connection:

```bash
ssh -T git@github.com
```

Expected result:

```
Hi <username>! You've successfully authenticated, but GitHub does not provide shell access.
```

---

### Git Remote Configuration

Repositories use SSH:

```bash
git@github.com:YOUR-USERNAME/repo-name.git
```

Example:

```bash
git remote set-url origin git@github.com:YOUR-USERNAME/macos-setup.git
```

---

## Repository Initialization

Projects are created under:

```bash
~/code/
```

Typical workflow:

```bash
mkdir -p ~/code/project-name
cd ~/code/project-name
git init
```

---

## Philosophy

- Reproducible setup
- Source-controlled configuration
- Separation of concerns:
  - Automator workflows → UI triggers
  - Shell scripts → logic
- SSH-first Git workflow

---

## Future Work

- Dotfile management (`.gitconfig`, `.zshrc`, etc.)
- Automator workflows + shell scripts
- Bootstrap/install scripts
- Homebrew package management

---

## Notes

- Moving from manual commands → managed configuration files
- This repository is the source of truth for system setup
