Chapter 6.     

Proof by contradiction.     


The basic idea is to assume that the statement we want to prove is false, and then show that this assumption leads to nonsense.      

Proposition.     
If a, b in Z, then a^2 - 4b != 2.      


Example:     
If a, b in Z, then a^2 - 4b != 2.     
Suppose this statement is false.     
It means that there exist a, b for which a, b in Z but a^2 - 4b = 2.     
a^2 - 4b = 2.     
a^2 = 2 + 4b = 2(1 + 2b) which is even.     
If a^2 even, then a is even.     
So a = 2x.     
4x^2 - 4b = 2.     
4(x^2 - b) = 2.      
2(x^2 - b) = 1.     
1 is even, which is false.     
So the initial statement is true.     


*Outline for Proof by Contradiction*    
Proposition P.     
Proof. Suppose ∼P.     
.     
.     
Therefore C ^ ∼C.     


*Definition 6.1* A real number x is rational if x = a/b for some a, b in Z.     
Also, x is irrational if it is not rational, that is if x != a/b for every a, b in Z.     


Example:     
The number sqrt(2) is irrational.     
Suppose it's not true, that sqrt(2) is irrational, then it must be rational.     
sqrt(2) = a/b, a, b in Z.     
a and b are not both even, because in this case the a/b could be simplified.     
2 = a^2/b^2.      
a^2 = 2b^2, then a^2 is even, so a is even.     
Then b can't be even, because a and b are not both even.     
a = 2x.     
2 = 4x^2/b^2.     
2b^2 = 4x^2.      
b^2 = 2x^2 which is even, but b can't be even, we have a contradiction.     
Then it must be that the initial statement is true.     



Example:      
There are infinitely many prime numbers.     
Suppose there are finite number of primes.       
Then p_n is the n-th lagrest prime number.      
Lets consider number a, a = (p_1 * p_2 * ... * p_n) + 1.       
Like any natural number > 1, a is divisible by some prime number, p_k, p_k is in the list (p_1 * p_2 * ... * p_n).     
It means that p_k | a, a = p_k * x.     
p_k * x = (p_1 * p_2 * ... * p_k * ... * p_n) + 1.     
p_k * x - 1 = (p_1 * p_2 * ... * p_k * ... * p_n).       
Divide both sided by p_k.       
x - 1/p_k = (p_1 * p_2 * ... * p_n).      
There is a natural number on the right side, but not on the left side.     
This is a contradiction.     



Example:      
For every real number x in [0, pi/2], we have sinx + cosx >= 1.       
Suppose there is real number x in [0, pi/2] for which sinx + cosx < 1.     
The values of sinx and cosx in [0, pi/2] can't be negative.    
0 < sinx + cosx < 1.     
0^2 < (sinx + cosx)^2 < 1^2.      
0 < sin^2(x) + 2sinxcosx + cos^2(x) < 1.     
0 < 2sinxcosx + 1 < 1.      
But sicnce sinx and cosx are not negative, 2sincosx + 1 can't be less than 1.    



Proving conditionals by contradiction.      
Example:      
If P, then Q.    
Proof by contradiction start with assumption that ~(P => Q) is true (or P => Q is false).     
According to the truth table P can be true when Q is false when P => Q is false.     
The first step then is to assume that P is true and Q is false (P and ~Q).     

*Outline for Proving a Conditional*     
Statement with Contradiction     
Proposition     
If P, then Q.     
Proof. Suppose P and ∼ Q.     
.     
.     
Therefore C ^ ∼C.     



Example:     
Suppose a in Z. If a^2 is even, then a is even.     
Suppose a^2 is even and a is odd.     
a = 2x + 1.     
a^2 = a * a = (2x + 1)^2 = 4x^2 + 4x + 1 = 2(2x^2 + 2x) + 1.     
So a^2 is odd and a^2 is even, contraditcion.     



Example:      
If a, b in Z and a >= 2, then a !| b, or a !| (b + 1).       
Suppose it's not true that a !| b or a !| b + 1.     
By DeMorgan's law  not ((a !| b) or (a !| b + 1)) is equal to not (a !| b) and not ((a !| b + 1)).     
Which is the same as a | b and a | (b + 1).     
Then it must be that b = ax and b + 1 = ay.      
b + 1 = ay divided by b = ax is equal to 1 = ay - ax.     
a(y - x) = 1.     
a is positive, (y - x) is also positive (otherwise a would be negative).     
a = 1/(y - x) which is less than 2.     
So a >=2 and a < 2. Contradiction.     




Example:     
Every non-zero rational number can be expressed as a product of two irrational numbers.       
In other words, if r is a non-zero rational number, then r is a product of two irrational numbers.     
Direct proof.     
Suppose r is a non-zero rational number. Then r = a/b for integers a and b.     
r can be writte as r = sqrt(2) * (r/sqrt(2)).     
sqrt(2) is irrational, we must show that r/sqrt(2) also irrational.     
Assume for the sake of contradicton, that r/sqrt(2) is rational.     
This means r/sqrt(2) = c/d.     
sqrt(2) = r * (d/c).     
But r = a/b.     
sqrt(2) = ad/bc which means sqrt(2) is rational.     
Contradiction.     
Therefore r/sqrt(2) is irrational.     
Consequently r = sqrt(2) * (r/sqrt(2)) is a product of two irrational numbers.      



Exercises for Chapter 6.      
A. Use the method of proof by contradiction to prove the following statements.     


1. Suppose n in Z. If n is odd, then n^2 is odd.     
Suppose n is odd and n^2 is even.     
n = 2x + 1.     
n^2 = (2x + 1)^2 = 4x^2 + 4x + 1 = 2(2x^2 + 2x) + 1 which is odd.     
Contradiction.     



3. Prove that 2^(1/3) is irrational.     
Suppose 2^(1/3) is rational, then 2^(1/3) = a/b.     
a/b is a reduced fraction (a and b can't be both even, otherwise we'd factor out 2 and cancel).     
(2^(1/3))^3 = (a/b)^3.     
2 = (a^3)/(b^3).     
2b^3 = a^3.     
a^3 is even.     
Then a is even (a = 2x, a^3 = 8x^3 = 2(4x^3)).     
Then 2b^3 = 8x^3.     
b^3 = 4x^3.     
b^3 = 2(2x^3).     
b^3 is even, then b is even (same reasoning as for a).     
Contradiction.    


5. Prove that sqrt(3) is irrational.      



6. If a, b in Z. a^2 - 4b - 2 != 0.     
Suppose a^2 - 4b - 2 = 0.     
a^2 = 4b + 2 = 2(2b + 1).     
a^2 is even, then a is even.     
So a = 2x.     
4x^2 - 4b - 2 = 0.     
2x^2 - 2b - 1 = 0.     
2(x^2 - b) = 1.    
1 is even, contradiction.     



8. Suppose a, b, c in Z . If a^2 + b^2 = c^2, then a or b is even.      
Suppose a^2 + b^2 = c^2 and not (a or b).      
By DeMorgan's law not (a or b) = not a and not b.     
So a and b are odd.     
a = 2x + 1, b = 2y + 1.     
(2x + 1)^2 + (2y + 1)^2 = c^2.     
4x^2 + 4x + 1 + 4y^2 + 4y + 1 = c^2.     
2(2x^2 + 2x + 2y^2 + 2y + 1) = c^2.     
c^2 is even, c is even.     
c = 2z
???


9. Suppose a, b in R . If a is rational and ab is irrational, then b is irrational.     
Suppose b is rational, b = x/y for some integers x, y.     
Since a is rational, a = k/m for some integers k, m.     
ab = (k/m) * (x/y).     
Since k, m, x and y are integers, ab is rational.     
Contradiction.     



10. There exist no integers a and b for which 21a + 30b != 1.          
???



11. There exist no integers a and b for which 18a + 6b != 1.    
Suppose 18a + 6b = 1.      
2(9a + 3b) = 1.     
Then a is even.     
Contradiction.     


12. For every positive x in Q, there is a positive y in Q for which y < x.     
Suppose y >= x.     
Since y is a positive number in Q, let y = x/2.     
Then x/2 >= x, contradiction.     


13. For every x in [pi/2, pi], sinx - cos x >= 1.     
Suppose sinx - cosx < 1.     
sinx >= 0 in [pi/2, pi].     
cosx <= 0 in [pi/2, pi].     
sinx - cosx >= 0 in [pi/2, pi].      
0 <= sinx - cosx < 1.     
Square all sides, 0^2 <= (sinx - cosx)^2 < 1^2.     
0 <= sin^2(x) - 2sinxcosx + cos^2(x) < 1.     
0 <= 1 - 2sinxcosx < 1.     
-2sinxcosx >= 0, cosx <= 0, sinx >= 0.     
1 + (-2sinxcosx) >= 1.     
Contradiction.     


14. If A and B are sets, then A intersect (B - A) = empty_set.   
Suppose A intersect (B - A) != empty_set.     
If it's not empty, then there is an a in (A intersect (B - A)).     
Since it's an intersection, then a in A AND a in (B - A).     
But a not in (B - A).     
Contradiction.     



15. If b in Z and b !| k for every k in N, then b = 0.     
Suppose b != 0.     
Case 1. b > 0, then b in N.     
Then it's not true that b !| k, contradiction.     
Case 2. b < 0, then -b in N.     
Then it's not true that b !| k, contradiction.     



16. If a and b are positive real numbers, then a + b >= 2sqrt(ab).     
Suppose a + b < 2 sqrt(ab).     
Since a and b are positive we can square both sides.     
(a + b)^2 < 4ab.     
a^2 + 2ab + b^2 < 4ab.     
a^2 -2ab + b^2 < 0.     
(a - b)^2 < 0.     
Squared number can't be negative, contraditcion.      


 
