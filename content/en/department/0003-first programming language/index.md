---
title: Programming Linguistics Report
date: 2024-03-01
---

The activity to explore Python's efficient technology for storing large integers

<!--more-->
```
-Department of Computer Science and Engineering 202011680 An Hyun PL Report

-Subject
Python's Efficient Technology for Storing Large integers

-Introduction
In traditional programming languages such as C language, the range of values that can be stored varies depending on the data type and data type. For example, determine the size of the values that can be stored as short and int, and long and long.
But Python doesn't have this data type. So let's learn how Python stores large integers and can reliably process data without the use of data types.

-Main Topic
Python represents all objects as C structures. All integers of them are managed using an internal structure called "PyLongObject." A feature of this structure is that it is essential to implement arithmetic with arbitrary precision.
If that's the case, we first need to know what arbitrary precision arithmetic is. Random precision is also called big-num arithmetic or multi-precision arithmetic. It contrasts with fixed precision arithmetic, which provides precision of 8 to 64 bits used in most programming languages. It has the disadvantage of being very slow, compared to the advantage of being able to calculate with almost infinite size of numbers and high accuracy. It also has the feature of using a variable length array of numbers rather than a fixed number of bits. Therefore, it is used in computers to handle very large numbers or calculations that require high precision.
This time, we're going to learn about PyLongObject. First of all, in Python, all data types are treated as objects, and so are integers. And we have to use structures to represent these objects, and the structure that represents integers is PyLongObject.
So let's talk about how PyLongObject can store integers. The structure stores an array using an ob_digit array, which is a variable-length array. This array has an element called a digit, which is typically stored in units of 30 bits (15 bits on some systems). If this is the case, a 30-bit digit has a value of 2^30. If you need to store more than this, you can divide it into several digits (2^30) and store them consecutively in an ob_digit array. And the signs of integers are stored in the ob_size field to represent positive numbers, negative numbers, and zero. The absolute value of ob_size also represents the number of digits.
Python can use PyLongObject to perform arbitrary precision arithmetic. Each digit in the ob_digit array is used as an independent number to perform operations such as addition, subtraction, multiplication, division, etc.
Random precision operations using PyLongObject structures can be slower than high-precision arithmetic because each operation requires multiple digits to be processed. However, compared to C language or other languages, where you have to pay attention to the size of the numbers and write your own data types for each number's range, Python's operations allow users to conveniently use large integers without having to worry about the range of numbers or data types, and they can be operated with almost infinite size and high accuracy.

-Conclusion
Unlike the general programming language, which uses data types to specify a fixed size to store integers, Python uses a technique called arbitrary precision arithmetic, and it uses a structure called PyLongObject to use it. It is a structure that stores integers using a variable-length array called ob_digits. This arrangement uses an element called digit, which is 30 bits in size, to store large numbers. And the size of the array can change fluidly depending on the number of digits, so no matter how large the number is, it is easy and convenient to store. And even when you do arithmetic, you can use digit as an independent number.
These features have the advantage of being able to perform operations with almost infinite size and high accuracy, as well as the disadvantage of being slow because each operation has to process multiple elements. However, because large integers can be used easily and conveniently without worrying about complex details such as data types, the language called Python seems to have made it easy and attractive to developers, and many developers have chosen Python.
```