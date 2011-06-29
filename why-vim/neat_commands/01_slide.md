!SLIDE bullets
# Some moar neat things you can do in vim

* `/foo/s-3`
* Nick's protip of the day: This command will search for foo an dplace
  the cursor 3 characters before the match.

!SLIDE bullets
# moar - JD

* `gg<S+v><S+G>=`
* JD - autoformat your file (i.e. set colwidths properly, set
  indentation to match your syntax file, etc).
* So if you open an html file that's not indented, this will nicely
  indent it all for you, for example.

!SLIDE bullets
# moar - David

* Set a marker in a buffer with `ma`.  Go to that marker with ``a`
* Set a global marker with `mA`.  Go to that marker from any buffer with
  ``A`

!SLIDE commandline
# moar - Josh
## Use vim as a badass diff tool ##

    $vimdiff file1 file2

!SLIDE bullets
# moar - Josh

* fold a section of code up with `zf`
* unfold a folded section with `zo`

!SLIDE commandline
# moar - Josh
# Open a gzipped file in vim

    $vim log/production.log.20.gz

!SLIDE bullets
# moar - Josh

* Open another file in a split beneath the current buffer
* `:sp otherfile.txt`
* For vertical split, use `vsp`
* navigate splits with <CTRL+w>+`h,j,k,l`

!SLIDE bullets small
# moar - Josh

* Editing a file for a while and realize it's screwed?
  Know it worked 15 minutes ago?
* Just undo 15 minutes
* `:earlier 15m`
* Oh no I meant 10 minutes ago?
* `:later 5m`
