## 📚 Table of Contents

- [🚀 Installation Guide](#-installation-guide)
  - [⚙️ Shell Autocomplete Setup](#️-shell-autocomplete-setup)
  - [🎨 Terminal Theme Setup (PowerShell)](#-terminal-theme-setup-powershell)
  - [🛠 VS Code Configuration](#-vscode-configuration)

## 🚀 Installation Guide

### ⚙️ Shell Autocomplete Setup

Install `inshellisense` globally using npm:

```bash
npm install -g @microsoft/inshellisense
```

To enable automatic startup of inshellisense in your shell sessions, run the appropriate command below based on your shell. This ensures inshellisense launches automatically in every new shell session:

```bash
# bash
is init bash >> ~/.bashrc

# pwsh
is init pwsh | Add-Content $profile

# powershell
is init powershell | Add-Content $profile
```

After running the appropriate command, restart your terminal or source the updated config file to apply

---

### 🎨 Terminal Theme Setup (PowerShell)

1. Install [FiraCode Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.4.0/FiraCode.zip)

2. Open PowerShell and install Oh My Posh using winget: (Make sure `winget` is installed):

```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```

3. Open your PowerShell profile in Notepad (or any text editor):

```powershell
notepad $PROFILE
```

4. Add the following line to the end of your profile script:

```powershell
oh-my-posh init pwsh --config "https://raw.githubusercontent.com/sapondanaisriwan/beautiful-terminal/refs/heads/main/adashima.omp.json" | Invoke-Expression
```

5. Once added, reload your profile for the changes to take effect.

```powershell
. $PROFILE
```

---

### 🛠 VSCode Configuration

1. Open Visual Studio Code.

2. Press `Ctrl + Shift + P` and type "Open User Settings (JSON)" and select it.

3. Add the following lines inside the JSON object:

```json
{
  // Sets PowerShell as the default terminal
  "terminal.integrated.defaultProfile.windows": "PowerShell",
  // Sets the font used in the code editor to "FiraCode Nerd Font".
  "editor.fontFamily": "FiraCode Nerd Font",
  // Sets the font used in the integrated terminal to "FiraCode Nerd Font".
  "terminal.integrated.fontFamily": "FiraCode Nerd Font"
}
```
