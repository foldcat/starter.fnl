# starter.fnl

Nvchad [starter](https://github.com/NvChad/starter/tree/main) repo 
completely ported to fennel via 
[nfnl](https://github.com/Olical/nfnl).

To install, simply run 

```bash
rm -rf ~/.local/share/nvim
git clone https://github.com/nvchad/starter.fnl ~/.config/nvim && nvim
```

Run `:MasonInstallAll` command after lazy.nvim finishes 
downloading plugins.

It is recommended to remove the following files and directories after 
installation:

```
.git/
.gitignore
UNLICENSE
README.md
```

Check out `fnl/plugins/init.fnl` for plugins to make the lisp
editing experience better.

### Note 

- nfnl may not trust `.nfnl.fnl`, when prompted with the option 
to trust it, say yes
- do not edit any lua files generated by nfnl
- one could use [see fennel](https://fennel-lang.org/see) in order 
to convert existing lua code to fennel
- fnlchad does not impose a performance lose as it compiles fennel 
directly to lua after saving any fennel files in this config
- due to the above reason, you must also manually remove the orphaned
`.lua` file in `/lua` directory after removing `.fnl` files from `/fnl`
- for an example config, see [this](https://git.sr.ht/~koyuki/nvchad2.5)

### Credits

Credit to [cajus-nfnl](https://github.com/rafaeldelboni/cajus-nfnl)
for inspiring this project.
