Disproof

How to disprove P: Prove ~P.     


How to disprove All x in S, P(x).      
Produce an example of an x in S that makes P(x) false.     


How to disprove P(x) => Q(x).      
Produce an example of an x that makes P(x) true and Q(x) false.      


How to disprove P with contradiction:      
Assume P is true, and deduce a contradiction.      



Exercises for Chapter 9      


1. If x, y in R, then |x + y| = |x| + |y|.     
Counterexample: x = 2, y = -5;      
|2-5| = 3; |2| + |-5| = 7;      



2. For every natural number n, the integer 2n^2 - 4n + 31 is prime.      
2n^2 - 4n + 31 = n(2n - 4) + 31.      
For n = 31; 31(2n - 4) + 31 = 31((2n - 4) + 1) which is not prime.      



3. If n in Z and n^5 - n is even, then n is even.     
Counterexample. 3^5 - 3 = 240, 3 is not even.     


4. For every natural number n, the integer n^2 + 17n + 17 is prime.     
Counterexample. n = 17, then 17 | n^2, 17 | 17n, 17 | 17.      


5. (A x B) union (C x D) = (A union C) x (B union D).     
Let A = { 1, 2 }, B = { 2, 3 }, C = { 2, 4}, D = { 3, 5 }.      
A x B = { (1, 2), (1, 3), (2, 2), (2, 3) }.     
C x D = { (2, 3), (2, 5), (4, 3), (4, 5) }.      
(A x B) union (C x D) = { (1, 2), (1, 3), (2, 2), (2, 3), (2, 5), (4, 3), (4, 5) }.     
A union C = { 1, 2, 4 }.     
B union D = { 2, 3, 5 }.      
(A union C) x (B union D) = { (1, 2), (1, 3), (1, 5), (2, 2), (2, 3), (2, 5), (4, 2), (4, 3), (4, 5) }.     
It's clear that (A x B) union (C x D) != (A union C) x (B union D).     


7. If A, B and C are sets and A x C = B x C, then A = B.     
Counterexample.     
Let A = { 1 }, B = { 2 }, C = { 3 }.     
Then A x C = { (1, 3) }.     
B x C = { (2, 3) }.     



8. A - (B union C) = (A - B) union (A - C).     
Counterexample.      
A = { 1, 2 }, B = { 2, 3 }, C = { 2, 4 }.    
B union C = { 2 }.     
A - (B union C) = { 1 }.     
A - B = { 1 }.     
A - C = { 4 }.     
(A - B) union (A - C) = empty_set.    



9. Power_set(A) - Power_set(B) set_in Power_set(A - B).     
Counterexample.     
A = { 1, 2 }, B = { 2, 3 }.     
Power_set(A) = { { empty_set }, { 1 }, { 2 }, { 1, 2 } }.    
Poser_set(B) = { { empty_set }, { 2 }, { 3 }, { 2, 3 } }.     
Power_set(A) - Power_set(B) = { { 1 }, { 1, 2 } }.    
A - B = { 1 }.    
Power_set(A - B) = { { empty_set }, { 1 } }.     



10. If A and B are sets and A intersection B = empty_set, then Power_set(A) - Power_set(B) set_in Power_set(A - B).     
False.     
Counterexample.     
Let A = { 1, 2 }, B = { 3, 4 }.     
Power_set(A) = { { empty_set }, { 1 }, { 2 }, { 1, 2 } }, Power_set(B) = { { empty_set }, { 3 }, { 4 }, { 3, 4 } }.     
Power_set(A) - Power_set(B) = { { 1 }, { 2 }, { 1, 2 } }, Power_set(A - B) = Power_set({ 1, 2 }) = { { empty_set }, { 1 }, { 2 }, { 1, 2 } }.    



11. If a, b in N, then a + b < ab.     
False.     
Counterexample.     
Let a = 1, b = 2.     
Then 1 + 2 = 3, 1 * 2 = 2.     



12. If a, b, c in N and ab, bc, ac have the same parity, then a, b, c have the same parity.     
Case 1.      
Suppose a, b and c are even, then a = 2x, b = 2y, c = 2z.     
Then ab = 4xy, ac = 4xz, bc = 4yz, which are even.     
Case 2.      
Suppose a, b and c are odd, then a = 2x + 1, b = 2y + 1, c = 2z + 1.     
ab = (2x + 1)(2y + 1) = 4xy + 2x + 2y + 1, same for bc and ac, they're odd.     



13. There exists set X for which R set_in X and empty_set in X.     
True.     
Let X = R union empty_set.      



14. If A and B are sets, then Power_set(A) intersection Powers_set(B) = Power_set(A intersection B).      



15. Every odd integer is the sum of three odd integers.     
True.     
n = n + 1 + (-1).      



16. If a and B are finite sets then |A union B| = |A| + |B|.      
False.     
Counterexample.      
Let A = { 1, 2 }, B = { 2, 3 }.      
A union B = { 1, 2, 3 }, |A union B| = 3.      
|A| = 2, |B| = 2.     



17. For all sets A and B, if A - B = empty_set, then B != empty_set.      
False.      
Counterexample.      
Let A = empty_set, B = empty_set.      
A - B = empty_set.      



18. If a, b, c in N, then at least one of a - b, a + c and b - c is even.      



20. There exist prime numbers p and q for which p - q = 1000.     
True.     
p - q = 1000.     
p = 1000 + q;
p = 1013, q = 13.      


21. There exist prime numbers p and q for which p - q = 97.      
False.     
By contradiction. Suppose p - q = 97, then p and q must have opposite parity.     
Suppose q is even, p is odd, the only even prime is 2.     
p - 2 = 97, p = 99.     
99 is not odd.     
Contradiction.     



22. If p and q are prime numbers for which p < q, then 2p + q^2 is odd.     
True.     
2p is always even by definition of an even number, q > 2, so it's an odd number.    
Sum of odd and even always odd.     
2x + 2y + 1 = 2(x + y) + 1.     



23. If x, y in R and x^3 < y^3, then x < y.     
True.     
x^3 < y^3.      
x^3 - y^3 < 0.     
(x - y)(x^2 + xy + y^2) < 0.     
x^2 + xy + y^2 > 0, since x^2 + y^2 always > 0, and x^2 + y^2 > xy.     
Divide (x - y)(x^2 + xy + y^2) by (x^2 + xy + y^2).     
x - y < 0.     
x < y.     



24. The inequality 2^x >= x + 1 is true for all positive real numbers x.     
False.      
Let x = 1/2, then 2^(1/2) ~=  1.41, 1/2 + 1 = 1.5.     



25. For all a, b, c in Z, if a | bc, then a | b or a | c.     
False.     
Let a = 10, b = 2, c = 5.     
10 | 10 but 10 !| 2 and 10 !| 5.     



26. Suppose A, B and C are sets. If A = B - C, then B = A union C.     
False.     
Suppose B = empty_set, C = { 3 }.      
A = B - C = empty_set - { 3 } = empty_set.     
B = A union C = empty_set union { 3 } = { 3 }.     



28. Suppose a, b in Z. If a | b and b | a, then a = b.     
False.     
Let a = 2, b = -2, 2 | -2 and  -2 | 2, but a != b.     
Another proof.     
b = ax, a = by.     
a = axy.     
1 = xy.     
So x = y = 1 or x = y = -1.     
In fact a = +-b


29. If x, y in R and |x+y|=|x−y|, then y=0.  
False.     
Let x = 0, y = 1, then |0 + 1| = |0 - 1|.     
1 = 1.    



30. There exist integers a and b for which 42a + 7b = 1.     
False.     
42a + 7b = 7(6a + b) = 1.     
6a + b = 1/7.     
There are no such integers.     
