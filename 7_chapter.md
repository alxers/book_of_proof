Chapter 7.     


Proving Non-Conditional Statements.     


7.1 If-and-Only-If Proof.      

This statement asserts that both of the     
following conditional statements are true:     
If P, then Q.     
If Q, then P.     



Outline for If-and-Only-If Proof     
Proposition     
P if and only if Q.     
Proof.     
[Prove P => Q using direct, contrapositive or contradiction proof.]     
[Prove Q => P using direct, contrapositive or contradiction proof.]     


Proposition     
The integer n is odd if and only if n^2 is odd.    

(Direct). Suppose n is odd, then n = 2a + 1 by definition of an odd number.     
Then n^2 = (2a + 1)^2 = 4a^2 + 4a + 1.     
4a^2 + 4a + 1 = 2(2a^2 + 2a) + 1 which is odd.     

Conversely we need to prove that n^2 being odd implies that n is odd.      
(Contrapositive). Suppose n is not odd, then n is even, n = 2a.     
n^2 = 4a^2 = 2(2a^2) which is even.     
So n^2 is even. This is contrapositive proof that if n^2 is odd then n is odd.      


Proposition Suppose a and b are integers. Then a ≡ b (mod 6) if and only if a ≡ b (mod 2) and a ≡ b (mod 3).        
Proof. First we prove that a ≡ b (mod 6).     
Suppose a ≡ b (mod 6), then 6 | (a - b).     
(a - b) = 6x.     
(a - b) = 2(3x), which means 2 | (a - b), a ≡ b (mod 2).     
(a - b) = 3(2x), which means 3 | (a - b), a ≡ b (mod 3).     

Suppose a ≡ b (mod 2) and a ≡ b (mod 3).     
2 | (a - b), (a - b) = 2y.    
So (a - b) is even.     
3 | (a - b), (a - b) = 3z.     
Since (a - b) is even, then 3z must be even too.     
z is even, otherwise a - b would be odd as product of two odd numbers.     
z = 2r for some integer r.     
a - b = 3z = 3 * 2r = 6r.     
Thus 6 | (a - b), a ≡ b (mod 6).     



*7.2 Equivalent Statements*     
Example:     
Theorem Suppose A is an n * n matrix. The following statements are equivalent:     
(a) The matrix A is invertible.     
(b) The equation Ax = b has a uniq solution for every b in R^n.     
(c) The equation Ax = 0 has only the trivial solution.     
(d) The reduced row echelon form of A is I_n.     
(e) det(a)!= 0.     
(f) The matrix A does not have 0 as an eigenvalue.     

"Equivalent" measn assertin that either all statements true, or all false.     
In order to prove it we need to prove that (a) => (b), (c) => (c), ..., (f) => (a)
(The order of proof might be different).     


*7.3 Existence Proofs; Existence and Uniqueness Proofs*    
Existentially quantified statement:     
E x, R(x).    

A simple example:     
Proposition There exists an even prime number.     
Proof. Observe that 2 is an even prime number.     

Proposition There exists an integer that can be expressed as the sum of two perfect cubes in two different ways.     
Proof. Consider number 1729. Note that 1^3 + 12^3 = 1729 and 9^3 + 10^3 = 1729.     

Sometimes existence statement will be embedded inside of a conditional statement.      

If a, b in N, then there exist integer k and l for which gdc(a, b) = ak + bl.      
This is a conditional statement that has the form:      
a, b in N => E k, l in Z, gdc(a, b) = ak + bl.     
To prove it with direct proof, we'd assume that a, b in N, then prove the existence statement E k, l in Z, gdc(a, b) = ak + bl.     


Proposition 7.1 If a, b in N, then there exist integers k and l for which gcd (a, b ) = ak + bl.     

Proof. (Direct) Suppose a, b in N.      
Consider set A = { ax + by : x, y in Z }. This set contains positive, negative integers and 0 (Let y = 0, then x ranges over all integers. Then ax + by = ax ranges over all multiples of a).     
Let d be the smallest positive element in A. Then d has a form d = ak + bl for some k, l in Z.     
Show that d = gcd(a, b).     
First show that d is a common divisor of a and b and then that it's the greatest common divisor.     
To see that d | a we use the divison algorithm.     
a = qd + r for integers q and r 0 <= r < d.     
r = a - qd.     
r = a - q(ak + bl).     
r = a - qak - qbl.     
r = a(1 - qk) + b(-ql).     
r in A and 0 <= r < d, but d is the smallest element, so r must be zero.     
Then a = qd, which means d | a.     
Same argument for d | b.     
Now prove that d is the greatest common divisor.     
gcd(a, b) divides a and b, a = gcd(a, b) * m, b = gcd(a, b) * n for some m, n in Z.    
So d = ak + bl = gcd(a, b) * mk + gcd(a, b) * nl.     



Uniqueness proofs.     
"There is a uniq *x* for which P(x)".      
Such a statement asserts that there is exactly one example x for which P(x) is true. To prove it, we must produce an example x = d for which P(d) is true, and we must show that d is the only such example.     

7.4 Constructive Versus Non-Constructive Proofs.     
Constructive - explicit example, non-constructive - example exists without actually giving it.     

Example:     

Proposition There exist irrational numbers x, y for which x^y is rational.    
Proof. Let x = sqrt(2)^(sqrt(2)) and y = sqrt(2).     
sqrt(2) is irrational, but it's not clear if sqrt(2)^(sqrt(2)) is rational or irrational.     
If it's irrational, then x^y = (sqrt(2)^(sqrt(2)))^(sqrt(2)) = 2 which is rational.     
If it's rational, then y^y = x.     
(non-constructive proof).     


Proposition There exist irrational numbers x, y for which x^y is rational. 



Exercises for Chapter 7      

1. Suppose x in Z. Then x is even if and only if 3x + 5 is odd.      
Suppose x is even, then x = 2a.     
3x + 5 = 3(2a) + 5 = 6a + 5 = 6a + 4 + 1 = 2(3a + 2) + 1, which is odd.    
Conversely if 3x + 5 is odd, then x is even.     
Suppose x is odd, so x = 2b + 1, then 3(2b + 1) + 5 = 6b + 3 + 5 = 6b + 8 = 2(3b + 4) which is even, not odd.    


3. Given an integer a, then a^3 + a^2 + a is even if and only if a is even.    
a is even, a = 2x, (2x)^3 + (2x)^2 + 2x = 8x^3 + 4x^2 + 2x = 2(4x^3 + 2x^2 + x) which is even.     
Suppose a is odd a = 2y + 1, (2y + 1)^3 + (2y + 1)^2 + 2y + 1 = (4y^2 + 4y + 1)(2y + 1) + 4y^2 + 4y + 1 + 2y + 1 = (4y^2 + 4y + 1)(2y + 1) + 4y^2 + 4y + 1 + 2y + 1 = 8y^3 + 4y^2 + 8y^2 + 4y + 2y + 1 + 4y^2 + 4y + 1 + 2y + 1 = 8y^3 + 16y^2 + 14y + 2 + 1 = 2(4y^3 + 8y^2 + 7y + 1) + 1 which is odd.     


5. An integer a is odd if and only if a^3 is odd.     
Suppose a is odd, a = 2x + 1    
(2x + 1)^3 = (4x^2 + 4x + 1)(2x + 1) = 8x^3 + 8x^2 + 2x + 4x^2 + 4x + 1 = 8x^3 + 12x^2 + 6x + 1 = 2(4x^3 + 6x^2 + 3x) + 1 is odd.     
Suppose a is even, a = 2y, 8y^3 = 2(4y^3) is even.     


7. x, y in R. THen (x + y)^2 = x^2 + y^2 if and only if y = 0, x = 0.      
Suppose (x + y)^2 = x^2 + y^2.      
x^2 + 2xy + y^2 = x^2 + y^2.     
2xy = 0.    
Suppose x = 0 or y = 0.    
Case 1) x = 0. (0 + y)^2 = x^2 + y^2, 0^2 + y^2 = x^2 + y^2.    
Case 2) y = 0. (x + 0)^2 = x^2 + 0^2 = x^2 + y^2.     



8. Suppose a, b in Z. Prove that a === b (mod 10) if and only if a === b (mod 2) and a === b (mod 5).     
1) Prove that a === b (mod 10) if a === b (mod 2) and a === b (mod 5).      
10 | a - b, a - b = 10x.      
a - b = 2(5x).     
Then a === b (mod 2) by definition.        
a - b = 5(2x).     
Then a === b (mod 5) by definition.        
2) Since a === b (mod 2) and a === b (mod 5), a - b = 2y and a - b = 5z.     
a - b is even, so z must be even.       
z = 2m.     
a - b = 5 * 2m = 10m.     
Then a === b (mod 10).      


9. Suppose a in Z. Prove that 14 | a if and only if 7 | a and 2 | a.     
1) 14 | a, then a = 14x.      
a = 7(2x).     
a = 2(7x).     
2) 7 | a, then a = 7y for some y in Z.     
2 | a, then a = 2z for some z in Z.     
Since a = 2z, a is even, then 7y and y must be even.     
y = 2k.     
a = 14k, then 14 | a.     


11. Suppose a, b in Z. Prove that (a - 3)b^2 is even if and only if a is odd or b is even.     
1) a = 2x + 1 or b = 2y.     
(a - 3)4y^2 = 4ay^2 - 14y^2 = 2(2ay^2 - 6y^2) is even.           
(2x + 1 - 3)b^2 = (2x - 2)b^2 = 2xb^2 - 2b^2 = 2(xb^2 - b^2) is even.     
2) a is odd or b is even is the same as a is even and b is odd.      
(2m - 3)(2k + 1)^2 = (2m - 3)(4k^2 + 4k + 1) = 8mk^2 + 8mk + 2m - 12k^2 - 12k - 3 = 2(4mk^2 + 4mk + m - 6k^2 - 6k - 1) - 1 which is odd.     


12. There exists a positive real number x for which x^2 < sqrt(x).     
Suppose x > 0 and x < 1, then x^2 < x.     
Suppose x = m * m then and sqrt(x) = m, so x < m.     
Then it follows that x^2 < x < sqrt(x).     

14. Suppose a in Z. Then a^2 | a if and only if a in {-1, 0, 1}.     



15. Suppose a, b in Z. Prove that a + b is even if adn only if a and b have the same parity.     
1) a + b = 2x.     
Suppose a is even and b is even, then a = 2m, b = 2k.     
2m + 2k = 2(m + k) which is even.     
Suppose a is odd and b is odd, then a = 2m + 1, b = 2k + 1.     
2m + 1 + 2k + 1 = 2(m + k + 1) whichis even.     
2) Suppose it's not the case that a and b have the same parity.     
F.e. a is even, b is odd, then a = 2m, b = 2k + 1.     
2m + 2k + 1 = 2(m + k) + 1 which is odd.     


18. There is a set X for which N in X and N set_in X.     
Observe that there is set X = { {N}, N }.     



19. If n in N, then 2^0 + 2^1 + ... + 2^n = 2^(n + 1) - 1.     
Let S = 2^0 + 2^1 + ... + 2^n, multiply S by 2 (both sides).     
2S = 2^1 + 2^2 + ... + 2^(n + 1).     
Subtract S from 2S, 2S - S = -2^0 + 2^(n + 1).      
So S = 2^(n + 1) - 1.     


20. There exists an n in N for which 11 | (2^n - 1).     
By Fermat theorem, if p !| and p is a prime then a^(p-1) === 1 (mod p).     
2^n === 1 (mod 11).      
2^(11-1) === 1 (mod 11).     
2^10 === 1 (mod 11).     



21. Every real solution of x^3 + x + 3 = 0 is irrational.     
Suppose there are rational solutions (a/b).     
(a/b)^3 + a/b + 3 = 0.     
a^3 + ab^2 + 3b^3 = 0.     
