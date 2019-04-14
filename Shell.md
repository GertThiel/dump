# Shell (Tricks)

## Project local ZSH configuration

[](https://coderwall.com/p/a3xreg/per-directory-zsh-config)

Put this snippet into your `~/.zshrc`:

```shell
function chpwd() {
    if [ -r $PWD/.zsh_config ]; then
        source $PWD/.zsh_config
    else
        source $HOME/.zshrc
    fi
}
```

Then put a `.zsh_config` in any directory you want. This is an example how to
define aliases to use [qlot](https://github.com/fukamachi/qlot), project local
Common Lisp library configurations, with
[Roswell](https://github.com/roswell/roswell):

```shell
alias ros='qlot exec ros -S .'
alias rove='qlot exec rove'
```
