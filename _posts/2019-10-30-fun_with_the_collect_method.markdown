---
layout: post
title:      "Fun With the .collect Method"
date:       2019-10-30 15:25:02 -0400
permalink:  fun_with_the_collect_method
---

One of my favorite things I've learned in Ruby is the concept of iterating over collections of items to work with data. There are plenty of methods to use and play around with to see how they work. Here, we'll work with `.collect`. Note, `.collect` is an alias for `.map` - i.e. they do the exact same thing. 

`.collect` has a couple of common uses. One that you may find yourself doing often is, simply, collecting items into a new array and returning it:

```
student_grades = {
 Aleksy: "A",
 Eunice: "B",
 Tovar: "C",
 Farha: "B"
}
```

All I want is an array of the grades only, with no names attached:

```
grades_only = student_grades.collect { |name, grade| grade }
 => ["A", "B", "C", "B"]
```

Another common thing to do is to transform each item in a collection and return a new array with those transformed items.

Let's say I have an array of names:

```
names = ["genevieve", "harlowe", "abigail", "luis", "donovan"]
```

Suppose there were another 60 names in this array and they were all formatted in different ways - some capitalized, some not. Instead of having to manually go in and fix every single name, I can `.collect` them into a new array and fix the formatting:

```
capitalized_names = names.collect { |name| name.capitalize }
 => ["Genevieve", "Harlowe", "Abigail", "Luis", "Donovan"]
```

These are just two simple ways to use the `.collect` method! It's straightforward and incredibly useful.

