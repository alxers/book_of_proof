Relations

Definition 11.1 A relation on a set A is a subset R set_in A x A. Abbreviated as (x, y) in R as xRy.     

Example 11.1 Let A = { 1, 2, 3, 4 }.     
R = { (1, 1), (2, 1), (2, 2), (3, 3), (3, 2), (3, 1), (4, 4), (4, 3), (4, 2), (4, 1) } set_in A x A.     
1R1, 2R1, ... etc.     
R is greater-then-or-equal set.     


Exercises for Section 11.1.     
.1. Let A = { 0, 1, 2, 3, 4, 5 }. Write out the relation R that express > on A.     
R = {     
    (1, 0), (2, 0), (3, 0), (4, 0), (5, 0),     
    (2, 1), (3, 1), (4, 1), (5, 1),     
    (3, 2), (4, 2), (5, 2),          
    (4, 3), (5, 3),               
    (5, 4)                    
}      


.2. Let A = { 1, 2, 3, 4, 5, 6 }. Write out the relation R that express | (divides) on A.     
R = {     
    (1, 1), (1, 2), (1, 3), (1, 4), (1, 5), (1, 6),      
    (2, 2), (2, 4), (2, 6),           
    (3, 3), (3, 6),                
    (4, 4),                
    (5, 5),                
    (6, 6)                
}   


.3. Let A = { 0, 1, 2, 3, 4, 5 }. Write out the relation R that express >= on A.     
R = {     
    (0, 0), (1, 0), (2, 0), (3, 0), (4, 0), (5, 0),     
    (1, 1), (2, 1), (3, 1), (4, 1), (5, 1),     
    (2, 2), (3, 2), (4, 2), (5, 2),          
    (4, 4), (4, 3), (5, 3),               
    (5, 5), (5, 4)                    
}      


.4.         
A = { 1, 2, 3, 4, 5 }     
R = {     
    (0, 0), (0, 4), (4, 0),     
    (1, 1), (1, 3), (3, 1), (1, 5), (5, 1),      
    (2, 2), (2, 4), (4, 2),      
    (3, 3),     
    (5, 5)                
}     


.5. 
A = { 0, 1, 2, 3, 4, 5 }      
R = { (1, 2), (2, 5), (3, 3), (4, 3), (4, 2), (5, 0) }



.6. Congruence modulo5 is a relation on the set A = Z. In this relation xRy means x ≡ y(mod5). Write out the set R in set-builder notation.      
R = { (x, y) in Z : 5 | x - y }       



.7. Write the relation < on the set A = Z as a subset R of Z x Z. This is an infinite set, so you will have to use set-builder notation.      
R = { (x, y) in Z x Z : y - x in N } set_in Z x Z.      


.9. Let A = { 1, 2, 3, 4, 5, 6 }. How many different relations are there on the set A ?       
There are 2^|A| = 2^6 subsets of A.      
There are 36 ordered pairs in A.       
So 2^36 many different relations.     

.10. Consider the subset R = (R x R) - { (x,x) : x in R } set_in R x R. What familiar relation onRis this? Explain.        
(R x R) is 2D plane, { (x,x) : x in R } is an equal coordinates.     
Remove all equal coordinates from 2D plane, you get all non-equal coordinates.          


.11. Given a finite set A, how many different relations are there on A ?     
There are 2^|A| subsets of A.      
There are |A| * |A| = |A|^2 ordered pairs in A.       
So 2^(|A|^2) many different relations.     

In the following exercises, R of R^2 = R x R or Z^2 = Z x Z indicated by gray shading. In each case, R is a familiar relation on R or Z. State it.      
.12.     




11.2 Properties of Relations
Definition 11.2 Suppose R is a relation on a set A.     

.1. Relation R is reflexive if xRx for every x in A.     
That is, R is reflexive if all x in A, xRx.     

.2. Relation R is symmetric if xRy implies yRx for all x,y in A.    
That is, R is symmetric if all x, y in A, xRy => yRx.       

.3. Relation R is transitive if whenever xRy and yRz, then also xRz.     
That is, R is transitive if for all x, y, z in A, ((xRy) ^ (yRz)) => xRz.     


Example 11.7. A = { b, c, d, e }, and R is the following relation on A: R { (b, b), (b, c), (c, b), (c, c), (d, d), (b, d), (d, b), (c, d), (d, c) }.      
.1. It's not reflexive, because it's not true that eRe. (should be true for all x in A).      
.2. It's symmetric, whenever we have xRy, it follows yRx too.      
.3. It's transitive.     


Example 11.8 Prove the following proposition.     
Proposition. Let n in N. The relation ≡ (mod n) on the set Z is reflexive, symmetric and transitive.     
1) Show that it's reflexive.     
For all integers in Z it's true that n | 0.     
n | (x - x), which is x ≡ x (mod n) by definition.     
So it's reflexive.     
2) Show that it's symmetric.      
For all x, y in Z it must be true that if x ≡ y (mod n) then y ≡ x (mod n).     
Suppose x ≡ y (mod n). Then n | (x - y).     
Then x - y = na for some a.      
Multiply by (-1) both sides, y - x = n(-a).     
Then n | (y - x), y ≡ x (mod n).     
3) Show that it's transitive.     
Show that if x ≡ y (mod n) and y ≡ z (mod n), then x ≡ z (mod n).      
n | (x - y) and n | (y - z), then x - y = na, y - z = nb.      
x - y + y - z = na + nb.     
x - z = n(a + b).     
n | (x - z).     
x ≡ z (mod n).     



Exercises for Section 11.2     

.1.Consider the relation R = { (a,a), (b,b), (c,c), (d,d), (a,b), (b,a) } on set A = { a, b, c, d }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.       
1) R is reflexive, it's true that for all x in R, xRx.      
2) R is symmetric, for all x, y it's true that xRy => yRx.      
3) ?

.2. Consider the relation R = { (a,b), (a,c), (c,c), (b,b), (c,b), (b,c) } on the set A = { a, b, c }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.     
1) R is not reflexive, it's not true that aRa.     
2) R is not symmetric, it's not true that bRa.     


.3. Consider the relation R = { (a,b), (a,c), (c,b), (b,c) } on the set A = { a, b, c }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is not reflexive, it's not true that xRx for all x in R.      
2) R is not symmetric, it's not true that f.e. aRb => bRa.      
3) R is transitive.     


.4. Let A = { a, b, c, d }. Suppose R is the relation    
R = { (a,a), (b,b), (c,c), (d,d),     
      (a,b), (b,a), (a,c), (c,a),     
      (a,d), (d,a), (b,c), (c,b),     
      (b,d), (d,b), (c,d), (d,c) 
    }.      
Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.     
2) R is symmetric.     
3) R is transitive (?).      


.5. Consider the relation R = { (0, 0), (sqrt(2), 0), (0, sqrt(2)), (sqrt(2), sqrt(2)) } on R. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.     
2) R is symmetric.      
?

.6. Consider the relation R = { (x,x) : x in Z } on Z. Is this R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?      
1) R is reflexive.     
2) R is symmetric.     
3) R is transitive.     
This relation is 2D plain.      (?)

.7. There are 16 possible different relations R on the set A = { a, b }. Describe all ofthem. (A picture for each one will suffice, but don't forget to label the nodes.) Which ones are reflexive? Symmetric? Transitive?     


.8. Define a relation on Z as xRy if |x−y| < 1. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?      
R = { (x, y) in Z x Z : |x - y| < 1 }     
1) R is reflexive, |x - x| < 1 for all x in R.     
???


.9. Define a relation on Z by declaring xRy if and only if x and y have the same parity. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why. What familiar relation is this?     
1) R is reflexive, xRx for all x in R since x have the same parity.     
2) R is symmetric, xRy => yRx, x and y have the same parity.     
3) R is transitive, if xRy and xRz, then xRz.     


.10. Suppose A != empty_set. Since empty_set set_in A x A, the set R = empty_set is a relation on A. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.       
1) R is not reflexive, it's not true that for all x in A, xRx. (?)     
2) R is symmetric.     
3) R is transitive.     


.11. Let A = { a, b, c, d } and R = { (a,a), (b,b), (c,c), (d,d) }. Is R reflexive? Symmetric? Transitive? If a property does not hold, say why.      
1) R is reflexive.      
2) R is symmetric, there are no such x, y for which (y, x) not in R if (x, y) in R.     
3) R is transitive, f.e. (aRa ^ aRa) => aRa.            

.12. Prove that the relation | (divides) on the set Z is reflexive and transitive.     
1) Show that | is reflexive.     
For any integer x in Z, it's true that x | x.      
2) Show that | is transitive.     
We must show that if x | y and y | z then x | z.     
Direct proof. Suppose that x | y and y | z, then y = x * a (for some a in Z) and z = y * b (for some b in Z).     
Then z = x * a * b = x (ab).     
By definition x | z.      

.13. Consider the relation R = { (x, y) in R x R : x - y  in Z } on R. Prove that this relation is reflexive, symmetric and transitive.      
1) Show that R is reflexive.     
For any (x, x) in R it's true that x - x in Z.     
2) Show that R is symmetric.     
If x - y in Z, then -(x - y) in Z, but -(x - y) = y - x.     
Which means xRy => yRx for all x, y in R.      
3) Show that R is transitive.     
Show that if x - y in Z and y - z in Z, then x - z in Z.     
Suppose x - y in Z and y - z in Z, then      
x - y = a, y - z = b for some a, b in Z,     
x - b - z = a, x - z = a + b, a + b in Z.     

.14. Suppose R is a symmetric and transitive relation on a set A, and there is an element a in A for which aRx for every x in A. Prove that R is reflexive.      
Since R is symmetric it follows that aRx => xRa.     
R is also transitive, so aRx ^ xRa => aRa.    

.15. Prove or disprove: If a relation is symmetric and transitive, then it is also reflexive.     
It's false (see Example 11.7, page 180).    
Disprove by counterexample.     
Consider A = { b, c, d }, and R is the following relation on A:     
R = { (b, b), (b, c), (c, b), (c, c), (b, d), (d, b), (c, d), (d, c) }      
R is symmetric, whenever we have xRy, it follows that yRx.     
R is transitive, but not reflexive, it's not true that dRd.      

.16. Define a relation R on Z by declaring that xRy if and only if x^2 === y^2(mod 4). Prove that R is reflexive, symmetric and transitive.     
R = { (x, y) in Z x Z : 4 | x^2 - y^2 }.     
Prove that R is reflexive.     
Observe that 4 | 0, so 4 | (x^2 - x^2) => x^2 === x^2 (mod 4).     
Prove that R is symmetric.     
Suppose x^2 === y^2 (mod 4), then by definition 4 | x^2 - y^2, then x^2 - y^2 = 4a, for some a in Z.     
Multiply by -1 we get y^2 - x^2 = 4(-a).     
Then 4 | y^2 - x^2 => y^2 === x^2 (mod 4).     
Prove that R is transitive.     
Suppose that 4 | x^2 - y^2 and 4 | y^2 - z^2.     
x^2 - y^2 = 4a, y^2 - z^2 = 4b.     
Add those two together we get x^2 - y^2 + y^2 - z^2 = 4a + 4b.     
x^2 - z^2 = 4(ab) => 4 | x^2 - z^2 => x^2 === z^2 (mod 4).     


.17. Modifying the above Exercise 8 (above) slightly, define a relation ~ on Z as x ∼ y if and only if |x-y|<=1. Say whether ∼ is reflexive. Is it symmetric? Transitive?
1) R is reflexive, |x - x| < 1 for all x in R.     
???


11.3 Equivalence Relations.     

Definition 11.3 A relation R is called equivalence relation on a set A if it's reflexive, symmetric and transitive.     


Definition 11.4 Suppose R is an equivalence relation on a set A. Given any element a, an equivalence class containing a is a subset of A [a] = { x in A : xRa }.     


R_1 = { (-1, -1), (1, 1), (2, 2), (3, 3), (4, 4) }

Example 11.9 Consider relation R_1 (equal to, "="), the equivalence class containing 2 is [2] = { x in A : x(R_1)2 } = { 2 }.     


Exercises for Section 11.3.      

.1. Let A = { 1, 2, 3, 4, 5, 6 }, and consider the following equivalence relation on A: R = { (1, 1), (2, 2), (3, 3), (4, 4), (5, 5), (6, 6), (2, 3), (3, 2), (4, 5), (5, 4), (4, 6), (6, 4), (5, 6), (6, 5) }. List the equivalence classes of R.     
[1] = { x in A : xR1 } = { 1 }     
[2] = { x in A : xR2 } = { 2, 3 }     
[3] = { x in A : xR3 } = { 3, 2 }     
[4] = { x in A : xR4 } = { 4, 5, 6 }     
[5] = { x in A : xR5 } = { 5, 4, 6 }     
[6] = { x in A : xR6 } = { 6, 4, 5 }     
{ 1 }, { 2, 3 }, { 4, 5, 6 }     
There are 3 equivalence classes.     


.2. Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose R has two equivalence classes. Also aRd, bRc and eRd. Write out R as a set.     
If aRd,bRc and eRd, then R contains (a, d), (b, c), (e, d).     
R is symmetric, so R contains (d, a), (c, b), (d, e).     
R is reflexive, R contains (a, a), (b, b), (c, c), (d, d), (e, e).     
aRd and eRd means there should be (a, e), (e, a)
R has two equivalence classes, they are:     
[a] = { a, d, e }.     
[b] = { c, b }.     
[c] = { b, c }.     
[d] = { a, d, e }.     
[e] = { d, e, a }.     
[a] = [d] = [e], [b] = [c].         
R = { (a, d), (b, c), (e, d), (d, a), (c, b), (d, e), (a, a), (b, b), (c, c), (d, d), (e, e), (a, e), (e, a) }
Solution_2.      
aRd and eRd means that a, e, d in the same equivalence class.     
bRc means b, c in the same equivalence class.     
There are two equivalence classes - { a, e, d }, { b, c }.          
For R to be an equivalence relation, it needs to include all possible pairs of elements in the same equivalence class and no others (!!!).     


.3. Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose R has three equivalence classes. Also aRd and bRc. Write out R as a set.      
If aRd, bRc, then R contains (a, d), (b, c).     
R is symmetric, R contains (d, a), (c, b).     
R is reflexive, R contains (a, a), (b, b), (c, c), (d, d), (e, e).     
R has three equivalence classes:
[a] = { d, a }.      
[b] = { c, b }.     
[c] = { b, c }.     
[d] = { c, b }.     
[e] = { e }.     
[a] = [d], [b] = [c], [e] - three classes.     
R = { (a, d), (b, c), (d, a), (c, b), (a, a), (b, b), (c, c), (d, d), (e, e) }     

.4.Let A = { a, b, c, d, e }. Suppose R is an equivalence relation on A. Suppose also that aRd and bRc, eRa and cRe. How many equivalence classes does R have?      
aRd => a, and d in the same equivalence class, [a] = [d]     
bRc => [b] = [c]     
eRa => [e] = [a]     
cRe => [c] = [e]     
[a] = [d] = [e] = [c] = [b].     
There is one equivalence class.     

.5. There are two different equivalence relations on the set A = { a, b }. Describe them. Diagrams will suffice.     
There should be two equivalence relations, R_1, R_2.     
Since they are equivalence relations, they should be reflexive, symmetric and transitive.     
R_1 = { (a, a), (b, b) }     
R_2 = { (a, a), (b, b), (a, b), (b, a) }     


.6. There are five different equivalence relations on the set A = { a, b, c }. Describe them all. Diagrams will suffice.     
R_1 = { (a, a), (b, b), (c, c) }.     
R_2 = { (a, a), (b, b), (c, c), (a, b), (b, a) }.     
R_3 = { (a, a), (b, b), (c, c), (a, c), (c, a) }.     
R_4 = { (a, a), (b, b), (c, c), (b, c), (c, b) }.     
R_5 = { (a, a), (b, b), (c, c), (a, b), (b, a), (a, c), (c, a), (b, c), (c, b) }.     


.7. Define a relation R on Z as xRy if and only if 3x-5y is even. Prove R is an equivalence relation. Describe its equivalence classes.      
1) Proof that R is reflexive.      
3x-5x = -2x - even.     
2) Proof that R is symmetric.     
3x - 5y = 2a.      
3x - 5y + 8y - 8x = 2a + 8y - 8x.     
3y - 5x = 2(a + 4y - 4x).      
3) Proof that R is transitive.       
3x - 5y = 2a, 3y - 5z = 2b.       
3x - 5y + 3y - 5z = 2a - 2b.      
3x - 2y - 5z = 2a - 2b.      
3x - 5z = 2(a - b + y).      
[0] = { x in Z : xR0 } = { 3x - 5 * 0 = 3x, 3x is even } = { x in Z : x is even }.     
[1] = { x in Z : xR1 } = { 3x - 5, 3x = 5, 3x is odd } = { x in Z : x is odd }.     



.8. Define a relation R on Z as xRy if and only if x^2 + y^2 is even. Prove R is an equivalence relation. Describe its equivalence classes.      
1) Reflexive x^2 + x^2 = 2x^2 - even.     
2) Symmetric x^2 + y^2, y^2 + x^2.      
3) Transitive x^2 + y^2 = 2a, y^2 + z^2 = 2b.      
x^2 + y^2 + y^2 + z^2 = 2a + 2b.      
x^2 + z^2 = 2(a + b - y^2).       
Equivalence classes.      
[0] = { x in Z : xR0 } = { x^2 + 0 = x^2 is even } = { x in Z : x even }.       
[1] = { x in Z : xR1 } = { x^2 + 1 is even } = { x in Z : x odd }.       


.9. Define a relation R on Z as xRy if and only if 4|(x + 3y). Prove R is an equivalence relation. Describe its equivalence classes.      
1) Reflexive 4 | (x + 3x), 4 | 4x.      
2) Symmetric 4 | (x + 3y), 4 | (y + 3x).      
x + 3y = 4a.      
3x + 9y = 12a.       
y + 8y + 3x = 12a.     
y + 3x = 12a - 8y.     
y + 3x = 4(3 - 2y).      
3) Transitive.      
x + 3y = 4a, y + 3z = 4b.      
x + 3y + y + 3z = 4a + 4b.      
x + 3z = 4(a + b - y).     
Equivalence classes.      
[0] = { x in Z : xR0 } = { 4 | x, x = 4a } = { ..., -4, 0, 4, 8, 12, 16, ... }     
[1] = { x in Z : xR1 } = { 4 | (x + 3 * 1) } = { ..., -3, 1, 5, 9, ... }     
[2] = { x in Z : xR2 } = { 4 | (x + 3 * 2) } = { ..., -6, -2, 2, 6, ... }     
[3] = { x in Z : xR3 } = { 4 | (x + 3 * 3) } = { ..., -1, 3, 7, ... }     


.10. Suppose R and S are two equivalence relations on a set A. Prove that R intersection S is also an equivalence relation. (For an example of this, look at Figure 11.2. Observe that for the equivalence relations R_2, R_3 and R_4, we have R_2 intersection R_3 = R_4.).     
1) Reflexive.      
Let x in A, since R, S equivalence relation on A, (x, x) in R, (x, x) in S => (x, x) in R intersection S.      
2) Symmetric.      
Let (x, y) in R intersect S, then (x, y) in R, S, since R, S are symmetric, then (y, x) in R, S, then (y, x) in R intersect S.     
3) Transitive.     
Let (x, y) in R intersect S and (y, z) in R intersect S. Then (x, y) in R, S and (y, z) in R, S. Since R and S are transitive, then (x, z) in R, S. Then (x, z) in R intersect S.      


.11. Prove or disprove: If R is an equivalence relation on an infinite set A, then R has infinitely many equivalence classes.      
False.       
Counterexample, see example 11.12 (=== mod(3)).       


.12. Prove or disprove: If R and S are two equivalence relations on a set A, then R union S is also an equivalence relation on A.       
False.       
Counterexample, figure 11.2, R_2 union R_3 = { (-1, -1), (1, 1), (2, 2), (3, 3), (4, 4), (-1, 1), (1, -1), (-1, 3), (3, -1), (1, 3), (3, 1), (2, 4), (4, 2), (1, 2), (2, 1), (2, 1), (1, 4), (4, 1), (3, 4), (4, 3), (2, 3), (3, 2) }.         
This relation is reflexive, symmetric but not transitive.       
(-1, 3) ^ (3, 4) => (-1, 4), there is no (-1, 4) in R_2 union R_3.     

.14. Suppose Ris a reflexive and symmetric relation on a finite set A. Define a relation S on A by declaring xSy if and only if for some n in N there are elements x1,x2,...,x_n in A satisfying xRx1, x1Rx2,x2Rx3,x3Rx4,...,x_(n-1)Rx_n, and x_nRy. Show that S is an equivalence relation and R set_in S. Prove that S is the unique smallest equivalence relation on A containing R.      
xRx1, x1Rx2 => xRx_n - transitive.      
Since R is symmetric => x1Rx, x2Rx1, ..., x_nRx(n-1) in S.      
R is reflexive => xRx in S.      
S is reflexive, symmetric, transitive, R set_in S.       


Definition 11.5 A partition of a set A is a set of non-empty subsets of A, such that the union of all the subsets equals A, and the intersection of any two different subsets is an empty_set.     


Exercises for Section 11.3 (11.4 in the 3rd edition)       

.1. List all partitions of set A = { a, b }.       
{ { a }, { b } }, { { a, b } }.      


.2. List all partitions of set A = { a, b, c }.      
{ { a }, { b }, { c } }, { { a, b }, { c } }, { { a }, { b, c } },      
{ { a, b, c } }, { { a, c }, { b } }.       


.3. Describe the partition of Z resulting from the equivalence relation === (mod 4).     
[0] = { x in Z : x === 0 (mod 4) } = { 4 | (x - 0) } = { ..., -4, 0, 4, 8, ... }     
[1] = { x in Z : x === 1 (mod 4) } = { 4 | (x - 1) } = { ..., -3, 1, 5, 9, ... }     
[2] = { x in Z : x === 2 (mod 4) } = { 4 | (x - 2) } = { ..., -2, 2, 6, 10, ... }     
[3] = { x in Z : x === 3 (mod 4) } = { 4 | (x - 3) } = { ..., -1, 3, 7, 11, ... }     


.5. Consider the partition P = { { ...,-4 , -2, 0, 2, 4, ... }, { ..., -5, -3, -1, 1, 3, 5, ... } } of Z. Let R be the equivalence relation whose equivalence classes are the two elements of P. What familiar equivalence relation is R?       
x === y (mod 2).     


.6. Consider the partition P = { { 0 }, { -1, 1 }, { -2, 2 }, { -3, 3 }, { -4, 4 }, ... } of Z. Describethe equivalence relation whose equivalence classes are the elements of P.     
x = -y (???).     


Exercises for Section 11.4 (11.5 in the 3rd edition)       

.1. Write the addition and multiplication tables for Z_2.     
.+   [0]  [1]      
[0]  [0]  [1]     
[1]  [1]  [0]     

.*   [0]  [1]      
[0]  [0]  [0]     
[1]  [0]  [1]     


.2. Write the addition and multiplication tables for Z_3.     
.+   [0]  [1]  [2]      
[0]  [0]  [1]  [2]     
[1]  [1]  [2]  [0]     
[2]  [2]  [0]  [1]     

.*   [0]  [1]  [2]      
[0]  [0]  [0]  [0]     
[1]  [0]  [1]  [2]     
[2]  [0]  [2]  [1]     


.5. Suppose [a], [b] in Z_5 and [a] * [b] = [0]. Is it necessarily true that either [a] = [0] or [b] = [0] ?     
All multiples of 5, f.e, [5], [10], [15], etc. are equal to [0].     
There is no way to make a number by multiplying any digit from 1 to 4 and get multiple of 5.     
So either [a] or [b] has to be equal to [0].      

.6. Suppose [a], [b] in Z_6 and [a] * [b] = [0]. Is it necessarily true that either [a] = [0] or [b] = [0] ?    
No, f.e. [a] = [2], b = [3].     
[2] * [3] = [2 * 3] = [6] = [0].     



.7. Do the following calculations in Z_9, in each case expressing your answer as[a]with 0 <= a <= 8.     
(a) [8] + [8] = [16] = [7].     
(b) [24] + [11] = [35] = [8].     
(c) [21] * [15] = [315], 315 = 35 * 9 => [315] = [0]  (every number multiplied by 9 in Z_9 will give [0]).     
(d) [8] * [8] = [64], 7 * 9 = 63, => [64] = [1].      



.8. Suppose [a],[b] in Z_n, and [a] = [a'] and [b] = [b']. Alice adds [a] and [b] as [a] + [b] = [a + b]. Bob adds them as [a'] + [b'] = [a' + b']. Show that their answers [a + b] and [a' + b'] are the same.     
Since [a] = [a'], by Theorem 11.1, a === a' (mod n), so n | (a - a') => a - a' = nk, b - b' = nl.     
Therefore a + b = (a' + nk) + (b' + nl) = a' + b' + n(k + l).     
(a + b) - (a' + b') = n(k + l).     
n | ((a + b) - (a' + b')).      
a + b = a' + b' (mod n) => [a + b] = [a' + b'].      
