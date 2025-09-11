<img width="978" height="662" alt="image" src="https://github.com/user-attachments/assets/5b02256c-b74f-483d-964b-6c1b6898ad97" />*******All divisors of a Number

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

----------------------------------------------------------------------------------------------------------------------------------------------------------------------
🧮 Sieve of Eratosthenes - Notes
✅ Introduction

The Sieve of Eratosthenes is an efficient algorithm to find all prime numbers up to a given limit n.
Instead of checking primality of each number individually, it eliminates the multiples of primes in a systematic way.

⚡ Algorithm Steps

1.Create a boolean array isPrime[0..n] and initialize all entries as true.
(isPrime[i] = true means i is assumed to be prime initially).

2.Mark 0 and 1 as not prime.

3.Start with the first prime p = 2.

4.For each prime p, mark all multiples of p (i.e., 2p, 3p, 4p ...) as not prime.

    Optimization: Start marking from p * p, because all smaller multiples of p would already be marked by smaller primes.

5.Move to the next number which is still true in isPrime[]. Repeat until p * p <= n.

The remaining numbers with isPrime[i] = true are primes.
<img width="978" height="662" alt="image" src="https://github.com/user-attachments/assets/56734345-14ff-4e9e-b635-46cde1dd5d98" />
