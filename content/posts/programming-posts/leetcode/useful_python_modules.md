---
title: "Useful Python Libraries & Modules"
date: 2024-07-27T10:54:00-02:30
hero: /images/posts/programming-posts/leetcode/useful_python_modules_hero.png
menu:
  sidebar:
    name: "Useful Python Libraries & Modules"
    identifier: useful_python_modules
    parent: leetcode
    weight: 1

---

### Bisect

[Reference](https://docs.python.org/3/library/bisect.html)


Incredible module for inserting and searching an array for values using a binary search
- Useful methods include:
  - `bisect.bisect(arr, val)` - searches for the value in the array and returns an insertion point coming after any existing entries of the value
  - `bisect.bisect_left` - searches for the value of the array and returns insertion point to the left of it
  - `bisect.bisect_right` - same as `bisect_left` but for insertions to the right
  - `bisect.insort` - inserts a value into the array in a sorted manner. Uses `bisect_right` and `insert` to insert the value. *This is time complexity $O(N)$ for a list*
    - If you intend to do this, a better approach could be to use a different data structure than a list