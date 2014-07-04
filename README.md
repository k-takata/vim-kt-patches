# K.Takata's patch queue for Vim #

This is my private patch queue for Vim.

Some of the patches are already sent to [vim_dev](https://groups.google.com/forum/?fromgroups#!forum/vim_dev), some others are work in progress.
(And some others are not written by me. Maybe copied from vim_dev.)

### How to use ###

```sh
$ hg qclone https://vim.googlecode.com/hg/ -p https://bitbucket.org/k_takata/vim-ktakata-mq vim
$ cd vim
$ hg qselect linux    # if needed
$ hg qpush -a
$ make
```

### License ###

The Vim License (if it is written by me.)