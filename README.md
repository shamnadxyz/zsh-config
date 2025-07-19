# My ZSH Config

- For Arch Linux

## Requirements

- [pkgfile](https://wiki.archlinux.org/title/Pkgfile)
- [sk](https://github.com/skim-rs/skim)
- [starship](https://github.com/starship/starship)
- [zoxide](https://github.com/ajeetdsouza/zoxide)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```sh
sudo pacman -S zsh fzf zsh-syntax-highlighting starship wl-clipboard \
    zoxide pkgfile --needed
```

## Instructions

Set $ZDOTDIR

Clone config

```sh
git clone --depth 1 https://github.com/shamnadxyz/zsh-config.git
```

- Copy .zshrc to $HOME directory

```sh
cp zsh-config/.zshrc ~/.zshrc
```

## Changing default shell to zsh

Locate zsh file path and append to /etc/shells

```sh
command -v zsh | sudo tee -a /etc/shells
```

Set ZSH as default

```sh
sudo chsh -s $(which zsh) $USER
```

Create Dirstack File

```sh
touch $HOME/.cache/dirs
```
