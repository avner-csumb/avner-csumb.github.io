---
layout: page
title: Arrays
---

A common programing task is to keep track of an ordered sequence of related values of objects. For example, say we want to create a leaderboard of the top ten scores for a sporting event. We could create ten different variables or, with an **array**, we can use a single name for the group and use index numbers to refer to the high scores in that group.

*Example leaderboard*

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{font-family:Arial, sans-serif;font-size:14px;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg th{font-family:Arial, sans-serif;font-size:14px;font-weight:normal;padding:10px 5px;border-style:solid;border-width:1px;overflow:hidden;word-break:normal;}
.tg .tg-e3zv{font-weight:bold}
.tg .tg-yw4l{vertical-align:top}
.tg .tg-9hbo{font-weight:bold;vertical-align:top}
</style>
<table class="tg">
  <tr>
    <th class="tg-e3zv">High scores</th>
    <th class="tg-031e">940</th>
    <th class="tg-031e">880</th>
    <th class="tg-031e">830</th>
    <th class="tg-031e">790</th>
    <th class="tg-031e">750</th>
    <th class="tg-031e">660</th>
    <th class="tg-031e">650</th>
    <th class="tg-031e">590</th>
    <th class="tg-yw4l">510</th>
    <th class="tg-yw4l">440</th>
  </tr>
  <tr>
    <td class="tg-9hbo">Indices</td>
    <td class="tg-yw4l">0</td>
    <td class="tg-yw4l">1</td>
    <td class="tg-yw4l">2</td>
    <td class="tg-yw4l">3</td>
    <td class="tg-yw4l">4</td>
    <td class="tg-yw4l">5</td>
    <td class="tg-yw4l">6</td>
    <td class="tg-yw4l">7</td>
    <td class="tg-yw4l">8</td>
    <td class="tg-yw4l">9</td>
  </tr>
</table>

<br />
An **array** is an object storing a numbered list of variables of the same type. The capacity of the array must be fixed when it is created, and insertions and deletions at interior positions of an array can be time consuming if many elements must be shifted. (We will discuss this topic further when we cover **Linked Lists**.)

Each variable is a primitive type or reference. The variables are indexed at zero and increment by one.

If we, for instance, want to create an array of characters, we declare it as such:

```java
char[] c;
```

This provides a reference to an array of characters (of any length).

To create the array of characters, we use the `new` command. We must specify the length of the array. Building on our `c` array, if we wish to allocate memory for an array of size `4`, we do the following:

```java
c = new char[4];
```

To assign values to members of an array, we do the following:

```java
c[0] = 'b';
c[1] = 'l';
c[2] = 'u';
c[3] = 'e';
```

Once you specify the length of an array, you cannot change it. If you run out of room and would like to create a larger array, you must create a new (larger) array and copy the elements from the original array to the new array.

Arrays have one instance variable called `length`. You cannot assign a value to `length`, but can use it to find the size of an array:

```java
c.length;
```

<br />

---

[« Generics](generics)
{: .navi-left}
