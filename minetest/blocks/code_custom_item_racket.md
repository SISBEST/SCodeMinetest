## Copy the `new line only` and add it to your `mod.rkt` file

```
#lang minetest

(define-block ### ### ###)

;; -- START OF NEW CODE --
(define-item ### ### ###)
;; -- END OF NEW CODE --


(add-behaviour-to ### (drop "default:sword_diamond"))
        
(compile-mod my-mod)
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste
