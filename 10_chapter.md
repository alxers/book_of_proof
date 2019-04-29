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
.1. For every integer n in N, it follows that 1 + 2 + ... + n = (n^2 +n)/2.      
Proof.     
(1) If n = 1, then 1 = (1^2 + 1)/2 = 1.      
(2) Let k >= 1, then if 1 + 2 + ... + k = (k^2 + k)/2 then 1 + 2 + ... + k + 1 = ((k + 1)^2 + k + 1)/2.      
((k + 1)^2 + k + 1)/2 = (k^2 + 2k + 1 + k + 1)/2 = ((k^2 + k) + (2k + 2))/2 =      
= (k^2 + k)/2 + 2(k + 1)/2 = (k^2 + k)/2 + (k + 1).     
1 + 2 + ... + k + k + 1 = (k^2 + k)/2 + (k + 1).     
1 + 2 + ... + k = (k^2 + k)/2.       


.2. For every integer n in N, it follows that 1^2 + 2^2 + ... + n^2 = (n(n + 1)(2n + 1))/6.       
Proof.     
(1) If n = 1, then 1^2 = 6/6 = 1.     
(2) Let k >= 1. We need show that if 1^2 + 2^2 + ... + k^2 = (k(k + 1)(2k + 1))/6, then 1^2 + 2^2 + ... + (k + 1)^2 = ((k + 1)(k + 2)(2(k + 1) + 1))/6.      
Observe, that (k(k + 1)(2k + 1))/6 = (2k^3 + k^2 + 2k^2 + k)/6.     
Then ((k + 1)(k + 2)(2(k + 1) + 1))/6 = (2k^3 + 3k^2 + 6k^2 + 9k + 4k + 6)/6 = (2k^3 + k^2 + 2k^2 + k)/6 + (6k^2 + 12k + 6)/6.     
Since (2k^3 + k^2 + 2k^2 + k) = (k(k + 1)(2k + 1)), then (2k^3 + k^2 + 2k^2 + k)/6 + (6k^2 + 12k + 6)/6 =      
= (k(k + 1)(2k + 1))/6 + 6(k^2 + 2k + 1)/6 = (k(k + 1)(2k + 1))/6 + (k + 1)^2.      
Then substitute (k + 1)^2 from both sides of      
1^2 + 2^2 + ... + (k + 1)^2 = (k(k + 1)(2k + 1))/6 + (k + 1)^2.      
Which is equals 1^2 + 2^2 + ... + k^2 = (k(k + 1)(2k + 1))/6.       



.3. For every integer n in N, it follows that 1^3 + ... + n^3 = (n^2(n + 1)^2)/4.     
(1) If n = 1 then 1^3 = (1(1 + 1)^2)/4 = 4/4 = 1.     
(2) Let k >= 1, we need to show that if 1^3 + 2^3 + ... + k^3 = (k^2(k + 1)^2)/4, then 1^3 + 2^3 + ... + (k + 1)^3 = ((k + 1)^2 * (k + 2)^2)/4.      
Observe that k^2 * (k + 1)^2 = k^2 * (k^2 + 2k + 1) = k^4 + 2k^3 + k^2.     
Since (k^2(k + 1)^2)/4 = ((k^2 + 2k + 1)(k^2 + 4k + 4))/4 = (k^4 + 4k^3 + 4k^2 + 2k^3 + 8k^2 + 8k + k^2 + 4k + 4)/4.    
(k^4 + 2k^3 + k^2)/4 + (4k^3 + 4k^2 + 8k^2 + 8k + 4k + 4)/4.     
As we observed k^2 * (k + 1)^2 = k^2 * (k^2 + 2k + 1) = k^4 + 2k^3 + k^2 then     
(k^4 + 2k^3 + k^2)/4 + (4k^3 + 4k^2 + 8k^2 + 8k + 4k + 4)/4 =     
(k^2 * (k + 1)^2)/4 + 4(k^3 + k^2 + 2k^2 + 2k + k + 1)/4 =      
(k^2 * (k + 1)^2)/4 + (k^3 + 3k^2 + 3k + 1) =     
(k^2 * (k + 1)^2)/4 + (k + 1)^3.     
Substitute (k + 1)^3 from both sides.     
1^3 + 2^3 + ... + k^3 = (k^2(k + 1)^2)/4.     



.4. If n in N, then 1 * 2 + 2 * 3 + ... + n * (n + 1) = (n(n + 1)(n + 2))/3.     
(1) If n = 1, 1 * (1 + 1) = (1 * (1 + 1) * (1 + 2))/3.     
2 = 6/3.      
(2) Let k >= 1, we need to show that if 1 * 2 + 2 * 3 + ... + (k + 1) * (k + 2) = ((k + 1)(k + 1 + 1)(k + 1 + 2))/3 then 1 * 2 + 2 * 3 + ... + k * (k + 1) = (k(k + 1)(k + 2))/3.     
Observe that k(k + 1)(k + 2) = k(k^2 + 3k + 2) = k^3 + 3k^2 + 2k.     
((k + 1)(k + 2)(k + 3))/3 = ((k^2 + 3k + 2)(k + 3))/3 = (k^3 + 3k^2 + 3k^2 + 9k + 2k +6)/3      
Note that k^3 + 3k^2 + 3k^2 + 9k + 2k +6 = k^3 + 3k^2 + 2k + 3k^2 + 9k + 6.    
Since k^3 + 3k^2 + 2k = k(k + 1)(k + 2), then     
(k^3 + 3k^2 + 3k^2 + 9k + 2k +6)/3 = (k + 1)(k + 2)/3 + 3(k^2 + 3k + 2)/3 =       
= k(k + 1)(k + 2)/3 + (k^2 + 3k + 2) = k(k + 1)(k + 2)/3 + (k + 1)(k + 2).  
So 1 * 2 + 2 * 3 + ... + (k + 1) * (k + 2) = k(k + 1)(k + 2)/3 + (k + 1)(k + 2)     
Substitute (k + 1)(k + 2) from both sides we get 1 * 2 + 2 * 3 + ... + k * (k + 1) = (k(k + 1)(k + 2))/3.        


.5. If n in N, then 2^1 + 2^2 + 2^3 + ... + 2^n = 2^(n+1) - 2.     
(1) If n = 1, 2^1 = 2^2 - 2, 2 = 2.     
(2) Let k >= 1, show that if 2^1 + 2^2 + 2^3 + ... + 2^(k+1) = 2^(k+2) - 2 then 2^1 + 2^2 + 2^3 + ... + 2^k = 2^(k+1) - 2.     
2^(k+2) - 2 = 2^(k+1) * 2 - 2.     
Divide both sides by 2.      
1^1 + 2^1 + 2^(k-1) + ... + 2^k = 2^(k+1) - 1.     
Substitute 1 from both sides.     
2^1 + 2^2 + ... + 2^k = 2^(k+1) - 2.     



.6. For every natural number n, it follows, that SUM(i=1, n)(8i - 5) = 4n^2 - n.     
(1) If n = 1, then 8 - 5 = 4 - 1.     
(2) Let k >= 1, show that SUM(i=1, k+1)(8i - 5) = 4(k+1)^2 - (k+1) then SUM(i=1, k)(8i - 5) = 4k^2 - k.     
4(k^2 + 2k + 1) - k - 1 = 4k^2 + 8k + 4 - k - 1.     
4k^2 - k + 8k + 3.     
SUM(i=1, k+1)(8i - 5) = (8 - 5) + (16 - 5) + ... + (8k - 5) + 8(k+1) - 5.     
8k + 8 - 5 = 8k + 3.     
Substitute 8k + 3 from both sides.     
(8 - 5) + ... + (8k - 5) = 4k^2 - k = SUM(i=1, k)(8i - 5).     


.7. If n in N, then 1 * 3 + 2 * 4 + ... + n(n + 2) = (n(n + 1)(2n + 7))/6.     
(1) If n = 1, then 3 = (1 * 2 * 9)/6 = 3.      
(2) Let k >= 1, show that if 1 * 3 + 2 * 4 + ... + (k + 1)(k + 1 + 2) = ((k + 1)(k + 1 + 1)(2(k + 1) + 7))/6, then 1 * 3 + 2 * 4 + ... + k(k + 2) = (k(k + 1)(2(k + 1) + 7))/6.        
Observe that (k(k + 1)(2k + 7)) = (k^2 + k)(2k + 7) = 2k^3 + 9k^2 + 7k.     
(k(k + 1)(2(k + 1) + 7))/6 = ((k^2 + 3k + 2)(2k + 9))/6 = (2k^3 + 9k^2 + 6k^2 + 27k + 4k + 18)/6 = (2k^3 + 9k^2 + 7k   +    6k^2 + 24k + 18)/6 = (2k^3 + 9k^2 + 7k)/6 + 6(k^2 + 4k + 3)/6.      
(k^2 + 4k + 3) = (k + 1)(k + 1 + 2).      
Subtract (k + 1)(k + 1 + 2) from both sides.       
We get 1 * 3 + 2 * 4 + ... + k(k + 2) = (k(k + 1)(2(k + 1) + 7))/6.   


.8. If n in N, then 1/2! + ... + n/(n + 1)! = 1 - 1/(n + 1)!.      
(1) n = 1, 1/2! = 1 - 1/2!.      
(2) Let k >= 1, show that if 1/2! + ... + (k + 1)/(k + 1 + 1)! = 1 - 1/(k + 1 + 1)!, then 1/2! + ... + k/(k + 1)! = 1 - 1/(k + 1)!.      
Observe, that (k + 2)! = k!(k + 1)(k + 2).      
1/2! + ... + (k + 1)/(k + 2)! = 1 - 1/k!(k + 1)(k + 2).      
1/2! + ... + k/(k + 1)! (k + 1)/k!(k + 1)(k + 2) + 1/k!(k + 1)(k + 2) = 1.      
1/2! + ... + k/(k + 1)! + (k + 2)/k!(k + 1)(k + 2) = 1.      
1/2! + ... + k/(k + 1)! = 1 - 1/(k + 1)!.       


.9. For any integer n >= 0, it follows that 24 | (5^(2n) - 1).      
(1) If n = 0, then 24 | 0.      
(2) Let k >= 1, show that if 24 | (5^(2k) - 1), then 24 | (5^(2k + 2) - 1).      
Observe that 5^2k - 1 = 24a, 5^2k = 24a + 1.     
Suppose 24 | (5^(2k + 2) - 1).     
Then (5^(2k + 2) - 1) = 24a.      
5^2 * 5^2k - 1 = 24a.     
25(24a + 1) - 1 = 24a.     
25 * 24a + 25 - 1 = 24a.     
25 * 24a + 24 = 24a.     
24(25a + 1) = 24a.     


.10. For any integer n >= 0, it follows that 3 | (5^2n - 1).     
(1) If n = 0, 3 | (1 - 1).      
(2) Let k >= 1, show that if 3 | (5^2k - 1), then 3 | (5^(2k + 2) - 1).     
Suppose 3 | (5^2k - 1), then 5^2k = 3a + 1.      
5^(2k + 2) - 1 = 3a.      
5^2k * 5^2 - 1 = 3a.       
(3a + 1) * 5^2 - 1 = 75a + 25 - 1 =      
= 75a + 24 = 3(25a + 6).      
Then 5^(2k + 2) - 1 = 3b, then 3 | (5^(2k + 2) - 1).      


.11. For any integer n >=, it follows that 3 | (n^3 + 5n + 6).     
(1) n = 1, 3 | (1 + 5 + 6), 3 | 12.      
(2) Let k >= 1, show that if 3 | ((k + 1)^3 + 5(k + 1) + 6), then 3 | (k^3 + 5k + 6).      
(k + 1)^3 + 5(k + 1) + 6 = (k^2 + 2k + 1)(k + 1) + 5k + 5 + 6 = k^3 + k^2 + 2k^2 + 2k + k + 1 + 5k + 5 + 6 = k^3 + 5k + 6    +    3k^2 + 3k + 6.      
Observe that 3k^2 + 3k + 6 = 3(k^2 + k + 2).      
Since 3 | k^3 + 5k + 6 and 3 | 3(k^2 + k + 2), then 3 | k^3 + 5k + 6 + 3k^2 + 3k + 6.       


.12. For any into n >= 0, it follows that 9 | (4^3n + 8).      
(1) If n = 0, then 9 | (1 + 8).      
(2) For the sake of contradiction suppose it's not true, that 9 | (4^3n + 8) for all n.      
Let k > 1 be the smalles integer for which 9 !| (4^3k + 8).     
Then 9 | (4^(3(k - 2)) + 8).     
4^(3k + 3) + 8 = 9a.      
4^3(4^(3k - 3) + 8) = 4^3 * 9a.      
4^3k + 4^3 * 8 = 4^3 * 9a.      
4^3k + 4^3 * 8 = 4^3 * 9a.      
4^3k + 512 = 64 * 9a.      
4^3k + 8 = 64 * 9a - 504.       
4^3k + 8 = 9(64a - 56).      
4^3k + 8 = 9b => 9 | 4^3k + 8. Contradiction.     


.13. For any integer n >= 0, it follows that 6 | (n^3 - n).      
(1) If n = 1, then 6 | (1 - 1).      
n = 2, 8 - 2 = 6, 6 | 6.     
n = 3, 27 - 3 = 24, 6 | 24.     
n = 4, 4^3 - 4 = 60, 6 | 60.     
n = 5, 5^3 - 5 = 120, 6 | 120.     
n = 6, 6^3 - 6 = 210, 6 | 210.     
(2) Let k >= 6, show that if 6 | ((k + 1)^3 - (k + 1)), then 6 | (k^3 - k).     
Let m = k - 5 (S_(k-5) is true).     
(k + 1)^3 - (k + 1) = (m + 6)^3 - (m + 6) =       
(m^2 + 12m + 36)(m + 6) - m - 6 =      
m^3 + 6m^2 + 12m^2 + 12 * 6m + 36m + 36 * 6 - m - 6 =       
(m^3 - m) + 18m^2 + 6(12m + 6m) + 210 =      
6a + 18m^2 + 6(18m) + 6 * 35 =      
6(a + 3m^2 + 18m + 35).       


.14. Suppose a in Z. Prove that 5 | 2^n * a implies 5 | a for any n in N.     
(1) If n = 0, then 5 | a implies that 5 | a.     
(2) Let k >= 1, show that if 5 | 2^k * a implies that 5 | a, then 5 | 2^(k + 1) * a implies that 5 | a.     


.15. If n in N, then 1/(1 * 2) + 1/(2 * 3) + ... + 1/(n(n + 1)) = 1 - 1/(n + 1).     
(1) If n = 1, then 1/2 = 1 - 1/2.     
(2) Let k >= 1, show that if 1/(1 * 2) + 1/(2 * 3) + ... + 1/(k(k + 1)) = 1 - 1/(k + 1), then 1/(1 * 2) + 1/(2 * 3) + ... + 1/((k + 1)(k + 2)) = 1 - 1/(k + 2).       
Observe, that 1/((k + 1)(k + 2)) = 1 - 1/(k + 2).      
1/((k + 1)(k + 2)) + 1/(k + 2) = (1 + k + 1)/((k + 1)(k + 2)) = (k + 2)/((k + 1)(k + 2)) = 1/(k + 1).       
Then 1/(1 * 2) + 1/(2 * 3) + ... + 1/(k(k + 1)) + 1/(k + 1) = 1.     
1/(1 * 2) + 1/(2 * 3) + ... + 1/(k(k + 1)) = 1 - 1/(k + 1).     


.16. For every natural number n, it follows that 2^n + 1 <= 3^n.      
(1) If n = 1, then 2 + 1 <= 3.       
(2) Let k >= 1. Show that if 2^k + 1 <= 3^k, then 2^(k + 1) + 1 <= 3^(k + 1).      
Suppose 2^k + 1 <= 3^k.      
2(2^k + 1) <= 3^k * 2.      
2^(k + 1) + 2 <= 3^k * 2, divide rhs by 3/2.      
2^(k + 1) + 2 <= 3^k * 3.      
2^(k + 1) + 1 <= 3^k * 3 - 1, add 1 to the rhs.     
2^(k + 1) + 1 <= 3^(k + 1).     

.17. Suppose A_1, ... A_n are sets in some universal set U, and n >= 2. Prove that (A_1 intersection ... A_n)(complement) = A_1(complement) union ... A_n(complement).      
(1) If n = 2, then we should prove that (A_1 intersection A_2)(complement) = A_1(complement) union A_2(complement).    
(A_1 intersection A_2)(complement) = (x in U) ^ (x not_in A_1 intersection A_2) = x in U ^ ~ (x in A_1 intersection A_2) =     
= x in U ^ (x not_in A_1) v (x not_in A_2) = (x in U ^ x not_in A_1) v (x in U ^ x not_in A_2) = A_1(compliment) union A_2(compliment)      
(2) (A_1 intersection ... A_k)(complement) =     
(A_1 intersection ... (A_k intersection A_k+1))(complement) =     
A_1(complement) union ... (A_k(complement) union A_k+1(complement))     


.18. Suppose A_1, ... A_n are sets in some universal set U, and n >= 2. Prove that (A_1 union ... A_n)(complement) = A_1(complement) intersection ... A_n(complement).  
(1) If n = 2, then we should prove that (A_1 union A_2)(complement) = A_1(complement) intersection A_2(complement).      
(A_1 union A_2)(complement) =       
(x in U) ^ (x not_in (A_1 union A_2)).  (definition of complement)          
(x in U) ^ ~ (x in (A_1 union A_2)).      
(x in U) ^ ~ (x in A_1 v x in A_2)). (definition of union)       
(x in U) ^ (x not_in A_1 ^ x not_in A_2). (DeMorgan's law)      
(x in U ^ x not_in A_1) ^ (x in U ^ x not_in A_2) => A_1(complement) intersection A_2(complement).     
(2) (A_1 union ... A_k)(complement) =     
(A_1 union ... (A_k union A_k+1))(complement) =     
A_1(complement) intersection ... (A_k(complement) intersection A_k+1(complement))     


.19. Prove that 1 + 1/4 + 1/9 + ... 1/n^2 <= 2 - 1/n.     
(1) If n = 1, then 1 <= 2 - 1.    
(2) Let k >= 1, show that if 1 + 1/4 + ... + 1/(k + 1)^2 <= 2 - 1/(k + 1), then 1 + 1/4 + ... + 1/k^2 <= 2 - 1/k.     
Suppose 1 + 1/4 + 1/9 + ... 1/k^2 <= 2 - 1/k is true.     
Add 1/(k+1)^2 to both sides.    
1 + 1/4 + 1/9 + ... 1/k^2 + 1/(k + 1)^2 <= 2 - 1/k + 1/(k + 1)^2.      
2 - 1/k + 1/(k + 1)^2 = 2 + (k - (k + 1)^2)/k(k + 1)^2 =     
2 - ((k + 1)^2 - k)/(k(k + 1)^2) = 2 - (k^2 + 2k + 1 -k)/(k(k + 1)^2) =     
2 - (k^2 + k + 1)/(k(k + 1)^2) < 2 - (k^2 + k)/(k(k + 1)^2) =     
2 - (k(k + 1))/(k(k + 1)^2) = 2 - 1/(k + 1).     

.20. Prove that (1 + 2 + 3 + ... + n)^2 = 1^3 + 2^3 + 3^3 + ... + n^3 for every n in N.     
(1) If n = 1, then 1^2 = 1^3.     
(2) Let k >= 1. Show that if (1 + 2 + ... + k) = 1^3 + 2^3 + ... + k^3, then (1 + 2 + ... + k + 1)^2 = 1^3 + 2^3 + ... + (k + 1)^3.     


.21. If n in N, then 1 + 1/2 + ... + 1/(2^n - 1) + 1/2^n >= 1 + n/2.      


.25. Concerning the Fibonacci sequence, prove that F_1 + F_2 + ... + F_n = F_n+2 - 1.      
(1) If n = 1, 1 = 2 - 1.     
(2) Let k >= 1, then if F_1 + F_2 + ... + F_(k+1) = F_k+3 - 1, then F_1 + F_2 + ... + F_k = F_k+2 - 1.      
Observe, that F_k+3 = F_k+2 + F_k+1 - 1.     
Subtract F_k+1 from both sides we get F_1 + F_2 + ... + F_k = F_k+2 - 1.     


.26. Concerning the Fibonacci sequence, prove that SUM(from k = 1 to n) (F_k)^2 = F_n * F_(n + 1).      
(1) If n = 1, then 1^2 = 1 * 1.      
(2) Let m >= 1, show that if SUM(from k = 1 to m) (F_k)^2 = F_m+1 * F_m+2 then SUM(from k = 1 to m) = F_m * F_m+1.     
(F_1)^2 + (F_2)^2 + ... + (F_m)^2 = F_m+1 * F_m+2.      
Observe, that (F_m+2) = F_m + F_m+1.      
F_(m+1) * F_(m+2) = F(m+1)(F_m + F(m+1)) = F_m * F_(m+1) + F(m+1)^2.      
Then (F_1)^2 + (F_2)^2 + ... + (F_m)^2 = F_m+1 * F_(m+1)^2.     
Subtract F_(k+1)^2 from both sides.      
(F_1)^2 + (F_2)^2 + ... + (F_m)^2 = F_m * F_m+1.     


.27. Concerning the Fibonacci sequence, prove that (F_1) + (F_3) + ... + F(2n-1) = F_2n.     
(1) n = 1, then F_1 = F_2, 1 = 1.      
(2) SUM(from k = 1 to n) F_(2n-1) = F_2n, SUM(from k = 1 to n+1) F_(2n + 2) = F_(2n+1) + SUM(from k = 1 to n) F_(2n-1).     
F_(2n+1) + F_2n = F_2(n+1).      


.28. Prove that F_2 + F_4 + F_6 + ... + F_2n = F(2n+1) - 1.      
(1) n = 1, F_2 = F_3 - 1, 1 = 1.      
(2) SUM(from k=1 to n) F_2n = F_(2n+1) - 1.      
SUM(from k=1 to n+1) = F_(2n+2) + SUM(from k=1 to n) F_2n = F_(2n+2) + F_(2n+1) - 1 = F_(2n+3) - 1.      


.31. ? Prove that SUM(from k=0 to n) = (n + 1) choose (r + 1), where 1 <= r <= n.      
(1) When n = 0, then 0 choose r = 1 choose (r + 1) (? no such r).      
(2) Show that if SUM(from k=0 to n) = (n + 1) choose (r + 1) then SUM(from k=0 to n+1) = (n + 1 + 1) choose (r + 1).     
Assume SUM(from k=0 to n) = (n + 1) choose (r + 1).     
Observe that (n + 1 + 1) choose (r + 1) = (n + 1) choose (r) + (n + 1) choose (r + 1).     
(n + 1) choose (r) + SUM(from k=0 to n) (k choose r) = SUM(from k=0 to n + 1) (k choose r).     
??? (Check if correct).     



.33. Suppose n(infinitely long) straight lines lie on a plane in such a way that no two of the lines are parallel, and no three of the lines intersect at a single point. Show that this arrangement divides the plane into (n^2 + n + 2)/2 regions.     

(1) If n = 1, then (1^2 + 1 + 2)/2 = 2.     
(2) Since (n^2 + n + 2)/2 is true for n, let's add n + 1.     
(n^2 + n + 2)/2 + n + 1 = (n^2 + n + 2)/2 + (2n + 2)/2 =      
= (n^2 + 2n + 1 + n + 1 + 2)/2 = ((n + 1)^2 + n + 1 + 2)/2.      


.34. Prove that 3^1 + 3^2 + ... + 3^n = (3^(n+1) - 3)/2 for all n in N.     
(1) n = 1, 3^1 = (3^2 - 3)/2 = 3.     
(2) Let k >= 1, show tat if 3^1 + 3^2 + ... + 3^k = (3^(k+1) - 3)/2, then 3^1 + 3^2 + ... + 3^(k+1) = (3^(k+2) - 3)/2.      
3^1 + 3^2 + ... + 3^(k+1) = (3^(k+2) - 3)/2.     
3^1 + 3^2 + ... + 3^(k+1) = (3^(k+1) * 3 - 3)/2.     
3^1 + 3^2 + ... + 3^(k+1) = 3(3^(k+1) - 1)/2.      
3^0 + 3^1 + ... + 3^k = (3^(k+1) - 1)/2 (divide both sides by 3).           
Since 3^0 = 1, subtract 1 from both sides.     
3^1 + ... + 3^k = (3^(k+1) - 1)/2 - 1.        
3^1 + ... + 3^k = (3^(k+1) - 1)/2 - 2/2.        
3^1 + ... + 3^k = (3^(k+1) - 3)/2.        


.35. Prove that if n, k in N, and n is even and k is odd, then (n choose k) is even.     
(1) Let n = 2, k = 1, then (n choose k) = 2!/(1! (2 - 1)!) = 2. 2 is even.     
(2)
