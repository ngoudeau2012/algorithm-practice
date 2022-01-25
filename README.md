# algorithm-practice
Momoization Recipe

 1. Make it work.
    - Visualize the problems as a data tree
    - implement the true using recursion
    - test it


 2. Make it efficient 
    - add a memo object
    - add a base case to return the memo values 
    - store return values into the memo

CanSum

Write a function 'canSum(targetSum, numbers)' that takes in a targetSum and an array of numbers as arguments.

The function should return a boolean indicating whether or not it is possible to generate the targetSum using the numbers from the array.

You may use an element of the array as many times as needed.

You may assume that all input numbers are nonnegative.

---

Notes: 

canSum(7, [5, 3, 4, 7]) -> true

canSum(7, [2, 4]) -> false 

- function has two inputs 

m = target sum
n = array length

analyze the hight of the tree - what would be the maximal distance from the top level call to the base case 

the height of the tree is 1 

how does the numbers of nodes change from one level to the next
if you have 3 numbers in an array then a node would have 3 

O(n^m) time complexity - problem we need to solve.
0(m) space complexity 