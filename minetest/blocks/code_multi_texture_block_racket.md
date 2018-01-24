## Copy the following code into your `mod.rkt` file

```
#lang minetest

;; -- START OF NEW CODE --

(define-block xxx yyy zzz)

(add-behaviour-to xxx
                  (tiles (list aaa ;top face
                               bbb ;bottom face
                               ccc ;right face
                               ddd ;left face
                               eee ;back face
                               fff ;front face
                               )))
                               
;; -- END OF NEW CODE --

(compile-mod my-mod)
```
* Highlight the code only and press **CTRL+C** to copy and **CTRL+V** to paste
