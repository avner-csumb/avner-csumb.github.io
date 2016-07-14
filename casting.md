---
layout: page
title: Types and Casting
---

:pager:

When you want to store data in a variable, you **have** to specify the *type*. Whereas in Python you might be able to write `x = 1`, in Java you must first state the type. We can do this in two lines:

```java
int x;
x = 1;
```

If you try to write the second line, without having first provided the first line (the *type*), you will get a compiler error.

Note: We can also write the above in one line: `int x = 1;`

For most commonly used data types, Java provides the following base types (also called *primitive* types):


| `boolean` | a boolean value: **true** or **false**  |
| `char` | 16-bit Unicode character |
| `byte` | 8-bit signed two's complement integer |
| `short` | 16-bit signed two's complement integer |
| `int` | 32-bit signed two's complement integer |
| `long` | 64-bit signed two's complement integer |
| `float` | 32-bit floating-point number |
| `double` | 64-bit floating-point number |

<br />
Java's `char` base type stores a value that represents a single text character.

There is no base type for strings. There is, however, a `String` class that is built in to Java. We can declare and a initialize a `String` instance as follows:

```java
String title = "Data Structures Bootcamp";
```

An important trait of Java's `String` class is that its instances are *immutable*; once an instance is created and initialized, the value of that instance cannot be changed.

**Note:** Java does provide a `StringBuilder` class which is effectively a mutable version of a string.

*Casting* is an operation that allows us to change the type of a value. In essence, we can take a value of one type and *cast* it into an equivalent value of another type. To explicitly cast, we use the following syntax:

&nbsp;&nbsp;&nbsp; *(type) exp*

**Important:** When we cast from a `double` to an `int`, we may lose precision, as any fractional portion of the value will be truncated. For example, consider the following:

```java
double d1 = 3.2;
double d2 = 3.9999;
int i1 = (int) d1;
int i2 = (int) d2;
double d3 = (double) i2;
```

Perform the casting example above in your IDE and print the results to the console (using `System.out.println()`).

---

[« Loop Conditions](loop-review)
{: .navi-left}

[Packages »](packages)
{: .navi-right}