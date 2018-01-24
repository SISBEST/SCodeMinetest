## Copy the `only the new lines` and add it to your `mod.rkt` file

```
#lang minetest

(define-block ### ### ###)

(define-item xxx xxx xxx)
(define-item yyy yyy yyy)
(define-item zzz zzz zzz)

;; -- START OF NEW CODE --
(add-behaviour-to
 ###
 (drop (hash "items" (list (hash "items" (list
                                          "my_racket_mod:xxx"
                                          "my_racket_mod:yyy"
                                          "my_racket_mod:zzz"))))))
;; -- END OF NEW CODE --
        
(compile-mod my-mod)
        
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste

## Click [here](https://s3.amazonaws.com/thoughtstem.cms.dev/MinetestAssets/Curriculum/videos/multipleItemDrop.mp4) to watch the tutorial video
