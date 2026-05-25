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
set number
set relativenumber
set scrolloff=8
set showcmd
set wildmenu
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

" === Keymaps ===
let mapleader = "\<Space>"
nnoremap <CR> :nohlsearch<CR>
nnoremap <Leader>t :lcd %:p:h \| :terminal<CR>
nnoremap <Leader>f :Ex<CR>
nnoremap <Leader>d "_d
nnoremap <C-h> <C-w>h
nnoremap <C-j> <C-w>j
nnoremap <C-k> <C-w>k
nnoremap <C-l> <C-w>l
tnoremap <C-h> <C-w>h
tnoremap <C-j> <C-w>j
tnoremap <C-k> <C-w>k
tnoremap <C-l> <C-w>l

" === Autocmd ===
autocmd BufWritePre * :%s/\(\S\)\s\+$/\1/e
```
