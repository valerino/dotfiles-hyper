# dotfiles-hyper
my dotfiles using [Hyper](https://hyper.is/) terminal, [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and [vimplug](https://github.com/junegunn/vim-plug)

__previous [dotfiles](https://github.com/valerino/dotfiles) are no more mantained !__

# prerequisites
. zsh as the default shell
. [Hyper](https://hyper.is/)
 
# installation
. clone this repo
~~~
mkdir -p repos
cd repos
git clone https://github.com/valerino/dotfiles-hyper
~~~

. install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
. install [dracula theme for zsh](https://draculatheme.com/zsh/)
. symlink .zshrc, .vimrc and .hyper.js in your $HOME to the copies in this repo
~~~
ln -s /Users/valerino/repos/dotfiles-hyper/.vimrc ~/.vimrc
ln -s /Users/valerino/repos/dotfiles-hyper/.zshrc ~/.vimrc

# this must be done with Hyper closed, since it locks the configuration file
ln -s /Users/valerino/repos/dotfiles-hyper/.hyper.js ~/.hyper.js
~~~
. restart Hyper
. once in Vim, issue _PlugInstall_ to install the vim plugins
. __enjoy!__


