# Learning virtualenv on Windows in git bash

These are my notes on how to work with virtual environments, in the git bash environment, on Windows.

## Workflow

1. Create virtual environment

```
virtualenv learn_venv
```

2. Activate virtual environment

For comparison try `pip list` to note what packages are available in your base system. Then, activate the virtual environment by running

```
. learn_venv/Scripts/activate
```

After activation, you will see the name of the environment above your command prompt. You can also run `pip list` to note that the packages available have changed.

3. Exit / deactivate virtual environment

```
deactivate
```

Note that this is _not_ the same construct that you used to create the virtual environment.

## Sources

The following articles have been helpful in getting this far:

[Hitchhiker's Guide: virtual environments](http://docs.python-guide.org/en/latest/dev/virtualenvs/)

[Can not activate a virtualenv in GIT bash mingw32 for Windows](https://stackoverflow.com/questions/10450992/can-not-activate-a-virtualenv-in-git-bash-mingw32-for-windows)

[Virtualenv's bin/activate is Doing It Wrong](https://gist.github.com/datagrok/2199506)

Less useful for Git bash, but applied wonderfully to the usual Windows command prompt:
[Out of a git console: how do I execute a batch file and then return to git console?](https://stackoverflow.com/questions/11865085/out-of-a-git-console-how-do-i-execute-a-batch-file-and-then-return-to-git-conso)