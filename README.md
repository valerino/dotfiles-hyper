# dotfiles-hyper
my dotfiles using [Hyper](https://hyper.is/) terminal, [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and [vimplug](https://github.com/junegunn/vim-plug)

__previous [dotfiles](https://github.com/valerino/dotfiles) are no more mantained !__

# prerequisites
* zsh as the default shell
* [Hyper](https://hyper.is/)
 
# pre-installation steps
* __IMPORTANT: use the default terminal for installation, not Hyper itself!
* __IMPORTANT: delete (making backups) of any existing ~/.zplug, ~/.vim, ~/.oh-my-zsh, ~/.hyper.js, ~/.vimrc, ~/.zshrc first, and restart the terminal__

# installation
* clone this repo
~~~
mkdir -p repos
cd repos
git clone https://github.com/valerino/dotfiles-hyper
~~~
* install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
* install [dracula theme for zsh](https://draculatheme.com/zsh/)
* symlink .zshrc, .vimrc and .hyper.js in your $HOME to the copies in this repo
~~~
# use my vimrc
ln -s /Users/valerino/repos/dotfiles-hyper/.vimrc ~/.vimrc

# delete the default .zshrc provided on installation of oh-my-zsh first, then use my zshrc
rm ~/.zshrc
ln -s /Users/valerino/repos/dotfiles-hyper/.zshrc ~/.zshrc

# use my hyper.js
ln -s /Users/valerino/repos/dotfiles-hyper/.hyper.js ~/.hyper.js
~~~
* restart Hyper, this will install plugins.
* vim plugins will be installed once in Vim.
* __profit! :)__ 

