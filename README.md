## 🚀 Installation

### Shell Autocomplete

Install `inshellisense` globally using npm:

```bash
npm install -g @microsoft/inshellisense
```

To enable automatic startup of inshellisense in your shell sessions, run the appropriate command below based on your shell. This ensures inshellisense launches automatically in every new shell session:

```bash
# bash
is init bash >> ~/.bashrc

# zsh
is init zsh >> ~/.zshrc

# fish
is init fish >> ~/.config/fish/config.fish

# pwsh
is init pwsh | Add-Content $profile

# powershell
is init powershell | Add-Content $profile

# xonsh
is init xonsh >> ~/.xonshrc

# nushell
is init nu | save $nu.env-path --append
```
After running the appropriate command, restart your terminal or source the updated config file to apply the changes.

### Terminal Theme

### Installation manual for windows [here](https://ohmyposh.dev/docs/installation/windows)

![nordv1](https://github.com/user-attachments/assets/e00055d3-b51f-4a9a-b193-b8de575057e9)