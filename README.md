# About
This code is modified from a discussion in [stackexchange](https://tex.stackexchange.com/questions/130586/vim-nice-folding-function), which is adapted from [LaTeX-Box](https://github.com/LaTeX-Box-Team/LaTeX-Box) plugin.

The purpose of the code is to fold latex documents, but there's no need to use the whole LaTeX-Box plugin.

# Installation
with [vim-plug](https://github.com/junegunn/vim-plug)

* put this folder under `~/.vim/my_plug`
* add this line to `~/.vimrc`

	> Plug '~/.vim/my_plug/foldtex'

* Done!

If the plugin `restore-view` or something similar is installed, maybe remove the `view` files (in `~/.vim/view`) then open the latex file.

To install without plugin manager, put the file in `~/.vim/ftplugin/tex/folding.vim`.

# note
This plugin hasn't been tested in many cases. So far it has been tested in one of my own latex file with `elsarticle` documentclass.

This plugin should able to fold at least these: part, chapter section, subsection, subsubsection, preambles, frontmatter, abstract, frame, table, figure, equation, and all other command embedded in begin / end.