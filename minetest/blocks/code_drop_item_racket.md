## Copy the `new line only` and add it to your `mod.rkt` file

```
#lang minetest

(define-block ### ### ###)

;; -- START OF NEW CODE --
(add-behaviour-to ###
                  (drop "default:sword_diamond"))
;; -- END OF NEW CODE --
        
(compile-mod my-mod)
        
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste
