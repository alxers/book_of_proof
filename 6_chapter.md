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
Suppose there are real number x in [0, pi/2] for which sinx + cosx < 1.     
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
3. Prove that 2^(1/3) is irrational.     
5. Prove that sqrt(3) is irrational.     
6. If a, b in Z. a^2 - 4b - 2 != 0.     

