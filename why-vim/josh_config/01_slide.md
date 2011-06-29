!SLIDE bullets
# Josh's config #

* So now that we've got that out of the way, I just wanted to point out a
few things that I do that I believe will make your configuration nicer,
or at least will make me more at home on your computer :)

* These will all be ~/.vimrc.local tweaks if you're running janus.

!SLIDE bullets
# Make tab navigation nicer #

    map <C-J> :tabn<CR>
    map <C-K> :tabp<CR>

* j and k take you up and down lines
* now J and K take you left and right tabs (it maps well in my head)

!SLIDE  bullets
# Open a file in a new tab a little faster #

    map <C-O> :tabnew 

* NOTE: There's a space at the end of that line
* Now ctrl+o will prefill `:tabnew ` for you so you just have to type the
  filename to open it in a new tab.  I'm usually in my rails project's
  root dir, so to open the People model I would
  `<C-O>app/models/people.rb` and I would let most of that tab-complete.

!SLIDE bullets small
# Show trailing whitespace and spaces before a tab #

    " Show trailing whitepace and spaces before a tab:
    :highlight ExtraWhitespace ctermbg=red guibg=red
    :autocmd Syntax * syn match ExtraWhitespace /\s\+$\| \+\ze\t/

* I hate these things existing in my code.  Now, if they exist, my editor
  will throw a garish red block in their place

!SLIDE bullets
# Set background color for the current line #
    " Set background color for the current line
    :set cursorline

* This makes my experience nicer, I like to see the current line
  highlighted.

!SLIDE bullets
# No toolbar, no mouse click #
    " Turn off menu in gui
    set guioptions="agimrLt"

    " Turn off mouse click in gui
    set mouse=""

* I don't want to see a toolbar in gvim, and I don't want clicking the
  mouse to set my cursor position in gvim.  This handles that.
