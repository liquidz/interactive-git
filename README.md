# interactive-git

Controll git interactively

## requirements

 * git
 * peco

## zsh setting

```
if hash ig 2>/dev/null; then
    function interactive-git () {
        BUFFER=$(ig -d)
        zle accept-line
    }
    zle -N interactive-git
    bindkey '^g' interactive-git
fi
```
