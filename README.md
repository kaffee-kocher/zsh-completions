# zsh-completions
My own ZSH completions. Feel free to use them.

## Enable ranger completion
Copy the `_ranger` file to one location of the `$fpath` variable. The command `echo $fpath | sed 's/ /\n/g'` shows all searching paths from the ZSH completion in a human-readable format.

After copying the `_ranger` file, add the following lines to your `~/.zshrc`:

```bash
autoload _ranger
compdef _ranger ranger
```

After restarting your ZSH (or apply `source ~/.zshrc`) the autocompletion for the ranger (file manager) command should work on your ZSH shell.
