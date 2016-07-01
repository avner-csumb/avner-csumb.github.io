---
layout: page
title: Exceptions
---

:rowboat:

An *exception* is an anomalous condition that alters or interrupts the flow of execution. Java provides built-in exception handling to deal with such conditions. Exception handling should not be part of normal program flow.

### Checked exceptions

* Checked exceptions are checked by the compiler at compile time.
* Methods that throw a checked exception must indicate so in the method declaration using the throws clause. This must continue all the way up the calling stack until the exception is handled.
* All checked exceptions must be explicitly caught with a catch block.

### Exception Handling Keywords

In Java, error-handling code is cleanly separated from error-generating code. Code that generates the exception is said to “throw” an exception, whereas code that handles the exception is said to “catch” the exception.

### The try/catch/finally Keywords

Thrown exceptions are handled by a Java try, catch, finally block. The Java interpreter looks for code to handle the exception, first looking in the enclosed block of code, and then propagating up the call stack to main() if necessary. If the exception is not handled on the main thread (i.e., not the Event Dispatch Thread [EDT]), the program exits and a stack trace is printed:


```java
try  {
  method();
} catch (EOFException eofe) {
  eofe.printStackTrace();
} catch (IOException ioe) {
  ioe.printStackTrace();
} finally {
  // cleanup
}
```

### The try-catch Statement

The `try-catch` statement includes one try and one or more catch blocks.

The try block contains code that may throw exceptions. All checked exceptions that may be thrown must have a catch block to handle the exception. If no exceptions are thrown, the try block terminates normally. A try block may have zero or more catch clauses to handle the exceptions.

TIP: A try block must have at least one `catch` or `finally` block associated with it.

---

[« Abstract classes](abstract-classes)
{: .navi-left}
