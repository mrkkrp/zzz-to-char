# Zzz to Char

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![MELPA](https://melpa.org/packages/zzz-to-char-badge.svg)](https://melpa.org/#/zzz-to-char)
![CI](https://github.com/mrkkrp/zzz-to-char/workflows/CI/badge.svg?branch=master)

This package provides two new commands: `zzz-to-char` and `zzz-up-to-char`
which work like the built-ins `zap-to-char` and `zap-up-to-char`, but allow
the user to quickly select the exact character they want to zzz to. The
commands work like the built-ins when there is only one occurrence of the
target character, excepting that they automatically work in the backward
direction, too. One can specify how many characters to scan from each side
of the point, see `zzz-to-char-reach`.

## Installation

The package is available via MELPA, so you can just type `M-x
package-install RET zzz-to-char RET`.

If you would like to install the package manually, download or clone it and
put on Emacs' `load-path`. Then you can require it in your init file like
this:

```emacs-lisp
(require 'zzz-to-char)
```

## Usage

Just bind `zzz-to-char` or `zzz-to-char-up-to-char` (depends on your taste,
the latter doesn't include the target char into the killed text):

```emacs-lisp
(global-set-key (kbd "M-z") #'zzz-to-char)
```

## License

Copyright © 2015–present Mark Karpov

Distributed under GNU GPL, version 3.
