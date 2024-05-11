# My ZSH Config

- For Arch Linux

## Requirements
- [fzf](https://github.com/junegunn/fzf)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
- [starship](https://github.com/starship/starship)

## Instructions
Set $ZDOTDIR
```
echo 'export ZDOTDIR="$HOME/.config/zsh"' >> $HOME/.zprofile
```
Clone config
```
git clone --depth 1 https://codeberg.org/doesitmatter0/zsh-config.git ~/.config/zsh
```
- Run 'zsh' command and test basic commands to make sure zsh is working.

## Changing default shell to zsh
Locate zsh file path and append to /etc/shells
```
command -v zsh | sudo tee -a /etc/shells
```
Set ZSH as default
```
sudo chsh -s $(which zsh) $USER
```
