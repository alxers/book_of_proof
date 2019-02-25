Mathematical Induction.     

Outline for Proof by Induction.     
Proposition The statements S_1, S_2, S_3, ... are all true.     

Proof. (Induction)     
(1) Prove that the first statement S_1 is true.     
(2) Given any integer k >= 1, prove that the statement S_k => S_k+1 is true.     
It follows by mathematical induction that every S_n is true.     


Example:     
Proposition. If n in N, then 1+3+5+7+...+(2n-1) = n^2.     
Proof.     
(1) Observe that if n = 1, this statement is 1 = 1^2, which is true.     
(2) We must prove S_k => S_k+1 for any k >= 1.     
That is if 1+3+5+7+...+(2k - 1) = k^2, then 1+3+5+7+...+(2(k+1) - 1) = (k + 1)^2.     
Direct proof. Suppose 1+3+5+7+...+(2k - 1) = k^2.     
Then 1 + 3 + 5 + 7 + ... + (2 (k + 1) - 1) =       
1 + 3 + 5 + 7 + ... + (2k - 1) + (2 (k + 1) - 1) =     
(1 + 3 + 5 + 7 + ... + (2k - 1)) + (2 (k + 1) - 1) =      
k^2 + (2 (k + 1) - 1) = k^2 + 2k + 1 = (k + 1)^2      
This proves that S_k => S_k+1.     
It follows by induction that 1 + 3 + 5 + 7 + ... + (2n - 1) = n^2 for every n in N.     


Proposition If n is a non-negative integer, then 5 | (n^2 - n).     
(1) If n = 0, 0 = 5x.    
(2) Let k >= 0, we need to prove that if 5 | (k^5 - k), then 5 | ((k+1)^5 - (k+1)).     
k^5 - k = 5x.     
(k + 1)^5 - (k + 1) = k^5 + 5k^4 + 10k^3 + 10k^2 + 5k + 1 - k - 1 =      
= (k^5 - k) + 5(k^4 + 2k^3 + 2k^2 + k) =       
= 5x + 5(...) = 5(x + ...).     
It follows by induction that 5 | (n^5 - n) for all non-negative integers n.     


Proposition For each n in N, it follows that 2^n <= 2^(n+1) - 2^(n-1) - 1.     
(1) If n = 1, then 2 <= 4 - 1 - 1      
(2) Suppose k >= 1. We need to show that 2^k <= 2^(k+1) - 2^(k-1) - 1 implies 2^(k+1) <= 2^(k+2) - 2^k - 1      
2^k <= 2^(k+1) - 2^(k-1) - 1.     
Multiply both sides by 2.     
2^(k+1) <= 2^(k+2) - 2^k - 2.      
Add 1 to the right side (it doesn't change inequation).      
2^(k+1) <= 2^(k+2) - 2^k - 1.     
It follows by induction that 2^n <= 2^(n+1) - 2^(n-1) - 1 for each n in N.     


Proposition 10.1 Suppose a_1, a_2, ... , a_n are n integers, where n >= 2. If p is prime and p | (a_1 * a_2 * a_3 ... * a_n), then p | a_i for at least one of the a_i.     
(1) Basic step. For n = 2. Suppose p | (a_1 * a_2), then p | a_1 or p | a_2. Or p !| a_1 AND p | a_2.      
If p !| a_1 => gcd(p, a_1) = 1.      
Then 1 = pk + a_1l.        
Multiply both sides by a_2.     
a_2 = a_2pk + a_1a_2l.      
p | a_2pk and p | a_1a_2l (by our proposition).      
(2) For k > 2.      
Show that p | (a_1a_2 ... a_k). Suppose p | (a_1a_2 ... a_k * a_k+1).      
By what we proved in basic step it follows that p | (a_1 * a_2 ... a_k) or p | (a_k+1).     



Proof by strong induction.     
Outline.     

Proposition The statements S_1, S_2, S_3, ... are all true.     
Proof (Strong induction)     
(1) Prove the first statement S_1. (Or the first several S_n.)     
(2) Given any integer k >= 1, prove (S_1 ^ S_2 ^ S_3 ^ ... ^ S_k) => S_k+1.     

Somtimes it's difficult to show that S_k forces S_k+1 to be true.     
Instead some "lower" statements S_m (with m < k) force S_k+1 to be true.    
With strong induction in Step (2) instead of assuming S_k is true, we assume that all the statents S_1, S_2, ..., S_k are true and show this forces S_k+1 to be true.     

Example:     
Proposition If n in N, then 12 | (n^4 - n^2)     
(1) Observe, that this statement is true for the first 6 n.      
(2) Let k >= 6, assume 12 | (m^4 - m^2) for 1 <= m <= k. (All statements S_1, S_2, ..., S_k are all true).     
=> m^4 - m^2 = 12a.     
We must show that 12 | ((k+1)^4 - (k+1)^2).     
Since S_k-5 is true, we have 12 | ((k-5)^4 - (k-5)^2).     
Let m = k - 5, k = m + 5.     
(k+1)^4 - (k+1)^2 = (m+6)^4 - (m+6)^2 = ... = (m^4 - m^2) + 24m^3 + 216m^2 + 852m + 1260 =       
= 12a + ... = 12(...).     
We get 12 | ((k+1)^2 - (k+1)^2).     


Graphs     
Is a structure with vertices and edges.    
Cycle is when it's possible to from one distinct vertex to another in a "loop".     
Graphs with no cycles called trees.    
A tree always have n - 1 edges given that there is an n vertices.     

Example:      
Proposition. If a tree has n vertices, then it has n - 1 edges.     
(1) If a tree has n = 1 vertex, then it has no edges.     
(2) We need to show that for k >= 1 it follows that (S_1 ^ S_2 ^ ... ^ S_k) => S_k+1.     
In other words, for all m if there is a tree with m vertices and m - 1 edges (where 1 <= m <= k), then it follows that a tree with k+1 vertices has k + 1 - 1 = k edges.     
Direct proof:     
Suppose for all integers m there are trees with m vertices and m - 1 edges.     
Let T be a tree with k + 1 vertices.      
Single out one edge "e" and remove it.      
We have two trees T_1 and T_2 with x and y vertices (x + y = k + 1).     
Both of those trees have fewer that k + 1 vertices, then by our inductive hypothethis they have x - 1 and y - 1 edges.     
The original tree then has x - 1 + y - 1 + 1 = x + y - 1 edges.     
Since x + y = k + 1, then x + y - 1 = k + 1 - 1 = k edges.     
We've shown that a tree with k + 1 vertices has k edges.      



Proof by smallest conterexample.      
Outline.     

Proposition. The statements S_1, S_2, ... S_n are all true.     

Proof (Smallest conterexample).      
(1) Check that the first statement S_1 is true.     
(2) For the sake of contradiction, suppose not every S_n is true.     
(3) Let k > 1 be the smallest integer for which S_k is false.     
(4) Then S_k-1 is true and S_k is false. Use this to get contradition.     

Example:     
Proposition If n in N, then 4 | (5^n - 1).     
Proof.      
(1) If n = 1, then 4 | (5-1), 4 | 4, which is true.     
(2) Suppose there is a k > 1 for which S_k is false.     
Then for S_k-1 it's true.     
4 | (5^(k-1) - 1).     
5^(k-1) - 1 = 4a.     
5 * 5^(k-1) - 5 = 20a.     
5^k - 1 = 20a + 4.     
5^k - 1 = 4(5a + 1).     
Which means 4 | (5^k - 1).      
Contraditction.      


Example.     
Fundamental theorem of arithmetics.     
Theorem 10.1.     
Any integer n > 1 has a unique prime factorization. That is, if n = p1 * p2 * p3 * ... * pk and n = a1 * a2 * ... al are two prime factorizations of n, then k = l, and the primes p_i and a_i are the same except they may be in a different order.     

Proof:     
Suppose n > 1.     
If n = 2, then it is its own prime factorization.     
Assume, that all integers between 2 and n has prime factorizations.    
Consider n + 1.     
If n + 1 is a prime, then it is its own prime factorizations.      
If n + 1 is not a prime, then n + 1 = ab (a > 1, b > 1).     
a and b are less than n + 1, so they can be represented as:     
a = p1 * p2 * ... * pk, b = a1 * a2 * ... * al.     
Then n = (p1 * p2 * ... * pk)(a1 * a2 * ... * al).     
Uniqueness proof.     
If n = 2, then the factorization is uniq.    
For the sake of contradiction suppose that for n >= 2 n = p1 * ... * pk and n = a1 * ... * al.     
and let n be the smallest integer of this kind.       
Then p1 | n => p1 | (a1 * ... * al).      
p1 | a_i by proposition 10.1.       
Since p1 | a_i and a_i is a prime, then p1 = a_i.      
Divide n by p1 (a_i).      
n = p2 * ... * pk, n = a1 * ... * a_i-1 * a_i+1 * ... * al.     
p2 * ... * pk and a1 * ... * a_i-1 * a_i+1 * ... * al is a different prime factorizations.     
But p2 * ... * pk does not equal n.      
Contradiction.       



Proposition The Fibonacci sequense obeys F^2_(n+1) - F_(n+1) * F_(n) - F^2_(n) = (-1)^n.     
(1) If n = 1, then 1^2 - 1 * 1 - 1^2 = -1 = -1^1.     
(2) Let k >= 1, then if F^2_(k+1) - F_(k+1) * F_(k) - F^2_(k) = (-1)^k, then F^2_(k+2) - F_(k+2) * F_(k+1) - F^2_(k+1) = (-1)^(k+1).      
Note F_(k+2) = F_(k+1) + F_k.      
F^2_(k+2) - F_(k+2) * F_(k+1) - F^2_(k+1) = (F_(k+1) + F_k)^2 - (F_(k+1) + F_k) * F_k+1 - F^2_(k+1) =      
= F^2_(k+1) + 2F_(k+1) * F_k + F^2_k - 2F^2_(k+1) - F_k * F_(k+1) =      
= -F^2_(k+1) + F_(k+1) * F_k + F^2_k =      
= - (F^2_(k+1) - F_(k+1) - F^2_k) =     
= -(-1)^k = -1(-1)^k = (-1)^(k+1).      


Exercises for Chapter 10.      
1. For every integer n in N, it follows that 1 + 2 + ... + n = (n^2 +n)/2.      
Proof.     
(1) If n = 1, then 1 = (1^2 + 1)/2 = 1.      
(2) Let k >= 1, then if 1 + 2 + ... + k = (k^2 + k)/2 then 1 + 2 + ... + k + 1 = ((k + 1)^2 + k + 1)/2.      
((k + 1)^2 + k + 1)/2 = (k^2 + 2k + 1 + k + 1)/2 = ((k^2 + k) + (2k + 2))/2 =      
= (k^2 + k)/2 + 2(k + 1)/2 = (k^2 + k)/2 + (k + 1).     
1 + 2 + ... + k + k + 1 = (k^2 + k)/2 + (k + 1).     
1 + 2 + ... + k = (k^2 + k)/2.       


2. For every integer n in N, it follows that 1^2 + 2^2 + ... + n^2 = (n(n + 1)(2n + 1))/6.       
Proof.     
(1) If n = 1, then 1^2 = 6/6 = 1.     
(2) Let k >= 1. We need show that if 1^2 + 2^2 + ... + k^2 = (k(k + 1)(2k + 1))/6, then 1^2 + 2^2 + ... + (k + 1)^2 = ((k + 1)(k + 2)(2(k + 1) + 1))/6.      
Observe, that (k(k + 1)(2k + 1))/6 = (2k^3 + k^2 + 2k^2 + k)/6.     
Then ((k + 1)(k + 2)(2(k + 1) + 1))/6 = (2k^3 + 3k^2 + 6k^2 + 9k + 4k + 6)/6 = (2k^3 + k^2 + 2k^2 + k)/6 + (6k^2 + 12k + 6)/6.     
Since (2k^3 + k^2 + 2k^2 + k) = (k(k + 1)(2k + 1)), then (2k^3 + k^2 + 2k^2 + k)/6 + (6k^2 + 12k + 6)/6 =      
= (k(k + 1)(2k + 1))/6 + 6(k^2 + 2k + 1)/6 = (k(k + 1)(2k + 1))/6 + (k + 1)^2.      
Then substitute (k + 1)^ from both sides of      
1^2 + 2^2 + ... + (k + 1)^2 = (k(k + 1)(2k + 1))/6 + (k + 1)^2.      
Which is equals 1^2 + 2^2 + ... + k^2 = (k(k + 1)(2k + 1))/6.       
