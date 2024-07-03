# My ZSH Config

## Requirements
- Debian-Based Linux Distribution
- [fzf](https://github.com/junegunn/fzf)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
```
sudo apt install fzf zsh-syntax-highlighting
```
## Instructions
Set $ZDOTDIR
```
echo 'export ZDOTDIR="$HOME/.config/zsh"' >> $HOME/.zprofile
```
Clone config
```
git clone --depth 1 https://codeberg.org/doesitmatter0/zsh-config.git -b debian ~/.config/zsh
```
## Changing default shell to zsh
Locate zsh file path and append to /etc/shells
```
command -v zsh | sudo tee -a /etc/shells
```
Set zsh as default
```
sudo chsh -s $(which zsh) $USER
```
