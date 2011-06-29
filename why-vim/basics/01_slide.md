!SLIDE bullets incremental
# Basics #

* When you first open a file in vim, you're in normal mode.
* To be able to type at all, you need to enter insert mode.  `i` is one
  way to do this.

!SLIDE bullets incremental
# Basics (cont) #
* To move through the file in normal mode, you use `h,j,k,l` to go left,
  up, down, right.  This is because all of these keys are on the home
  rows and if you're typing a lot, you'll never have to take your hands
  out of the proper typing position.
* To save a file, `:w`
* To quit, `:q`

!SLIDE bullets incremental
# Basics (cont) #
* Extremely configurably via plugins and ~/.vimrc
* To get started, you can type `:help vimtutor` in normal mode.  This
  will take you to a tutorial that is very good for learning vim.

!SLIDE bullets incremental
# Some more quickies #

* To delete the rest of the line and enter insert mode to replace what
  was there: `C`
* To change a word: `cw`
* To delete a word: `dw`
* To delete a line: `dd`
* To yank a line (copy to vim clipboard): `yy`

!SLIDE bullets incremental
# Some more quickies (cont) #
* To paste what's in the vim clipboard: `p`
* To cut a single letter: `x`
* To incremental search a file: `/foo`
* To regex replace in a file globally: `:%s/foo/bar/g`

!SLIDE bullets incremental
# Slightly more advanced #

* Chaining these commands is where you start to feel really powerful.
* Transpose two letters in a word?  Fix it by going to the first letter
  and `xp`.  That will cut a letter and paste it after the cursor.
* Have a line of code that really needs to be below the next line?
  `ddp` will cut the line and paste it on the next line.

!SLIDE bullets incremental
# Slightly more advanced (cont) #
* It needed to be above the line you were on?  `ddP`
* Need to delete the next 18 lines?  `18dd`
* Repeat the last command? `.`  So to insert an asterisk at the front of
  a few lines, you can just `I* <ESC>j.j.j.j.j.j.`

!SLIDE bullets incremental
# Slightly more advanced (cont) #
* Record a macro? `qa` will start recording a macro referenced by the
  'a' key.  You can do anything at all in your macro.  Press q again to
  stop recording.

!SLIDE bullets incremental
# Slightly more advanced (cont) #
* Replay a macro? `@a` will replay the macro referenced by the 'a' key.
* If I wanted to insert `<li></li>` around 12 lines in a row, I might type
  the following:
* `qaI<li><ESC>A</li>jq11@a`

!SLIDE bullets incremental
# Slightly more advanced (cont) #
* I know it looks a  little confusing but it all goes into muscle memory
  after a bit and you become unbelievably fast and flexible.  I don't
  think of it as "type all the commands that do that."  I think of it as
  "I would like to do this" and out my fingers comes the appropriate means
  to that end.  It's what people are talking about when they say vim
  becomes an extension of your mind.

!SLIDE bullets incremental
# Slightly more advanced (cont) #
* Run a command in cwd?  `!mkdir foo`

!SLIDE bullets
# Where can I learn more? #

* (Shamelessly stolen from janus's README)
* Read the slides at [VIM: Walking Without Crutches](http://walking-without-crutches.heroku.com/#1)
* Watch the screencasts at [vimcasts.org](http://www.vimcasts.org)
* Watch Derek Wyatt's energetic tutorial videos at [his site](http://www.derekwyatt.org/vim/vim-tutorial-videos/)

!SLIDE bullets
# Where can I learn more? (cont) #

* Read wycats' perspective on learning vim at [Everyone who tried to convince me to use vim was wrong](http://yehudakatz.com/2010/07/29/everyone-who-tried-to-convince-me-to-use-vim-was-wrong/)
* Read this and other answers to a question about vim at [StackOverflow: Your problem with Vim is that you don't grok vi](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/1220118#1220118)
