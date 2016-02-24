---
title: Arrays
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is an Array?

An Array is collection of individual values (list)

# What are some examples of information that would be Arrays as opposed to some other data type?

Arrays are great for storing similar data under on variable instead of multple variables. 
you can store any type of string or interger, there is really no limition. 

# What is one way, using Ruby, to retrieve the 6th element in an Array? How about the 8th element? What happens if you try to retrieve the value of the _9999th_ element (or some element that doesn't exist in the array)?

array1 = ['jay', 'bernal', 'julio', 'melissa', 'ann', 'aria', 'maggie', 'cindee', 'chris']
array1 [5]
array1 [7]
array1 [11] = will return a null value

# The previous question asks about finding, for example, the 6th element in an Array. Is it possible to find the **-6th** (Notice the negative symbol!) element in an Array? What does that even mean?

array1 [-6] - will find 'ann' if searches from right to left, but no zero index.

# How would you perform an operation on every element inside an Array?

You can use Iterating to change every element within the array.

array1 = ['jay', 'bernal', 'julio', 'melissa', 'ann', 'aria', 'maggie', 'cindee', 'chris']
array1.each {|i| puts i.upcase }

# How do you add elements to an Array?

array1.push('john') - adds the item to the end
array1 << 'smith' - adds the item to the end

array1.unshift('doug') - adds items to the begining
array1.insert(5, 'mary') - this will added 'mary' to the fifth position

# Given the Array `["Laura", "Fiona", "Tori"]`, how would you replace `"Fiona"` with `"Florence"` so that you end up with `["Laura", "Florence", "Tori"]`?

name = ["Laura", "Fiona", "Tori"]
name.delete ('Fiona')
name.insert(1,"Florence")

# What do the methods `push`, `pop`, `shift`, and `unshift` do?

push - adds objects to the end of the array
pop - removes the last object of the array
shift - removes the first object of the array and returns that object
unshift - Prepends objects to the front of the array, moving other elements upwards.

# How do you determine how many elements are in an Array?

use the length method. name.length

# How would you reverse the order of elements in an Array?

name.reverse

# How would you convert a String `"Sumeet Jain"` into an Array `["Sumeet", "Jain"]`? How about to `["S", "u", "m", "e", "e", "t", " ", "J", "a", "i", "n"]`? How would you convert the Array back into a String?

"Sumeet Jain".split()
"Sumeet Jain".split("")