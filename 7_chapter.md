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
