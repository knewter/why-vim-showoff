!SLIDE bullets incremental
# An Awesome Config #
## Janus ##

* Yehuda Katz and Carl Lerche wrote [janus](http://www.github.com/carlhuda/janus)
* It's a "vim distribution" that bundles together a certain
  configuration and a lot of plugins into one installation script.  It's
  intended to make it easy for TextMate users to get comfy in vim.

!SLIDE bullets incremental
# An Awesome Config (cont) #
* For the purposes of this talk, I've switched to using it on my
  machine.  I will probably switch back to my custom configuration
  again, but I felt I should give it more than a cursory try if I'm going
  to bring it up :)
* Installation is super simple and explained on the README.

!SLIDE bullets incremental
# Base Customizations #

* Line numbers
* Ruler (line and column numbers)
* No wrap (turn off per-buffer via set :wrap)
* Soft 2-space tabs, and default hard tabs to 2 spaces
* Show tailing whitespace as .

!SLIDE bullets incremental
# Base Customizations (cont) #
* Make searching highlighted, incremental, and case insensitive unless a capital letter is used
* Always show a status line
* Allow backspacing over everything (identations, eol, and start characters) in insert mode

!SLIDE bullets incremental
# Base Customizations (cont) #
* \<Leader>e expands to :e {directory of current file}/ (open in the current buffer)
* \<Leader>tr expands to :te {directory of current file}/ (open in a new MacVIM tab)
* \<C-P> inserts the directory of the current file into a command

!SLIDE bullets incremental
# Base Customizations (cont) #
* Automatic insertion of closing quotes, parenthesis, and braces
* Ships with over 100 color themes

!SLIDE bullets incremental
# Plugins #

* "Project Drawer" aka NERDTree - for project traversal (note: I never
  use anything like this)
* Ack.vim - ack inside cwd for a pattern
* Align - make your code line up nicely easily
* Command-T - like command-t in textmate

!SLIDE bullets incremental
# Plugins (cont) #
* ConqueTerm - embed a terminal inside a vim buffer
* Surround - modify what's surrounding a bit of text
* NERDCommenter - helps you format, modify comments nicely
* SuperTab - tab completion based on current context

!SLIDE bullets incremental
# Plugins (cont) #
* ctags - complete to your language's tag list
* Fugitive - an unbelievably awesome git plugin.  :Gblame on a file is
  fantastic.  Gdiff to see changes on your files, etc.
* Gist-vim - type :Gist in a buffer to paste the buffer to a gist and
  return the url

!SLIDE bullets incremental
# Plugins (cont) #
* ZoomWin - zoom in, out of split windows
* Hammer - convert the current buffer to html and open it in your
  browser.  For instance, when editing markdown files (like this one!)

!SLIDE bullets incremental
# Additional Syntaxes #

* Janus also ships you nice syntax highlighting for a host of file
  types.
* Markdown (bound to \*.markdown, \*.md, and \*.mk)
* Mustache (bound to \*.mustache)
* Arduino (bound to \*.pde)

!SLIDE bullets incremental
# Additional Syntaxes (cont) #
* Haml (bound to \*.haml)
* Sass (bound to \*.sass)
* SCSS (bound to \*.scss)
* An improved JavaScript syntax (bound to \*.js)

!SLIDE bullets incremental
# Additional Syntaxes (cont) #
* Map Gemfile, Rakefile, Vagrantfile and Thorfile to Ruby
* Git commits (set your EDITOR to mvim -f)
