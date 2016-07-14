---
layout: page
title: Loop Conditions
---

Suppose we are asked to write a program that prints all prime numbers from 2 to n. Assume that we have previously written a method `isPrime()` that takes an integer and returns a boolean.

Find the error in the code.

```java
public static void printPrimes(int n) {
  int i;
  for( i=2; i<n; i++ ) {
    if(isPrime(i)) {
      System.out.print(" " + i);
    }
  }
}
```

With our error removed, when we finish the `for` loop and the method is about to return, what is the final value of `i`?

---

[« Week 2 Overview](week2)
{: .navi-left}

[Casting »](casting)
{: .navi-right}