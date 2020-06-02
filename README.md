# ADS Coursework
This is my solution for the coursework set for the Algorithms and Data Structures Module at Durham University
The questions were as follows:
## Question 1
Produce python code to add keys to a hash table. You must create the code for two functions `hash_quadratic` and `hash_double` that add keys (we ignore the values) to a hash table of size 19 using the hash function defined by *h(k)=6k+3 mod 19*. In `hash_quadratic` collisions should be handled by probing. In `hash_double` collisions should be handled using Double Hashing using the secondary hash function *h'(k)=11-(k mod 11)*. The input to the functions is a list of keys (positive integers) to add to the hash table and the output is the contents of the table where the symbol "-" indicated a bucket in the array containing no data. You can assume the input contains no duplicates.

## Question 2
Let k be 2,3 or 4. The k-child of a positive integer is defined to be a number obtained by taking the kth power of each digit and adding them. For example the 2 child of 19 is 1<sup>2</sup>+9<sup>2</sup>=82. The k-descendant sequence of a positive integer begins with the integer and then each successive term is the k-child of the previous one. The sequence terminates if it reaches a 1 or a term is repeated.

A positive integer is k-ephemeral if its k-descendant sequence ends in 1, and otherwise it is k-eternal.

Write a function called `count_ephemeral(n1,n2,k)` which, given two positive integers n<sub>1</sub> and n<sub>2</sub>, n<sub>1</sub>< n<sub>2</sub>, and k in {2,3,4} returns the number of k-ephemeral numbers i.
