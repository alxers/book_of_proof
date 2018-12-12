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
Conterexample: x = 2, y = -5;      
|2-5| = 3; |2| + |-5| = 7;      



2. For every natural number n, the integer 2n^2 - 4n + 31 is prime.      
2n^2 - 4n + 31 = n(2n - 4) + 31.      
For n = 31; 31(2n - 4) + 31 = 31((2n - 4) + 1) which is not prime.      



3. If n in Z and n^5 - n is even, then n is even.     
Conterexample. 3^5 - 3 = 240, 3 is not even.     


4. For every natural number n, the integer n^2 + 17n + 17 is prime.     
Conterexample. n = 17, then 17 | n^2, 17 | 17n, 17 | 17.      


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
Conterexample.     
Let A = { 1 }, B = { 2 }, C = { 3 }.     
Then A x C = { (1, 3) }.     
B x C = { (2, 3) }.     



8. A - (B union C) = (A - B) union (A - C).     
Conterexample.      
A = { 1, 2 }, B = { 2, 3 }, C = { 2, 4 }.    
B union C = { 2 }.     
A - (B union C) = { 1 }.     
A - B = { 1 }.     
A - C = { 4 }.     
(A - B) union (A - C) = empty_set.    



9. Power_set(A) - Power_set(B) set_in Power_set(A - B).     
Conterexample.     
A = { 1, 2 }, B = { 2, 3 }.     
Power_set(A) = { { empty_set }, { 1 }, { 2 }, { 1, 2 } }.    
Poser_set(B) = { { empty_set }, { 2 }, { 3 }, { 2, 3 } }.     
Power_set(A) - Power_set(B) = { { 1 }, { 1, 2 } }.    
A - B = { 1 }.    
Power_set(A - B) = { { empty_set }, { 1 } }.     



10. If A and B are sets and A intersection B = empty_set, then Power_set(A) - Power_set(B) set_in Power_set(A - B).     
