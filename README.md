# dotfiles

### Setup:

* zsh
    * install zsh

            yay -S zsh

    * install oh-my-zsh 

            sh -c "$(curl https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

    * install zsh-syntax-highlighting

            git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $CONF/zsh/oh-my-zsh/plugins/zsh-syntax-highlighting

* tmux
    * install tmux
    
            yay -S tmux 
    
    * install tmux package manager via

            git clone https://github.com/tmux-plugins/tpm $CONF/tmux/plugins/tpm

    * install plugins with 

            prefix + I

* vim
    * install vimplug (this should be done automatically at vim startup) via

            curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
            https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

    * install all other plugins with

            :PlugInstall 

    * make vim bin scripts executable
    
            chmod +x ./nvim/bin/*
        
    * install python requirements
    
            pip3 install ./nvim/requirements.txt 
        
    * install tasklib for taskwiki

            cd ./nvim/plugged/taskwiki
            pip3 install -r requirements

* x server
    * on manjaro
        * source ./x/xinitrc from /etc/xdg/xfce4/xinitrc
    * if not yet installed: install xcompmgr
    * create symlink from home dir into config repo
    
            ln -s $CONF/x/

* dwm 
    * download & compile from source
    
            git clone https://git.suckless.org/dwm
    
    * install patches
        * bar-height
        * bottomstack
        * centretitle
        * combo
        * fibonacci
        * uselessgap

* st 
    * download & compile from source

            git clone https://git.suckless.org/st

    * install patches
        * alpha
        * anygeometry
        * anysize
        * clipboard
        * vimBrowse ?

* ranger
    * download devicons
    * download image preview package

* tex
    * on manjaro
        * install texlive-most
    * on mac
        * install macTex
    * install latex-mk (for vimtex)

* other packages (e.g. from AUR, npm, pip or homebrew)
    * AUR
        * task, tasksh, timew
        * lsd
        * fzf
        * ripgrep (rg), needed for fzf-preview
        * top/gtop
        * neomutt
        * ytdl, rtv
        * colordiff
        * colorpicker
        * ncdu, tldr
        * sl, cmatrix, cowsay, fortune
        * xclip, xsel ? x... ?
    * npm
        * weather-cli, nasa-cli
        * cli-fireplace, carbon-now-cli
        * emoji-finder
    * pip3
        * ricksay, YuleLog
    * various / as of yet uncategorized
        * dropbox
        * pipes.sh
        * s (search)
        * mdv (markdown viewer)
        * pass (pw manager)
        * sxiv
        * bpython, mycli
