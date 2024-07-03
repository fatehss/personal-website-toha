---
title: "673. Number of Longest Increasing Subsequence"
date: 2024-06-12T19:54:00-02:30
hero: /images/posts/programming-posts/leetcode/673_NLIS_hero.jpg
menu:
  sidebar:
    name: "673. Number of Longest Increasing Subsequence"
    identifier: 673NLIS
    parent: leetcode
    weight: 1

---

Today we are finding [the number of longest increasing subsequences](https://leetcode.com/problems/number-of-longest-increasing-subsequence/description) in an integer array.

### Approach

Since this involves finding the maximum length of something, we can make a good guess that it is a DP problem. Moreover, it does not look like we can use a two pointer greedy approach since there are multiple sequences to be found and they can be spaced out all over the array. Instead, we need to look at the problem deeper to see if there is some kind of recurrence to be exploited.

Let `nums = [1,3,7,6,3,8,9,2]`. It has a length of 8. If we stare at it enough, we can see that an LIS here has a length of 5, an example being `[1,3,6,8,9]`. But we also have 