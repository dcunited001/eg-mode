EG-Mode
=========

> a sample minor-mode for emacs

#### Defining Minor Modes:
http://www.gnu.org/software/emacs/manual/html_node/elisp/Defining-Minor-Modes.html

#### Minor Mode Conventions:
http://www.gnu.org/software/emacs/manual/html_node/elisp/Minor-Mode-Conventions.html


```
(interactive (list (or current-prefix-arg 'toggle)))
(let ((enable (if (eq arg 'toggle)
  (not foo-mode) ; this mode's mode variable
  (> (prefix-numeric-value arg) 0))))
(if enable
  do-enable
    do-disable))
```
