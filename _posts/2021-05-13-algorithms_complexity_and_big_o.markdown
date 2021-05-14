---
layout: post
title:      "Algorithms Complexity and Big O"
date:       2021-05-14 01:21:06 +0000
permalink:  algorithms_complexity_and_big_o
---


## Time Complexity

The time complexity of an algorithm refers to the total amount of operations performed by the algorithm to return an output.  Here are a few examples of an operation:

* comparison(*a < b*)
* sum(*a + b*)
* division(*a /  b)*
* const nums = [];
* currentNode = currentNode.next;

## Space Complexity

The space complex refers to the amount of memory used by the algorithm.  If the algorithom creates a data structure such as an array, the memory used by the array will be part of the algorithms space complexity.  If the algorithm is recursive, the memory used by the call stack during the recusion will be part of the algorithm's space complexity.

## Big O Notation

Big O Notation describes an algorithm's worst case time or space complexity.  The longest time an algorithm will run or the max amount of memory that the algorithm uses.  Here are a few examples of big O notation:

* O(1) 
* O(log n)
* O(n)
* O(n log n)
* O(n^2)
* O(n^3)
* O(2^n)
* O(n!)
* O(n^n)

An example of how it is expressed in relation to an algorithm's complexity is:

*mergeSort runs in O(n log n) time and uses O(log n) space*

O(1) time refers to constant time complexity or constant space complexity.  Constant time means the complexity is not dependent on the input size.  It always completes in the same time.  Constant space means the memory used by the algorithm will the same every time it is run; the complexity is not dependent on the size of the input.

n represents input(an argument) into the algorithm.  If you have multiple inputs that contribute to an algorithm's complexity, they can be represented by multiple variables(such as m, b, s, or any other letter that makes sense).

## Conclusions
Space and time complexites expressed in big O notation are concerned with how input to the algorithm affects run time and memory used.  An algorithm that performs 10 operations reguardless of input size runs in O(1) time even though it takes 10 operations to produce an output.  The amount of operations do not matter, the amount of change does.  An algorithm that copies an array 3 times will not use O(3n) space, it will use O(n) space because it will always copy three arrays independent of input size.

To keep it simple, this overview was very brief.  It would be a good idea to research why doing something a constant number of times doesn't affect big O complexity.  Also, the same reasoning can be applied to why lower order terms do not affect big O complexity( O(n log n + n) is O(n log n) *multiplication matters but addition does not*).  I not saying that constant factors never matter( there are times when you'll want to reduce your constant factors ), but big O notation is not concerned with those constant factors.








