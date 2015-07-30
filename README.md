**Personal Emacs setup and configuration files**.

I use `.el`-files placed in the `.emacs.d`-folder for any custom emacs configuration. The main setup is done by `setup.el`, which in turn loads the other setup files. `setup.el` is initalized simply by including

```elisp
;; Load setup
(load "~/.emacs.d/setup.el")
```

in the `.emacs`-file.

###Other notes-to-self

**Installation**
- Install `auctex` using package-install: `M-x package-list-packages RET`, locate `auctex`, and install (`package-list-packages` updates the package list).
- Install `projectile` using package-install: `M-x package-install RET projectile`
- Install `auto-complete` using package-install: `M-x package-install RET auto-complete RET`
- Install `latex-preview-pane` using package-install: `M-x package-install RET latex-preview-pane RET`
- Install `magit` using package-install: `M-x package-install RET magit RET`

*magit keybindings*
- `C-x g` *magit-status*
- `s` *stage* files, `u` unstage files (`S` and `U` to stage/unstage all hunks)
- `c c` to *commit* -> type message -> `C-c C-c` to finish
- `b b` to switch branch
- `P P` (in capital letters) to *git push*
- `F F` (in capital letters) to *git pull*

*polymode*
- `M-n r` in polymode-r mode to use the new *rmarkdown* (`render()`). Thanks to @r2evans and @malcook. 
- `M-n w` to *weave* (capital W to choose weaver), and `M-n e` to *export* (capital E to choose exporter)
