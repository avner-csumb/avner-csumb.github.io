---
layout: page
title: Enum Types
---

 :musical_keyboard:

Given the current data types we have encountered (int, boolean, float, char, etc.), how might we represent a finite set of choices? For example, what if we want to represent the days of the week (Monday, Tuesday, etc.)?

Up-to-now, our best choice is probably to define the days of the week as constants. In Java, a constant is preceded by `static final` and then the data type. So, we might do that following:

```java
static final int MON = 0;
static final int TUE = 1;
static final int WED = 2;
```

We can then make an assignment such as `today = MON`, rather than the more cryptic, `today = 0`.

We can, however, do even better using so-called *enumerated* types, or *enums* for short. An *enum* is a type that is only allowed to take on values from a finite set of values.

Enums are declared as follows:

&nbsp;&nbsp;&nbsp; *modifier* **enum** *name* { *valueName*<sub>0</sub>, *valueName*<sub>1</sub>, ..., *valueName*<sub>n-1</sub> };

where the *modifier* can be blank, **public**, **protected**, or **private**.

Returning to our days of the week example, we can write:

```java
public enum Day { MON, TUE, WED, THU, FRI, SAT, SUN };
```
Once defined, `Day` becomes an official type and we may declare variables or parameters with type `Day`. For example, we can declare: `Day today;`.

In the above example, to assign a value to that variable, we do the following: `today = Day.MON;`

<br />

<small>(Adapted from *Data Structures and Algorithms in Java*, 6th Edition)</small>


---
[« Packages](packages)
{: .navi-left}

[Generics »](generics)
{: .navi-right}