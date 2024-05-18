# VIM Python IDE for Unix

## I want to configure Vim so that I can use it to develop python scripts. THis is what I have found.

## NOTE: this uses the color scheme solorized from https://ethanschoonover.com/solarized/
## your Terminal emulator should also be set to use this color scheme for this to look good! 

## NOTE: you must install the python package flake8 for code checking to work
``` python3 -m pip install flake8 ```

* Plug-in managers:
Vundle: https://github.com/VundleVim/Vundle.vim
    - Reqirements: git, curl

    - Instalation:
    git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

    - Configuration:

    edit ~/.vimrc as metioned in the README.md of Vundle. a copy is located here ./.vimrc
    Note: there is a Plugin for a local file install uncommented, it throws an error. I have comented it out.
    Note: when you run vim for the first time there will be erros as the plugins in the .vimrc file have not been installed. 
   run ```python3 test.py```
   in the vim editor window run ```:PluginInstall```
   this will install all the nesisary plugins.
   
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

    nerdtree-git-plugin:
        mark files in NERDTree with git symbols.
        
        Plugin 'Xuyuanp/nerdtree-git-plugin'
        Plugin 'ryanoasis/vim-devicons'

## USAGE
NERDTree: \<CR-n\> (ctrl + n) will bring up the tree in the left hand window

move between windows: \<CR-w\>\<CR-w\>  need to do it twice. 

Git: type :Git or :G and command. example: `:G status` 

- Other things to Explore:
    * netrw: https://www.vim.org/scripts/script.php?script_id=1075
