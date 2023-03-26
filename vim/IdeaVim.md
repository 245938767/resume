# 我Idea中Vim的配置

```vimrc

let mapleader=' '
set clipboard+=unnamed

" 插件
set surround
set easymotion
set NERDTree

" 相对行号
set relativenumber
set number

" 设置在状态栏显示按键
set showcmd

" 不要使用vi的键盘模式，而是vim自己的
set nocompatible

" 输入法
:set keep-english-in-normal
:set keep-english-in-normal-and-restore-in-insert
set keep-english-in-normal[-and-restore-in-insert]


inoremap jj <Esc>
noremap <C-j> 4j
noremap <C-k> 4k

" 快速的单词跳转
noremap W 5w
noremap B 5b

nnoremap L $
nnoremap H ^

" 格式化
nnoremap <Leader>f :action ReformatCode<CR>

" 搜索文件
nnoremap <C-p> :action SearchEverywhere<CR>

" 分屏
" nnoremap sv :action SplitVertically<CR>
" nnoremap sh :action SplitHorizontally<CR>
noremap sj :set nosplitbelow<CR>:split<CR>:set splitbelow<CR>
noremap sk :set splitbelow<CR>:split<CR>
noremap sh :set nosplitright<CR>:vsplit<CR>:set splitright<CR>
noremap sl :set splitright<CR>:vsplit<CR>
nnoremap sc :action Unsplit<CR>

" 粘贴
vnoremap p pgvy

" 重命名变量
nnoremap <Leader>rn :action RenameElement<CR>

" gd   GotoDeclaration
nnoremap gd :action GotoDeclaration<CR>

" gi   GotoImplementation
nnoremap gi :action GotoImplementation<CR>

nnoremap <Leader>ca :action ShowIntentionActions<CR>

" 优化导包 <leader>io
nnoremap <Leader>io :action OptimizeImports<CR>

" 标签切换
nnoremap <C-l> gt
nnoremap <C-h> gT

" NERDTree
nnoremap <C-b> :NERDTreeFocus<CR>
let g:NERDTreeMapActivateNode='l'
let g:NERDTreeMapJumpParent='h'
let g:NERDTreeMapQuit='<C-b>'

```