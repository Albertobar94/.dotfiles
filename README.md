# dotfiles

My dev environment setup files

# Font

- [Anonymous Pro](https://www.marksimonson.com/fonts/view/anonymous-pro)

# Setup

Create `apps.txt` file:

```sh
slack
discord
figma
spotify
android-platform-tools
android-file-transfer
vlc
keka
kap
keycastr
iterm2
visual-studio-code
sublime-text
```

Install Apps:

```sh
xargs brew install < apps.txt
```

Create cli-pps file:

```sh
ffmpeg
imagemagick
wget
telnet
tldr
```

Install Cli Apps:

```sh
xargs brew install < apps.txt
```

Install github cli:

```bash
brew install gh
```

Install vscode extentions:

```sh
cat extensions.txt | xargs -L1 code --install-extension
```

# Install Oh my ZSH.

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

# Install P10k

- Go to [P10k Website](https://github.com/romkatv/powerlevel10k#installation)

# Install Zsh plugins.

autosuggesions plugin:
```sh
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

zsh-syntax-highlighting plugin:
```sh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

zsh-fast-syntax-highlighting plugin:
```sh
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```

zsh-autocomplete plugin:
```sh
git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```

### Enable plugins by adding them to .zshrc.

- Open .zshrc: 

```sh
code ~/.zshrc
```

- Find the line which says 

```sh
plugins=(git)
```

- Replace that line with
```sh
plugins=(git zsh-autosuggestions zsh-syntax-highlighting fast-syntax-highlighting zsh-autocomplete)
```
### References

- [Oh my ZSH](https://github.com/ohmyzsh/ohmyzsh)
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
- [zsh-fast-syntax-highlighting](https://github.com/zdharma/fast-syntax-highlighting)
- [zsh-autocomplete](https://github.com/marlonrichert/zsh-autocomplete)

# TODO
- document the rest
- [check dotfiles example repo](https://github.com/WilliamFernsCodes/.dotfiles/blob/main/README.md)
- [check CJ's repo](https://github.com/CodingGarden/mac-setup)