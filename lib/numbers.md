---
title: Numbers
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What are the different kinds of numbers in Ruby?

1) Integer (fixnum) This is any whole number meaning any positive or negative number that does not have any decimals.
    Examples include: 34, 2, -5469
2) Floating point numbers (Float) This is a number that utilizes decimal points.
    Examples include: 6.45636, -43.435, 27.57
3) Rational Numbers  These are numbers which are represented as a fraction of two integers. 
    Examples 0.25 is represented as 1/4 and 3.5 is represented as 7/2.

# What are some common operations and comparisons you would perform on numbers?

Common operations include addiion +, subtraction -, multiplication *, division /, exponents **, modulus %, etc.
These operations can be carried out on all of the types of numbers above and different combinations of each.  For example an integer 
can be multiplied by a float or a rational number can be added to an integer.

Common comparisons include ==, >, <, >=, <=, and !=. These comparisons will result in a boolean value (true or false). Like the 
opperators above, any combination of numbers above can be utilized to make a comparison. 

# What is the difference between the `+` operation on a number versus on a String?

When using the '+' operator on a number it returns the arithmetic value of the addition. Adding two integers, 5 + 5, would return 
the integer 10. If the '+' operator is used on a string it is called concatenation which joins two strings together end-to-end. 
"Hello" + "Hello" would return "HelloHello" and "5" + "5" would return the string "55".  

# If you have a _String_ `"20"` and want to perform a mathematical operation (like division or multiplication) on it, will it work? If yes, why? If not, how would you make it work?

You can not perform division on a string. "20" divided by 2 would return an error.  Multiplication works one way with a string 
but not with a result one would likely expect. You can not take 2 * "20" but you can take "20" * 2.  The latter example would 
return "2020". "20" * 3 would return "202020". This is more easily demonstrated using a string that does not use numerical characters.
Lets say we take 2 * "cup".  It doesn't make sense to multiply 2, cup times. Alternatively "cup" * 2 makes sense becuase we can take 
"cup" two times or "cupcup". Back to a sting of "20", if we wanted to do some form of mathmatics we would need to convert (I believe
this is called cast?) the string into a type of number.  "20" could be represented by an integer by taking "20".to_i. So if we 
wanted to divide "20" by two we would write "20".to_i / 2.

# What is the purpose of the `times` operation? Is that the same as `*`?

The times operation is different than the '*' operator becuase the times operation is an iterator. The times operation tells 
a block of code to run x times.  An example would be if we wrote 3.times {print "Hello"} returns "HelloHelloHello".  The '*' 
operator signifies multiplication. We can get the same result of the exammple above by writing "Hello" * 3. The difference comes 
when we replace the 'print "Hello"' in the 'times' example above with something more complex.
