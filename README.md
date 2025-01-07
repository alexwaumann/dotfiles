# Dotfiles

## Theme

- [catppuccin for alacritty](https://github.com/catppuccin/alacritty)
- [catppuccin for tmux](https://github.com/catppuccin/tmux)

## Dependencies

- [brew](https://brew.sh/)
- [alacritty](https://alacritty.org/)
- [zsh](https://zsh.sourceforge.io/)
- [zplug](https://github.com/zplug/zplug)
- [starship](https://starship.rs/config/)
- [tmux](https://github.com/tmux/tmux/wiki)
- [tpm](https://github.com/tmux-plugins/tpm)
- [git](https://git-scm.com/book/be/v2/Customizing-Git-Git-Configuration)
- [cargo](https://doc.rust-lang.org/cargo/)
- [fnm](https://github.com/Schniz/fnm)
- [python](https://www.python.org/)
- [pipenv](https://pipenv.pypa.io/en/latest/)
- [neovim](https://neovim.io/)
- [bat](https://github.com/sharkdp/bat)
- [fzf](https://github.com/junegunn/fzf)
- [font-sauce-code-pro-nerd-font](https://www.nerdfonts.com/font-downloads)

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
curl https://sh.rustup.rs -sSf | sh
brew install --cask alacritty font-sauce-code-pro-nerd-font
brew install zsh zplug starship tmux tpm git fnm python pipenv neovim bat fzf

fnm install 23

git config --global user.name "name"
git config --global user.email email
git config --global core.editor nvim
git config --global core.pager bat
git config --global core.excludesfile ~/.gitignore_global
git config --global init.defaultBranch main
```

## Optional Dependencies

- [eza](https://github.com/eza-community/eza)
- [fd](https://github.com/sharkdp/fd)
- [gh](https://cli.github.com/)
- [htop](https://htop.dev/)
- [jq](https://jqlang.github.io/jq/manual/)
- [ripgrep](https://github.com/BurntSushi/ripgrep)
- [tldr](https://github.com/tldr-pages/tldr)
- [tree](https://github.com/kddnewton/tree)
- [wget](https://www.gnu.org/software/wget/)

```
brew install eza fd gh htop jq ripgrep tldr tree wget
```

## Other Programs

```
brew install --cask alfred discord google-chrome obsidian spotify
```

## Setup

```
cd && mkdir projects && cd projects

git clone git@github.com:alexwaumann/dotfiles.git
cd dotfiles

source zsh/zshenv
ln -sf ~/projects/dotfiles/zsh/zshrc ~/.zshrc
ln -sf ~/projects/dotfiles/zsh/zshenv ~/.zshenv
ln -sf ~/projects/dotfiles/zsh/zprofile ~/.zprofile
ln -sf ~/projects/dotfiles/tmux.conf ~/.tmux.conf
ln -sf ~/projects/dotfiles/alacritty ~/.config/alacritty
```

## Neovim

Neovim config is managed [here](https://github.com/alexwaumann/nvim).
