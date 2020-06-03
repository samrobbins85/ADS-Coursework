# ADS Coursework

This is my solution for the coursework set for the Algorithms and Data Structures Module at Durham University
The questions were as follows:

## Question 1

Produce python code to add keys to a hash table. You must create the code for two functions `hash_quadratic` and `hash_double` that add keys (we ignore the values) to a hash table of size 19 using the hash function defined by _h(k)=6k+3 mod 19_. In `hash_quadratic` collisions should be handled by probing. In `hash_double` collisions should be handled using Double Hashing using the secondary hash function _h'(k)=11-(k mod 11)_. The input to the functions is a list of keys (positive integers) to add to the hash table and the output is the contents of the table where the symbol "-" indicated a bucket in the array containing no data. You can assume the input contains no duplicates.

## Question 2

Let k be 2,3 or 4. The k-child of a positive integer is defined to be a number obtained by taking the kth power of each digit and adding them. For example the 2 child of 19 is 1<sup>2</sup>+9<sup>2</sup>=82. The k-descendant sequence of a positive integer begins with the integer and then each successive term is the k-child of the previous one. The sequence terminates if it reaches a 1 or a term is repeated.

A positive integer is k-ephemeral if its k-descendant sequence ends in 1, and otherwise it is k-eternal.

Write a function called `count_ephemeral(n1,n2,k)` which, given two positive integers n<sub>1</sub> and n<sub>2</sub>, n<sub>1</sub>< n<sub>2</sub>, and k∈{2,3,4} returns the number of k-ephemeral numbers i.

## Question 3

A sum and product expression is a statement containing positive integers, brackets and the plus and times operators. A sum and product expression is said to be good if none of the pairs of brackets it contains are redundant. Brackets are redundant if their removal does not affect the calculation that is done.

Write an algorithm that decides whether a sum and product expression is good. Ideally the input should be read just one, from left to right. You can assume

- The input is a correct expression except that it might have redundant brackets i.e. all brackets in the expression are part of a matching pair
- All operators are explicit

## Question 4

This question asks to prove or disprove statements about the complexity of various functions. The details are contained within the PDF file

## Question 5

This question asks to give expressions for runtime by solving using Master Theorem. The details are contained within the PDF file

## Question 6

### Part a

Instead of recursively calling `MergeSort` until the list to be sorted has length 1, we will instead implement `SelectionSort` to sort any list of length 4 or less, and we want the algorithm to output a sorted list from largest to smallest. These algorithms are sometimes known as hybrid sorting algorithms. Provide python code that performs this hybrid `MergeSort` and `SelectionSort` algorithm on an input array A. We will also assume that the input array A contains unique elements, so no element appears more than once, and the length of A is a power of 2.

### Part b

Give an example of a worst case input to this algorithm. That is an input that requires the most comparison operations, along with justification as to why that is the case

### Part c

Now we want to generalise the algorithm to allow a user to enter an input array A of any length, not just a power of two. Provide new Python code to perform this hybrid `MergeSort` and `SelectionSort` algorithm on inputs of any length. We will still assume that the input array A contains unique elements, so no element appears more than once.

### Notes on my code

I implemented the algorithm to work on inputs of any length initially, so my code for part a and c is identical, and in the file `MergeSort.py`
