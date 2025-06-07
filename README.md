# 💻 Device Setup

This document outlines the setup process for my development and productivity environment across **macOS**, **Linux**, and **Windows**. It includes package installations, system configurations, and essential tools I use across devices.

---

## 🛠️ macOS Setup

### 1. Install Homebrew

Run the following command in your terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

After installation, configure the environment (example for `zsh`):

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

---

### 2. Install Packages with Homebrew

Use the following syntax:

```bash
brew install <formula_name>         # For CLI tools
brew install --cask <cask_name>     # For GUI applications
```

---

### ✅ Homebrew Formulae (CLI Tools)

```bash
brew install nvm    # Node Version Manager – manage multiple Node.js versions
brew install uv     # Rust-based Python Virutal ENV manager
brew install yarn   # JavaScript package manager
```

---

### ✅ Homebrew Casks (GUI Apps)

```bash
brew install --cask 1password
brew install --cask discord
brew install --cask font-jetbrains-mono
brew install --cask font-jetbrains-mono-nerd-font
brew install --cask ghostty
brew install --cask google-drive
brew install --cask librewolf --no-quarantine        # See note below
brew install --cask logi-options+
brew install --cask moonlight
brew install --cask steam
brew install --cask visual-studio-code
brew install --cask vlc
```

---

#### ⚠️ LibreWolf Special Note

LibreWolf is marked as "broken" on MacOS because [LibreWolf developers choose not to pay for an Apple Developer certificate](https://librewolf.net/docs/faq#why-is-librewolf-marked-as-broken). Use the `--no-quarantine` flag when installing.
