vis-gruvbox
===========

This is an attempted port of the [original Gruvbox colorscheme](https://github.com/morhetz/gruvbox) for Vim to the [Vis text editor](https://github.com/martanne/vis). It contains all of the Gruvbox colors used by that colorscheme and can be configured to light or dark mode at any of the pre-built contrast settings. Simply make the adjustments indicated by the comments in the file, move it to `~/.config/vis/themes/`, and set your theme in Vis as follows:

    :set theme gruvbox

Or add the following line to your `visrc.lua`:

    vis:command('set theme gruvbox')

Other notes
-----------

 - Because of the inherent differences between Vim and Vis in how syntax highlighting works, this is not a perfect duplicate of the original Gruvbox theme, but it is reasonably close and has worked well for me.
 - If you have a terminal with a transparent background and want to use that instead of the opaque background set by the theme, you can set the theme to use it by changing the value of `vis.lexers.STYLE_DEFAULT` to `'back:default,fore:'..colors.fg1` instead of `'back:'..colors.bg0..',fore:'..colors.fg1`.
