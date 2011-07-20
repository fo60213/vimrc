maso's vimrc
============
Original Author: Tsung-Hsiang (Sean) Chang <vgod@vgod.tw>

Modifier: maso (fo60213)

Fork me on GITHUB  https://github.com/fo60213/vimrc.

HOW TO INSTALL
--------------

1. Check out from github

        $ git clone https://github.com/fo60213/vimrc ~/.vim
        $ cd ~/.vim
        $ git submodule update --init

2. Install ~/.vimrc and ~/.gvimrc

        $ ./install-vimrc.sh
  
UPGRADE PLUGIN BUNDLES
----------------------

All plugins (except vim-latex, matlab-colour) were checked out as git submodules, 
which can be upgraded with `git pull`. For example, to upgrade Nerd Tree 

     $ cd ~/.vim/bundle/nerdtree
     $ git pull

HOW TO USE
----------

see the "USEFUL SHORTCUTS" section in vimrc to learn my shortcuts.

PLUGINS
-------

* [Pathogen](http://www.vim.org/scripts/script.php?script_id=2332): Pathogen let us install a plugin as a bundle in ~/.vim/bundle seprately.

* [Nerd Tree](http://www.vim.org/scripts/script.php?script_id=1658): A tree explorer plugin for navigating the filesystem.

  Useful commands:
  * `:Bookmark [name]` - bookmark any directory as name
  * `:NERDTree [name]` - open the bookmark [name] in Nerd Tree

* [AutoClose](http://www.vim.org/scripts/script.php?script_id=1849):  Inserts matching bracket, paren, brace or quote.

* [vim-surround](https://github.com/tpope/vim-surround/blob/master/doc/surround.txt): deal with pairs of surroundings.

* [matchit](http://www.vim.org/scripts/script.php?script_id=39): extended % matching for HTML, LaTeX, and many other languages. 

* [xmledit](http://www.vim.org/scripts/script.php?script_id=301): XML/HTML tags will be completed automatically.

* [SuperTab](http://www.vim.org/scripts/script.php?script_id=1643): Do all your insert-mode completion with Tab.

* [snipMate](http://www.vim.org/scripts/script.php?script_id=2540): TextMate-style snippets for Vim

  `:help snipMate` to see more info.

* [YankRing](http://www.vim.org/scripts/script.php?script_id=1234): Maintains a history of previous yanks, changes and deletes 
  
  `:help yankring` to see more info.
  
* [Cute Error Marker](http://www.vim.org/scripts/script.php?script_id=2653): showing error and warning icons on line.
  
   Note: MacVim users need to enable "Use experimental renderer" to see
   graphical icons.

* [vim-latex](http://vim-latex.sourceforge.net/): Latex support.

* [OmniCppComplete](http://www.vim.org/scripts/script.php?script_id=1520): C/C++ omni-completion with ctags database.

* [JavaComplete](http://www.vim.org/scripts/script.php?script_id=1785): Java Omni-completion.

* [Vim-Ruby](https://github.com/vim-ruby): vim configuration files to help you to programming with Ruby.

* [Matlab-colour](http://www.mathworks.com/matlabcentral/fileexchange/28240-highlighting-matlab-files-in-vim): matlab syntax highlight, indent, and many useful things developed by [Yaroslav](http://www.mathworks.com/matlabcentral/fileexchange/authors/62644)

* [Matlab-Snippets](https://github.com/fo60213/matlab-snippets): matlab snippets which is original from [matlab-tmbundle](https://github.com/textmate/matlab.tmbundle).

Language specific supports
--------------------------

* Latex: Read `:help latex-suite.txt`
* Restructured Text: `ctrl-u 1~5` inserts Part/Chapter/Section headers
* HTML, Javascript, Python, CSS, C, C++, Java, Ruby: use `TAB` to do omni-completion.
* HTML/XML: End tags are automatically completed after typing a begin tag. (Typing > twice pushes the end tag to a new line.)

Other good references
---------------------

* http://amix.dk/vim/vimrc.html
* http://spf13.com/post/perfect-vimrc-vim-config-file

What I modified
---------------

* remove Command-T, Vislncr plug-in
* add vim-ruby plug-in
* add matlab-colour plug-in, and change color of fucntion's "end" to let it be different with loop's "end", and change its newline character to Unix style
* add matlab-snippets
* add text width restriction to 80
* set SuperTab's function to default (C-P)
