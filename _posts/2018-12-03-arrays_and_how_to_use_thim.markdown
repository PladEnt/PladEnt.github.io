---
layout: post
title:      "Arrays And How to Use Thim"
date:       2018-12-04 01:37:59 +0000
permalink:  arrays_and_how_to_use_thim
---


 	 Arrays are ordered, integer-indexed collections of any object.
Array indexing starts at 0, and move on to 1,2,3, and so on. A negative index is assumed to be relative to the end of the array, an index of -1 indicates the last element of the array, -2 is the next to last element in the array, and so on.
You can make a new array by using the literal constructor []. Arrays can contain different types of objects. For example, the array below contains an integer, a string, and a float.

1. ary = [1, "two", 3.0] 
2. #=> [1, "two", 3.0]

  An array can also be created by explicitly calling “.new” with zero, one (the initial size of the Array) or two arguments (the initial size and a default object).

1. ary = Array.new
2. #=> []
3.
4. Array.new(3)
5. #=> [nil, nil, nil]
6. 
7. Array.new(3, true)
8. #=> [true, true, true]

that the second argument populates the array with references to the same object. Therefore, it is only recommended in cases when you need to instantiate arrays with natively immutable objects such as Symbols, numbers, true or false.

  You can add to the front of arrays with “.unshift” 

1. ary = [“this is an array”]
2. #=> [“this is an array”]
3.
4. ary.unshift(“I added this, and”)
5. #=> [“I added this, and”, “this is an array”]

and add to the end with “.push”, and with the shovel method “<<”.

1. ary = [“this is an array”]
2. #=> [“this is an array”]
3.
4. ary.push(“, and I added this”)
5. #=> [“this is an array”, “, and I added this”]
6.
7. ary << (“, and this too”)
8. #=> [“this is an array”, “, and I added this”, “, and this too”]

And using “.pop” on an array will remove the last item from the end of the array.

1. ary = [1, 2, 3]
2. #=> [1, 2, 3]
3. 
4. ary.pop
5. #=> [1, 2]

And using “.shift” on an array will remove the item from the front of the array.

1. ary = [1, 2, 3]
2. #=> [1, 2, 3]
3.
4. ary.shift
5. #=> [2, 3]

