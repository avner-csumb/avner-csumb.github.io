---
layout: page
title: Big-O Notation
---

A formal approach to describing the performance or complexity of an algorithm is called **Big O Notation**. This describes how an algorithm performs as its input changes.

For instance, an algorithm described as having a worst-case performance of `O(n²)` means that as the size of the input doubles, the algorithm takes four times longer to run. An `O(n²)` algorithm is often not the most efficient implementation, although this is entirely dependent on the exact goal of the algorithm.

Big O tends to be applicable for larger values of n. When n is small, the running time or space consumption of an algorithm is often negligible. Regardless, for any algorithm you do write, it is always worth considering Big O notation, even for small values of n, as, over time, you may find you are running your algorithm with larger and larger input.
