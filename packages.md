---
layout: page
title: Java Packages
---

 :package:

 A *package* allows a group of related type definitions (such as classes and enums) to be grouped together. For a type to belong to a package, e.g., `packageName`, the code must be located in a directory named e.g., `packageName` and each file must begin with:

```java
 package packageName;
 ```

 With this information, we are able to understand the *protected* access modifier. Recall, a *public* class is visible to all classes everywhere. Access modifiers can also apply to class members (variables and methods). The *private* modifier specifies that the member can only be accessed in its own class.

 Classes within the same package have access to any of each other’s members having `public`, `protected` or default visibility (i.e., anything but `private`).


---
[« Casting](casting)
{: .navi-left}

[Enum Types »](enum)
{: .navi-right}