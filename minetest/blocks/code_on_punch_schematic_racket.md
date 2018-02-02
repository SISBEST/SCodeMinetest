## Copy the `new lines only` and add it to your `mod.rkt` file

```
#lang minetest

;; -- START OF NEW CODE --
(define-block aaa ### ###)

(define bbb
  (schematic wool-mapping (scale
                           .1 ###)))
                         
(game-rule
 on: block punch aaa
 do: (place-schematic bbb))
;; -- END OF NEW CODE --
        
(compile-mod my-mod)
```
**Reminder:**  **CTRL+C** to copy and **CTRL+V** to paste

## Click [here]() to watch the tutorial video

## Previous Code
1. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_custom_block_racket.md) for custom block code
2. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_custom_item_racket.md) for custom item code
3. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_drop_item_racket.md) for item drop code
4. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_drop_multiple_items_racket.md) for multiple item drop code
5. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_on_punch_particles_racket.md) for particles code
6. Click [here](https://github.com/thoughtstem/TS-CurriculumPublic/blob/master/minetest/blocks/code_multi_texture_block_racket.md) for mutiple textured block code


Need some textures click [here](https://github.com/thoughtstem/TS-CurriculumPublic/tree/master/minetest/images), or a simple racket file click [here](https://s3.amazonaws.com/thoughtstem.cms.dev/MinetestAssets/Curriculum/starter_Files/mymod.rkt)
