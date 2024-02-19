[![Build status](https://ci.appveyor.com/api/projects/status/08qq79ukn7y64i3o/branch/default?svg=true)](https://ci.appveyor.com/project/k-takata/vim-ktakata-mq-osdn/branch/default)

# K.Takata's patch queue for Vim #

This is my private patch queue for Vim.

Some of the patches are already sent to [vim_dev](https://groups.google.com/forum/?fromgroups#!forum/vim_dev), some others are work in progress.
(And some others are not written by me. Maybe copied from vim_dev.)

## How to use ##
### First time ###

    $ hg qclone http://hg.osdn.net/view/vim/vim -p http://hg.pf.osdn.net/view/k/k_/k_takata/vim-ktakata-mq vim
    $ cd vim
    $ hg qselect linux    # if needed
    $ hg qpush -a
    $ make

You can use one of the following URL for the main repository of Vim:
 * <https://hg.256bit.org/vim>
 * <http://hg.osdn.net/view/vim/vim>

### Update ###

If you want to get the latest source code after qclone, you can use the following commands:

    $ hg qpop -a
    $ hg pull -u
    $ hg pull -u --mq
    $ hg qpush -a

Or you can use [this script](https://gist.github.com/k-takata/3a152aa2307cc3969cfd):

    $ mqpull.sh

## License ##

The Vim License (if it is written by me.)
