## Steps to setup:

- install plugin manager (vim-plug): 
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

- copy .vimrc to home directory:
```
curl -fLo ~/.vimrc https://raw.githubusercontent.com/andykirik/vimsetup/main/.vimrc
```

- create undo directory: 
```
mkdir ~/.vim/undodir -p
```

- install plugins which are in .vimrc file: reload .vimrc (:source % or restart vim) and :PlugInstall to install plugins.


Plugins:

Lightline - status line
	https://github.com/itchyny/lightline.vim

gruvbox - color scheme
	https://github.com/morhetz/gruvbox

Syntax file and other settings for TypeScript. 
	https://github.com/leafgarland/typescript-vim

man.vim - View man pages in vim. Grep for the man pages.
```
Viewing man pages:
	:Man printf - open printf(1) man page in a split
	:Vman 3 putc - open putc(3) man page in a vertical split (read more here on what the manual page numbers mean, they are really useful)
	:Man pri<Tab> - command completion for man page names
	:Man 3 pri<Tab> - completion "respects" the man page section argument
	:Man 6 <Ctrl-D> - list all man pages from section 6
```
Vim Rtags - Vim bindings for rtags.
	https://github.com/lyuts/vim-rtags

ctrlp.vim - Full path fuzzy file, buffer, mru, tag, ... finder for Vim.
	https://github.com/ctrlpvim/ctrlp.vim
```
Basic Usage:
	Run :CtrlP or :CtrlP [starting-directory] to invoke CtrlP in find file mode.
	Run :CtrlPBuffer or :CtrlPMRU to start CtrlP in find buffer or find MRU file mode.
	Run :CtrlPMixed to search in Files, Buffers and MRU files at the same time.
	Check :help ctrlp-commands and :help ctrlp-extensions for other commands.
Once CtrlP is open:
	Press <F5> to purge the cache for the current directory to get new files, remove deleted files and apply new ignore options.
	Press <c-f> and <c-b> to cycle between modes.
	Press <c-d> to switch to filename search instead of full path.
	Press <c-r> to switch to regexp mode.
	Use <c-j>, <c-k> or the arrow keys to navigate the result list.
	Use <c-t> or <c-v>, <c-x> to open the selected entry in a new tab or in a new split.
	Use <c-n>, <c-p> to select the next/previous string in the prompt's history.
	Use <c-y> to create a new file and its parent directories.
	Use <c-z> to mark/unmark multiple files and <c-o> to open them.
```
youcompleteme  - A code-completion engine for Vim
	https://vimawesome.com/plugin/youcompleteme
```
Installation Ubuntu 20.04:
	Install YCM plugin using plugin manager
	apt install build-essential cmake vim-nox python3-dev
	apt install mono-complete golang nodejs default-jdk npm
	cd ~/.vim/plugged/YouCompleteMe
	python3 install.py --all
Installation Ubuntu 16.04
	Install YCM plugin using plugin manager
	apt install build-essential cmake vim-nox python3-dev
	cd ~/.vim/plugged/YouCompleteMe
	python3 install.py --clangd-completer
```
UndoTree - 
	https://github.com/mbbill/undotree
```
Usage:
	:UndotreeToggle to toggle the undo-tree panel. 
	You may want to map this command to whatever hotkey by adding the following line to your vimrc, take F5 for example:
	nnoremap <F5> :UndotreeToggle<CR>
```
netrw - directory browser
```
:Explore or :Ex <path> - opens netrw in the current window
:Sexplore or :Sex <path> - opens netrw in a horizontal split
:Vexplore or :Vex <path> - opens netrw in a vertical split
:Vex! <path> - opens netrw in a vertical split, opposite side
I - Toggle the banner
c - Make the browsing directory the current working directory
i - Cycle between different listing modes (one of them is tree mode)
enter - Open files/directories
- - Go up one directory
o - Open file/directory in new horizontal split
v - Open file/directory in new vertical split
t - Open file/directory in new tab
p - Preview file without (moving the cursor from netrw)
x - Open the file/directory with the default system app
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
