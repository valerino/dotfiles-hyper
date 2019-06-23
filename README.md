# dotfiles-hyper
my dotfiles using [Hyper](https://hyper.is/) terminal, [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and [vimplug](https://github.com/junegunn/vim-plug)

__previous [dotfiles](https://github.com/valerino/dotfiles) are no more mantained !__

## prerequisites
* install zsh as the default shell
* install [Hyper](https://hyper.is/)
 
## pre-installation steps
* __use the default terminal for installation, not Hyper itself!__
* __delete (making backups if you need some special settings to reapply) of any existing ~/.zplug, ~/.vim, ~/.oh-my-zsh, ~/.hyper.js, ~/.vimrc, ~/.zshrc first, and restart the terminal__

## installation
~~~
# clone this repo somewhere
mkdir -p /Users/valerino/repos
cd /Users/valerino/repos
git clone https://github.com/valerino/dotfiles-hyper
~~~

* install [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
* install [dracula theme for zsh](https://draculatheme.com/zsh/)
* restart the terminal so it uses oh-my-zsh

### install zsh plugins (_optional_)
~~~
# install zsh autocompletion plugin into oh-my-zsh
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

# install zsh syntax-highlighting plugin into oh-my-zsh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
~~~

## use my provided configurations for zsh, vim, hyper
~~~
# symlink my .vimrc
ln -s /Users/valerino/repos/dotfiles-hyper/.vimrc ~/.vimrc

# delete the default .zshrc provided on installation of oh-my-zsh first
rm ~/.zshrc

# symlink my .zshrc (NOTE: *only* if you haven't installed the above zsh plugins, you may edit it first to remove them from oh-my-zsh plugins section)
ln -s /Users/valerino/repos/dotfiles-hyper/.zshrc ~/.zshrc

# symlink my .hyper.js
ln -s /Users/valerino/repos/dotfiles-hyper/.hyper.js ~/.hyper.js
~~~

## done!
* restart Hyper, this will install Hyper plugins. 
* vim plugins will be installed once starting vim.
* __profit! :)__ 

