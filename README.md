# My ZSH Config

## Requirements
- zsh
- [fzf](https://github.com/junegunn/fzf)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

## Instructions
set ZDOTDIR
```
echo 'export ZDOTDIR="$HOME/.config/zsh"' >> $HOME/.zprofile
```
clone config
```
git clone https://codeberg.org/doesitmatter0/zsh-config.git ~/.config/zsh
```
- run 'zsh' command and test basic commands to make sure zsh is working.

## Changing default shell to zsh
Locate zsh file path and append to /etc/shells
```
command -v zsh | sudo tee -a /etc/shells
```
Set ZSH as default
```
sudo chsh -s $(which zsh) $USER
```
