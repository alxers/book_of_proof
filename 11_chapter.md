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

.3. Relation R is transitive if whenever xRy and yRz, then also xRz.     
That is, R is transitive if for all x, y, z in A, ((xRy) ^ (yRz)) => xRz.     


Example 11.7. A = { b, c, d, e }, and R is the following relation on A: R { (b, b), (b, c), (c, b), (c, c), (d, d), (b, d), (d, b), (c, d), (d, c) }.      

