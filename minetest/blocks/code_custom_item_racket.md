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

## Click [here](https://s3.amazonaws.com/thoughtstem.cms.dev/MinetestAssets/Curriculum/videos/editItemCode.mp4) to watch the tutorial video

## Previous Code
1. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_custom_block_racket.md) for custom block code
2. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_custom_item_racket.md) for custom item code
3. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_drop_item_racket.md) for item drop code
4. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_drop_multiple_items_racket.md) for multiple item drop code
5. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_on_punch_particles_racket.md) for particles code
6. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/edit/master/minetest/blocks/code_multi_texture_block_racket.md) for mutiple textured block code


Need some textures click [here](https://github.com/thoughtstem/TS-CurriculumPublic/tree/master/minetest/images), or a simple racket file click [here](https://s3.amazonaws.com/thoughtstem.cms.dev/MinetestAssets/Curriculum/starter_Files/mymod.rkt)
