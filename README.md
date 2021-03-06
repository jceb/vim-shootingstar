vim-shootingstar
================

Like the magic * but start matching at the cursor position.

Installation
------------

I recommend installing [pathogen.vim](https://github.com/tpope/vim-pathogen), and then execute the following commands:

    cd ~/.vim/bundle
    git clone https://github.com/jceb/vim-shootingstar.git

Usage
-----

* Given your cursor (`|`) is here: `shoo|ting start`
* Pressing `<leader>*` (e.g `\*`) will search for the term `ting` if it's part of the word `\<shooting\>`
* In vim search syntax this is equivalent to: `/\<shoo\zsting\>`

Supported keybindings
* <Leader>* and <Leader># for searching forward/backward for the exact word
* <Leader>g* and <Leader>g# for searching forward/backward without stopping at word boundaries

Why would I need that?
Peronsally, I'm using the `*` often when I want to refactor code, e.g. change the name of a variable or function.
Often I just want to change a certain part of the name and it would come very handy if the search would be able to place the cursor right there.
I'm too lazy to pull up the original search term and edit it, so I end up typing the whole name during the change.
This little plugin solves exactly the described issue by introducing just an extra character infront of the magic `*`.

License
-------
Copyright © Jan Christoph Ebersbach. Distributed under the same terms as Vim itself. See :help license
