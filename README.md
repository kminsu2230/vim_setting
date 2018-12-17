### repo info

    개인적인 vim 세팅이다 

#### setup info

    파일을 받은 후 vim80_kms폴더를 vim80으로 수정 후 '/usr/share/vim/' 폴더에 넣기

	* vim80_ori는 오리지널 파일
    


#### version / OS

    8.0 / Mac

#### colorscheme : vim-monokai-tasty

    url : (https://github.com/patstockwell/vim-monokai-tasty)

#### content

    sublime3 와 유사한 세팅으로 함

#### set vim code

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   General Setting
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
 
    " Sets history line
    set history=500
 
    " Mapping <leader> => ,
    let mapleader=","
 
    " Show current position at bottom-right
    set ruler
    set lazyredraw
    set magic
 
    " Show matching brackets when text indicator is over them
    set showmatch

    " How many tenths of a second to blink when matching brackets
    set mat=2

    " Show line number
    set number

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   Search Setting
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

    " Ignore case when searching
    set ignorecase

    " Be smart when searching
    set smartcase

    " Highlight search last result
    set hlsearch

    " Move cursor when searching
    set incsearch

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   Color Setting
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

    " Syntax Enable
    syntax on

    colorscheme vim-monokai-tasty

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   Indent Setting
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

    " tab == 4 space
    set tabstop=4
    set shiftwidth=4
    set softtabstop=4

    " Using tab like 4 space
    set smarttab

    " Auto Indent
    set ai

    " Smart Indent
    set si

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   Key Mapping
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

    " ,vi =>  Show edit tab .vimrc
    nnoremap <leader>vi :tabe ~/.vimrc<CR>

    " ,src => Reload .vimrc
    nnoremap <leader>src :source ~/.vimrc<CR>

    " ,q => Quit
    map <leader>q <ESC><ESC>:q<CR>

    " F2 => Save File
    "imap <F2> <ESC><ESC>:w<CR>
    map <F2> <ESC><ESC>:w<CR>

    " F3 => Toggle line number

    map <F3> <ESC>:set nu! relativenumber!<CR>

    " jk => esc, Escape insert mode
    inoremap jk <ESC>

    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""
    "   Moving tab Setting
    """"""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""""

    map <C-j> <C-W>j
    map <C-k> <C-W>k
    map <C-h> <C-W>h
    map <C-l> <C-W>l  
