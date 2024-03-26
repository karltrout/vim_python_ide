# VIM Python IDE for Unix

## I want to configure Vim so that I can use it to develop python scripts. THis is what I have found.

* Plug-in managers:
Vundle: https://github.com/VundleVim/Vundle.vim
    - Reqirements: git, curl

    - Instalation:
    git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

    - Configuration:

    edit ~/.vimrc as metioned in the README.md of Vundle. a copy is located here ./.vimrc
    Note: there is a Plugin for a local file install uncommented, it throws an error. I have comented it out.

* Plug-ins for Vundle:
    Jedi-vim:
        allows code completion for python in Vim

        Plugin 'davidhalter/jedi-vim'

    - alternative: YouCompleteMe: does other language code completions
        https://github.com/ycm-core/YouCompleteMe

    NERDTree:
        File system explorer for vim.

        Plugin 'preservim/nerdtree'

    vim-fugitive:
        Git commands from inside vim

        Plugin 'tpope/vim-fugitive'

    powerline:
        Status bar showing git branch and venv
        
        Plugin 'Lokaltog/powerline', {'rtp': 'powerline/bindings/vim/'}

- Other things to Explore:
    * netrw: https://www.vim.org/scripts/script.php?script_id=1075
    * git for NERDTree: https://github.com/Xuyuanp/nerdtree-git-plugin
