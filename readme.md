# pastery.el

Paste buffer or region to pastery.net from emacs.

## install

### without package manager

Get `pastery.el` and add to load paths with:

```emacs-lisp
(load-to-list 'load-path "/PATH/TO/pastery.el")
```

### melpa

To included `melpa` to your package archives.

```emacs-lisp
(add-to-list 'package-archives '("melpa" . "http://melpa.org/packages/") t)
```

Simply download from the `M-x package-list-packages RET` and include to your `.emacs`.

```emacs-lisp
(require 'pastery)
```

## usage

Setup your pastery key in `customize-variable`

```emacs-lisp
(customize-variables
  '(pastery-api-key "YOUR_KEY"))
```

### to list

`M-x pastery-list`

This will open a buffer with a list of all you pastes available.

### to get a single paste

`M-x pastery-get PASTE_ID`

This will open a buffer with the information of the paste where you can get its URL.

### to submit a paste

If you have a region selected, it will be sent. To send an entire buffer just call the function.

`M-x pastery-submit`

## license

See license.md
