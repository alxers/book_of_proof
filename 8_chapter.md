# Chapter 8     


Proof Involving Sets      


How to show a in { x : P(x) }     
Show that P(a) is true.     


How to show a in { x in S : P(x) }      
1. Verify that a in S.     
2. Show that P(a) is true.     


How to Prove A set_in B      
(Direct approach)      

Proof. Suppose a in A.     
...     
Therefore a in B.      
Thus a in A implies a in B,     
so it follows that A set_in B.     



How to Prove A set_in B      
(Contrapositive)     

Proof. Suppose a not in B.     
...     
Therefore a in A.     
Thus a not in B implies a not in A,     
so it follows that A set_in B.     



How to Prove A = B.     

Proof.     
[Prove that A set_in B.]     
[Prove that B set_in A.]     
Therefore, since A set_in B and B set_in A,      
it follows that A = B.      


Ex.    

1. Prove that { 12n : n in Z } set_in { 2n : n in Z } intersection { 3n : n in Z }.     
By definition of intersection x in { 2n : n in Z } AND x in { 3n : n in Z }.    
So x = (2 * 3)n = 6n.      
Suppose x in { 12n : n in Z }, then x = 12n = 6(2n).     
Since x in { 12n : n in Z } and x in ({ 2n : n in Z } intersection { 3n : n in Z }), then, by definition of set_in, { 12n : n in Z } set_in { 2n : n in Z } intersection { 3n : n in Z }.      


3. If k in Z, then { n in Z: n | k } set_in { n in Z : n | k^2 }


4. If m, n in Z, then { x in Z : mn | x } set_in { x in Z : m | x } intersection { x in Z : n | x }.     
1) Show that { x in Z : mn | x } set_in { x in Z : m | x }       
x = ma by definition of mn | x    
x = m(na)      
Also x = mb by definition of m | x, so x = mb where b = na.     
x in A and x in B.     
2) Show that { x in Z : m | x } intersection { x in Z : n | x }.     
x in { x in Z : m | x } and x in { x in Z : n | x }      


5. If p and q are positive integers, then { pn : n in N } intersection { qn : n in N } != empty_set.     


6. A set_in B then A - C set_in B - C.      
1) Suppose A set_in B, then by definition of set_in a in A and a in B.      
Also a not in C.      
Then a in (A - C) and a in (B - C), which means A - C set_in B - C.     


7. If B set_in C then A x B set_in A x C.      
Direct proof.     
Suppose A x B, then a in A and b in B.     
Since B set_in C, then b in B and b in C.     
Then if b in B and b in C, then (a, b) in A x C.     
Then (a, b) in A x B and (a, b) in A x C, so A x B set_in A x C      


14. (A union B) - C = (A - C) union (B - C).     
{ x: (x in A or x in B) and (x not_in C) } =     
= { x: (x in A and x not_in C) or (x in B and x not_in C) }
