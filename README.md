# About
This code is modified from a discussion in [stack exchange](https://tex.stackexchange.com/questions/130586/vim-nice-folding-function), which is adapted from [LaTeX-Box](https://github.com/LaTeX-Box-Team/LaTeX-Box) plugin.

The purpose of the code is to fold latex documents, but there's no need to use the whole LaTeX-Box plugin.

# Feature
This plugin should able to fold at least these: part, chapter section, subsection, subsubsection, preambles, frontmatter, abstract, frame, table, figure, equation, and all other command embedded in begin / end.

# Installation
## Using vim-plug
To install with [vim-plug](https://github.com/junegunn/vim-plug), the easiest way is to add this line
    > Plug 'akaron/foldtex.vim'

Alternatively, add as a local plugin

* make a folder for all these local plugins, such as `~/.vim/my_plug`
* put this `foldtex.vim` folder under `~/.vim/my_plug`
* add this line to `~/.vimrc`

	> Plug '~/.vim/my_plug/foldtex'


## without plugin manager
To install without plugin manager, put the file in `~/.vim/ftplugin/tex/folding.vim`.

# note
* This plugin hasn't been tested in many cases. So far it has been tested in one of my own latex file with `elsarticle` documentclass.
* If the plugin `restore-view` or something similar is installed, maybe remove the `view` files (in `~/.vim/view`) then open the latex file.
* It is *slow* to load latex files. For example, a 25 page elsarticle (single column, 11pt, preprint) cost 4-5 seconds to load. It's same while using LaTeX-Box. Have no idea how to improve.
* Sometimes it is slow while input in tex file. Maybe I'll try other package.
