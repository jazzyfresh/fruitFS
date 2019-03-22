# fruitFS
a file system that is preferential to fruits

## Overview

Builds a file system hierarchy
and allows user to manipulate it via
CREATE, MOVE, DELETE commands.

```bash
$ cat fruit.in | ./fruit > fruit.out
$ diff fruit.out fruit.test
```

## Design

Represent a file system namespace with strings in a cache.
This was a quick hack that I thought supported
CREATE, DELETE, LIST, but now I'm realizing that
I should have created a tree after all.
The design choice was mostly because I didn't give myself
enough time to remember/google how bash data structures work.
