# .bashrc vs .bash_profile

If you would like to understand, [read this](http://www.joshstaiger.org/archives/2005/07/bash_profile_vs.html).

Put all your custom settings in your `~/.bashrc` file and source it in your `~/.bash_profile` with the following code.

```shell
if [ -f ~/.bashrc ];
  then
    source ~/.bashrc
fi
```
