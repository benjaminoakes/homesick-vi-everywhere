# homesick-vi-everywhere

A Homesick castle to use `vi` keybindings everywhere.

## Shortcut

Need `vi` mode right away?  Hit `M-C-j` (`Meta` then `Control` then `j`).  On Ubuntu, `Meta` is the right `Alt` key.  On the Mac, you might have to hit the keys all at once (after configuring Meta in your terminal, typically as `Option`).  [More info...](https://cnswww.cns.cwru.edu/php/chet/readline/readline.html#SEC22) (🚫 _broken link as of 2019-07-31_.  An [archived version](https://web.archive.org/web/20171027212523/https://cnswww.cns.cwru.edu/php/chet/readline/readline.html#IDX207) is available.)

This is temporary, but useful sometimes, like when using a Docker container.

## What Is It?

### Problem

Many programs default to `emacs` keybindings, but your favorite editor is `vi`.  You would like to have `bash`, `irb`, etc. to have the same keybindings you've come to know and love.

### Solution

Use `homesick-vi-everywhere`, a package of dotfiles to enable `vi` keybindings wherever possible.

This will allow you to use `vi` keybindings in:

* `bash`
* `coffee`
* `irb` (Ruby)
* `mysql`
* `node`
* `python`
* `sqlite3`
* `tmux`
* ...and others that use GNU readline

## Installation

It's the same as any other Homesick castle (keep in mind that you can have more than one).  Here are the basics:

    gem install homesick
    homesick clone benjaminoakes/homesick-vi-everywhere
    homesick symlink homesick-vi-everywhere

If you want to modify your shell so that `vi` is used in more cases, source `vi-everywhere` like so:

    source "$HOME/.vi-everywhere/bash.d/init.sh"

And for `tmux`, add this line in `~/.tmux.conf`:

    source-file "$HOME/.vi-everywhere/tmux.conf"

Please refer to [the documentation for Homesick](https://github.com/technicalpickles/homesick) for more information.

## Updating

Like with installation, it's the same as any other Homesick castle:

    homesick pull benjaminoakes/homesick-vi-everywhere

## Contributing

If you run into an issue specific to this project, please [create an issue on GitHub](https://github.com/benjaminoakes/homesick-vi-everywhere/issues).

Pull requests to add or improve `vi` keybindings for more programs are welcome!

## License

Copyright (C) 2013 Benjamin Oakes

This program is licensed under GPLv2.  See LICENSE for a copy.
