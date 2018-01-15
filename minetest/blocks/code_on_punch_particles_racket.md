## Copy the `new lines only` and add it to your `mod.rkt` file

```
#lang minetest

(define-block ### ### ###)

;; -- START OF NEW CODE --
(game-rule
 on: block punch ###
 do: (particles 20 ###))
;; -- END OF NEW CODE --
        
(compile-mod my-mod)
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste
