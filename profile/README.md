<img src="/profile/logo-full.svg" width="500" height="250" />

<br/>

### (/kɪnˈtsuːɡi/, Japanese: 金継ぎ, lit. "golden joinery")
#### noun, also known as "kintsukuroi" (金繕い, "golden repair")
> 1. the Japanese art of repairing broken pottery by mending the areas of breakage with urushi lacquer dusted or mixed with powdered gold, silver, or platinum
> 2. a homoiconic programming language inspired by REBOL that compiles to LOVE- or Playdate-compatible Lua

<br/>

```red
qsort: function [blk] [
  if (length blk) <= 1 [return blk]
  set [pivot @rest] blk
  set [lo hi] loop/partition [for [x] in rest do [x < pivot]]
  append (append qsort lo pivot) qsort hi
]

unsorted: [3 1 4 1 5 9 2 6 5 3]
sorted: qsort unsorted
probe sorted                            ; 1 1 2 3 3 4 5 5 6 9
```
