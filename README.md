# dotfiles

Setup:
   
* dwm 
    * install patches
        * fibonacci

* oh-my-zsh
    * install oh-my-zsh 
        sh -c "$(curl https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    * install zsh-syntax-highlighting
        git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
    
* ranger
    download devicons & image preview package

* tmux
    * install tmux package manager via
        git clone https://github.com/tmux-plugins/tpm $CONF/tmux/plugins/tpm
    * install plugins with 
        prefix + I

* st 
    * install patches
    
* vim
    * install vimplug (this should be done automatically at vim startup) via
        curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
        https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
    * install all other plugins with
        :PlugInstall 

    * other packages (e.g. from AUR or homebrew)
        * lsd
        * fzf
        * top/gtop
        * ...
        * sl, cmatrix, cowsay, fortune, ytdl
