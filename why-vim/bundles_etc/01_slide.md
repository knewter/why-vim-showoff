!SLIDE bullets
# Plugins, Bundles, etc #

* So there are tons of vim plugins out there.  These typically are
  shipped in .tar.gz files that you can unzip to your ~/.vim directory.
* That's pretty cool, and you can find a ton of them on
  [www.vim.org](http://www.vim.org)
* Installing plugins this way is like using global variables though :(

!SLIDE bullets
# pathogen #

* Tim Pope's [pathogen](http://www.vim.org/scripts/script.php?script_id=2332) is included with janus.
* It allows you to unzip plugins into ~/.vim/bundle and it will autoload
  them, without them getting all promiscuous in your global namespace.

!SLIDE bullets
# vimpack #

* Bram Swenson used to work for one of our clients, and he contributes
  to our open source projects somewhat regularly.
* He wrote [vimpack](https://github.com/bramswenson/vimpack).  It's like
  rubygems for vim setups.  It also has some pretty neat features coming
  down the pipeline.  It's written in ruby also.

!SLIDE bullets
# vimpack cont #
* `vimpack install rails.vim` will install the latest rails.vim
* `vimpack list` will list installed plugins
* `vimpack search foo` will search for plugins that include the word
  foo.  You can also specify the plugin type you're looking for
  (colorscheme, syntax, etc.)

!SLIDE bullets
# vimpack cont #
* vimpack has bundles coming as the next big feature.  It's like rvm for
  your vim setup.  So you can have different sets of plugins installed
  under different circumstances.
* Also, vimpack setups are git repos, so in the future janus could just
  be a vimpack repo you install via `vimpack install repo janus` and
  you'd get all of the janus install functionality, but in a nicely
  managed environment.
