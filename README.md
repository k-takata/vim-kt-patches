<!-- [![Build status](https://ci.appveyor.com/api/projects/status/08qq79ukn7y64i3o/branch/default?svg=true)](https://ci.appveyor.com/project/k-takata/vim-ktakata-mq-osdn/branch/default) -->

# K.Takata's patch queue for Vim

This is my private patch queue for Vim.

Some of the patches are already sent to [vim_dev](https://groups.google.com/forum/?fromgroups#!forum/vim_dev), some others are work in progress.
(And some others are not written by me. Maybe copied from vim_dev.)

## How to use

Use [stq](https://github.com/k-takata/stq) to manage the patches.

### First time

    $ stg clone https://github.com/vim/vim.git vim
    $ cd vim
    $ git clone https://github.com/k-takata/vim-kt-patches.git .git/patches
    $ stq select linux    # if needed
    $ stq push -a
    $ make

### Update

If you want to get the latest source code after clone, you can use the following command:

    $ stq pull

## License

The Vim License (if it is written by me.)
