[![Build status](https://ci.appveyor.com/api/projects/status/j9v6gmrxqlk7i8wr/branch/default?svg=true)](https://ci.appveyor.com/project/k-takata/vim-ktakata-mq/branch/default)

# K.Takata's patch queue for Vim #

This is my private patch queue for Vim.

Some of the patches are already sent to [vim_dev](https://groups.google.com/forum/?fromgroups#!forum/vim_dev), some others are work in progress.
(And some others are not written by me. Maybe copied from vim_dev.)

## How to use ##
### First time ###
```sh
$ hg qclone https://bitbucket.org/vim-mirror/vim -p https://bitbucket.org/k_takata/vim-ktakata-mq vim
$ cd vim
$ hg qselect linux    # if needed
$ hg qpush -a
$ make
```

### Update ###

If you want to get the latest source code after qclone, you can use the following commands:

```sh
$ hg qpop -a
$ hg pull -u
$ hg pull -u --mq
$ hg qpush -a
```

Or you can use [this script](https://gist.github.com/k-takata/3a152aa2307cc3969cfd):

```sh
$ mqpull.sh
```

## License ##

The Vim License (if it is written by me.)
