# dev_env
i2sec Internal development environment

### Linux

* Ubuntu\Debian

```
$ sudo apt-get install git exuberant-ctags ncurses-term curl
```

* Gentoo
```
$ sudo emerge --ask dev-util/ctags sys-libs/ncurses dev-vcs/git dev-python/pyflakes net-misc/curl
```

* Arch Linux via *pacman* (recomend used *pacaur*)
```
$ sudo pacman -S git-core ctags ncurses curl
```
* Fedora

```
$ sudo dnf install ncurses-devel git ctags-etags curl
```

* openSUSE
```
$ sudo zypper in ncurses-devel git ctags curl
```

### Python bundle (optionally)

* pyflakes
* jedi
* neovim (neovim only) 

```
$ pip install flake8 jedi
$ pip2 install --user --upgrade neovim
$ pip3 install --user --upgrade neovim
```

## Installation

* Download your own vimrc file at http://www.vim-bootstrap.com
* Put your vimrc file into home folder or `$XDG_CONFIG_HOME/nvim/init.vim` if you use NeoVim

**vim:** `mv ~/Downloads/generate.vim ~/.vimrc`

**neovim:** `mv ~/Downloads/generate.vim $XDG_CONFIG_HOME/nvim/init.vim`

* Execute ViM and it will install plugins automatically
```
vim +PlugInstall +qall
```

### Updating to the latest version

    :VimBootstrapUpdate (thanks to @sherzberg)
    :PlugInstall
