# Because I need passwords

* install dropbox
* install 1Password
  * connect 1Password to Dropbox sync & wait for my passwords

# brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

# cask

```
brew tap caskroom/cask
brewk cask install google-chrome
brew cask install spotify
```

# base utils

```
brew install cmake
```

# git
```
brew install git
ssh-keygen -t rsa -b 4096 -C "robert.pankowecki@gmail.com"
eval "$(ssh-agent -s)"
# edit ~/.ssh/config => https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/
ssh-add -K ~/.ssh/id_rsa
pbcopy < ~/.ssh/id_rsa.pub
# add shh key to github and bitbucket

brew install gpg
# install keybase form https://keybase.io/docs/the_app/install_macos
brew install gpg-agent pinentry-mac
# setup gpg-agent as described https://gist.github.com/bmhatfield/cc21ec0a3a2df963bffa3c1f884b676b

brew install gist
gist login
```

# vim
```
brew install vim --with-lua --with-override-system-vi --with-python3
pip3 install --upgrade pip setuptools wheel
brew install neovim
pip2 install --user --upgrade neovim
pip3 install --user --upgrade neovim
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
vim +PluginInstall +qall
cd ~/.vim/bundle/YouCompleteMe && ./install.py --all
```

# dotfiles
```
git clone git@github.com:mpraglowski/dotfiles.git ~/dotfiles
cd ~/dotfiles
sh bootstrap.sh
```

# terminal
```
# download http://ethanschoonover.com/solarized
# download & install SourceCode Pro for Powerline from https://github.com/powerline/fonts
brew cask install iterm2
brew install tmux
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
tmux source ~/.tmux.conf
# install plugins https://github.com/tmux-plugins/tpm#installing-plugins
```

# moar utils
```
brew install make --with-default-names
brew install tree
brew install ack
brew install the_silver_searcher
brew install htop
brew install gnu-sed
brew install hh
```

# ruby
```
brew install rbenv
brew install heroku
brew install sqlite
```

# webdev
```
brew install yarn
brew install node@6
```

# databases
```
brew install mysql
brew services start mysql

brew install redis
brew services start redis

brew install postgres
brew services start postgres
```

# fish

```
brew install fish
brew install fzf

# https://github.com/fisherman/fisherman#install
fisher install fzf
```
