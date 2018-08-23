CHAPTER 5     

Contrapositive Proof     

Since P => Q is equivalent to ~Q => ~P the latter expression is called the contrapositive (logically equivalent) form of P => Q.    

Outline for Contrapositive Proof.    
Proposition If P, then Q.    
Proof. Suppose ~Q.    
...    
Then ~P.    


Proposition.    
Suppose x in Z. If 7x+9 is even, then x is odd.    
Suppose x is even.    
Then x = 2a.    
7(2a) + 9 = 14a + 9 = 14a + 8 + 1 = 2(7a + 4) + 1.    
7x + 9 = 2b + 1, where b = 7a + 4.     
Thus 7x + 9 is odd.     
If x is not odd and 7x + 9 is not even, then if x is odd then 7x + 9 is even.    



Suppose x in Z. If x^2 - 6x + 5 is even, then x is odd.    
Suppose x is even.    
Then x = 2a.    
4a^2 - 12a + 5 = 4a^2 - 12a + 4 + 1 = 2(2a^2 - 6a + 2) + 1.    
Thus x^2 - 6x + 5 is odd.    
If x is not odd, x^2 - 6x + 5 is not even, so if x is odd, then x^2 - 6x + 5 is even.



Suppose x, y in R. If y^3 + yx^2 <= x^3 xy^2, then y <= x    
Suppose y > x    
y^3 - xy^2 + yx^2 - x^3 <= 0    
y^3(y - x) + x^2(y - x) <= 0    
If y > 0, then y - x > 0    
Divide both sides by (y - x)    
Then y^2 + x^2 <= 0, which is false    

(Book proof)
Suppose y > x     
Then y - x > 0     
Multiply both sides by the positive x^2 + y^2    
(y - x)(x^2 + y^2) > 0(x^2 + y^2)      
yx^2 + y^3 - x^3 - xy^2 > 0      
y^3 + yx^2 > x^3 + xy^2    
Therefore y^3 + yx^2 > x^3 + xy^2, so it's not true that y^3 + yx^2 <= x^3 xy^2.     



Suppose x, y in Z. If 5 !| xy (5 does not divide xy), then 5 !| x and 5 !| y.    
Suppose 5 | x and 5 | y.    
Then x = 5a, y = 5b.    
xy = 5a5b = 5(5ab).    
xy = 5c, where c = 5ab => 5 | xy.    

(Book of proof)    
By DeMorgan’s law, it is not true that 5 !| x or it is not true that 5 !| y.    
Therefore 5 | x or 5 | y. We consider these possibilities separately.    
Case 1. Suppose 5 | x . Then x = 5a for some a in Z.    
From this we get xy = 5(ay), and that means 5 | xy.     
Case 2. Suppose 5 | y. Then y = 5a for some a in Z.    
From this we get x y = 5(ax), and that means 5 | xy.    
The above cases show that 5 | xy, so it is not true that 5 - xy.    



*Definition 5.1* Given integers a and b and an n ∈ N , we say that a and b
are *congruent modulo* n if n | (a - b). We express this as a ≡ b (mod n).
If a and b are not congruent modulo n , we write this as a 6 ≡ b (mod n).    
(сравнимо по модулю)

Example 5.1    
Here are some examples:    
1. 9 ≡ 1 (mod 4 ) because 4 | (9 − 1).    
2. 6 ≡ 10 (mod 4 ) because 4 | (6 − 10).    
3. 14 !≡ 8 (mod 4 ) because 4 !| (14 − 8).    


In practical terms, a ≡ b (mod n ) means that a and b have the same
remainder when divided by n.    



Proposition. Let a, b in Z and n in N. If a congruent modulo b (mod n), then a^2 congurent modulo b^2 (mod n).      
By definition congurent modulo n | (a - b).     
Then n | (a^2 - b^2).    
a^2 - b^2 = (a - b)(a + b).    
n | (a - b) x, where x = (a + b).     


Proposition. Let a, b in Z and n in N. If a congruent modulo b (mod n), then ac congurent modulo bc (mod n).     
By definition n | (a - b).     
Then n | (ac - bc).    
n | c(a - b).          



Proposition. Suppose a, b in Z and n in N. If 12a !≡ 12b (mod n), then n !| 12.     
Suppose 12a ≡ 12b (mod n).    
Then n | (12a - 12b).    
n | 12(a - b).    
Which means n | 12.    



Exerceses for Chapter 5.     


1. Suppose n in Z. If n^2 is even, then n is even.    
Suppose n is odd.    
Then n = 2a + 1.    
Then n^2 = (2a + 1)^2 = 4a^2 + 4a + 1 = 2(2a^2 + 2a) + 1 which is odd.    
So it must be that n is even.    


2. Suppose n in Z. If n^2 is odd, then n is odd.    
Suppose n is even.    
Then n = 2a.    
Then n^2 = 4a^2 = 2(2a^2) which is even.    
So it must be that n is odd.     


3. Suppose a, b in Z. If a^2(b^2 - 2b) is odd, then a and b are odd.    
Suppose a and b are even.    
Then a = 2m, b = 2n.    
Then 4m^2(4n^2 - 4n) = 16(mn)^2 - 16(m^2)n = 2(8(mn)^2 - 8(m^2)n) which is even.    
So it must be that a and b are odd.     


4. Suppose a, b, c in Z. If a does not divide bc, then a does not divide b.     
Suppose a | b.    
Then b = ax.     
Then b/x = a.    
Which means a | bc where c = 1/x.    


5. Suppose x in R. If x^2 + 5x < 0, then x < 0.
Suppose x >= 0.    
Then x^2 and 5x are not negative.     
So x^2 + 5x >= 0.     



6. Suppose x in R. If x^3 - x > 0, then x > 0.    
Suppose x <= 0.    
Then x(x^2 - 1) <= 0.    
So it's not true that when x <= 0, x^3 - x > 0.    

7. Suppose a, b in Z. If both ab and a + b are even, then both a and b are even.     
Case 1.    
Suppose a is odd.    
Then a = 2n + 1, b = 2m.    
ab = (2n + 1)2m = 4mn + 2m = 2(2mn + m).    
ab = 2k, where k = 2mn + m.     
ab is even.    
Case 2.    
Suppose b is odd.    
Then b = 2n + 1, a = 2m.    
ab = 2k, where k = 2mn + m.    
ab is even.    
Case 3.
Suppose a and b is odd.    
Then a = 2m + 1, b = 2n + 1.    
ab = (2m + 1)(2n + 1) = 4mn + 2m + 2n + 1 = 2(2mn + m + n) + 1.    
ab = 2k + 1.    
ab is odd.     



8. Suppose x in R. If x^5 - 4x^4 + 3x^3 - x^2 + 3x - 4 >= 0, then x >= 0.    
Suppose x < 0.    
Then x^4(x - 4) + x^2(3x - 1) + 3x - 4 < 0.    
So it's not the case that x^5 - 4x^4 + 3x^3 - x^2 + 3x - 4 >= 0 when x < 0.    
Then it must be that x^5 - 4x^4 + 3x^3 - x^2 + 3x - 4 >= 0 then x >= 0.    



9. Suppose n in Z. If 3 !| n^2, then 3 !| n.    
Suppose 3 | n.    
Then n = 3a.    
n^2 = 9a^2 = 3(3a^2).    
So 3 | n^2.     




10. Suppose x, y, z in Z and x != 0. If x !| yz, then x !| y and x !| z.     
Case 1.    
Suppose x | y.    
Then y = xa for some a in Z.    
yz = xb, dividing by z, y = x(b/z).     
When x | y it follows that x | yz.    
Case 2.    
Suppose x | z.    
Then z = xc for some c in Z.    
yz = xc, dividing by z, y = x(c/z).    
When x | z it follows that x | yz.    
