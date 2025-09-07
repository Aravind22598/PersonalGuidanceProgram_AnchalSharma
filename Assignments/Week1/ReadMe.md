*******All divisors of a Number

Given an integer n, print all the divisors of N in the ascending order.
 
Examples:

Input : n = 20
Output: 1 2 4 5 10 20
Explanation: 20 is completely divisible by 1, 2, 4, 5, 10 and 20.
Input: n = 21191
Output: 1 21191
Explanation: As 21191 is a prime number, it has only 2 factors(1 and the number itself).
Constraints:
1 ≤ n ≤ 109

Expected Complexities
Time Complexity: O(sqrt(n)
Auxiliary Space: O(sqrt(n))

My Notes:  This question i initially know how to find factors in o(sqrt(n)) time but here the trick is how to print the divisors in ascending order.
           so i initially printed small factors(i) and stored (n/i) factors in array list and later on i traversed array list in reverse and printed all the factors
