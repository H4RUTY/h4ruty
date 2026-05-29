here is my `.vimrc`:

```vim
" === General ===
set encoding=utf-8
set noswapfile
set nobackup
set autoread
set undofile
set undodir=~/.vim/undo
set clipboard=unnamed

" === UI ===
syntax on
colo sorbet
set number
set relativenumber
set scrolloff=8
set showcmd
set wildmenu
set nowrap
set laststatus=2
set list
set listchars=tab:»\ ,trail:·
set splitright
set splitbelow
let g:netrw_banner = 0

" === Indent ===
set tabstop=4
set shiftwidth=4
set expandtab
set smartindent

" === Search ===
set ignorecase
set smartcase
set hlsearch
set incsearch

" === Remaps ===
let mapleader = "\<Space>"
nnoremap <Leader><CR> :nohlsearch<CR>
nnoremap <Leader>t :lcd %:p:h \| :terminal<CR>
nnoremap <Leader>f :Ex<CR>
nnoremap <Leader>d "_d

" === Autocmd ===
autocmd BufWritePre * :%s/\(\S\)\s\+$/\1/e
```
