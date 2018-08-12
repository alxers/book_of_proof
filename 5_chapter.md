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
