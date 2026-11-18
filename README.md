# dots
dotfiles etc

## doom

[Doom Emacs](https://github.com/doomemacs/doomemacs) user config (`$DOOMDIR`).

Setup:

```sh
git clone https://github.com/tjleing/dots ~/dots
git clone --depth 1 https://github.com/doomemacs/doomemacs ~/.config/emacs
ln -s ~/dots/doom ~/.config/doom
~/.config/emacs/bin/doom install
```

### Jai

Uses forks of [jai-ts-mode](https://github.com/tjleing/jai-ts-mode) (installed
by `doom sync`) and [tree-sitter-jai](https://github.com/tjleing/tree-sitter-jai)
(parser regenerated at ABI 14 for Debian's libtree-sitter 0.22).
Install the grammar once per machine:

```
M-x treesit-install-language-grammar RET jai
```

The LSP is `jailsp` (Jacket), which must be on `PATH`.
