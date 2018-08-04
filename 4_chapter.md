Part II
Chapter 4

Definition 4.3 Two integers have the same parity if they are both even or they are both odd. Otherwise they have opposite parity

Definition 4.4 Suppose a and b are integers. We say that a divides b, written a | b, if b = ac for some c in Z. In this case we also say that a is a divisor of b, and that b is a multiple of a.

4.3 Direct Proof
(proposition is a statement that, although true, is not as significant as a theorem.)

Suppose we have:
Proposition If P, then Q.

The goal is to show that this statement is true.
1. When P is false, P => Q is always true, so we don't have to worry about this case.
2. When P is true we must show that Q is also true



*Outline of Direct Proof*

Proposition If P, then Q.

Proof. Suppose P.
...
Therefore Q.

Example:

1) Proposition If x is odd, then x^2 is odd.
Proof. Suppose x is odd.

Therefore x^2 is odd.

2) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2b + 1 by definition of an odd number.    
...    
Therefore x^2 is odd.    


3) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
...    
x^2 = 2b + 1    
Therefore x^2 is odd.    


4) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
Then x^2 = (2a + 1)^2 = 4a^2 + 4a + 1 = 2a(2a + 1) + 1    
...    
x^2 = 2b + 1    
Therefore x^2 is odd.    

5) Proposition If x is odd, then x^2 is odd.    
Proof. Suppose x is odd.    
x = 2a + 1 by definition of an odd number.    
Then x^2 = (2a + 1)^2 = 4a^2 + 4a + 1 = 2(2a^2 + 2a) + 1    
So x^2 = 2b + 1 where b = (2a^2 + 2a)    
Therefore x^2 is odd.    


Example:    

Proposition Let a, b and c be integers. If a | b and b | c, then a | c.    

1) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.    
...    
Therefore a | c    

2) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.  
By definition a | b means b = ax, b | c means c = by    
...    
Therefore a | c  

3) Proposition Let a, b and c be integers. If a | b and b | c, then a | c.  
By definition a | b means b = ax, b | c means c = by    
a | c means c = az
Therefore a | c  


Example:    

Proposition If a, b, c ∈ N , then lcm ( ca, cb ) = c · lcm ( a, b ).    

Let m = lcm(ca, cb), n = c * lcm(a, b)    
By definition lcm(a, b) is an integer divisible by a and b, then lcm(a, b) = ax = by    
So n = c * ax = c * by, but m is the *smallest* multiple of ca and cb (by definition). Thus m <= n.    
On the other hand m = lcm(ca, cb) = cax = cby by definition of lcm.    
Then 1/c * m = ax = by is a multiple of a and b. lcm(a, b) <= 1/c * m.    
But c * lcm(a, b) <= m, n <= m.    
Since m <= n and n <=m, must be that n = m.    


Example:

Proposition If x and y are positive and x <= y, then sqrt(x) <= sqrt(y).    
Subtrackt y from both sides x - y <= 0    
sqrt(x)^2 - sqrt(y)^2 <= 0    
(sqrt(x) + sqrt(y))(sqrt(x) - sqrt(y)) <= 0    
Divide both sides by positive (sqrt(x) + sqrt(y))    
sqrt(x) - sqrt(y) <= 0    
Add sqrt(y) to both sides    
sqrt(x) <= sqrt(y)    


Example:

To show that If x and y are positive real numbers, then 2 * sqrt(xy) <= x + y we can start backwards.    
Since we proved that x <= y, then sqrt(x) <= sqrt(y) we can use this property    
4xy <= (x + y)^2    
4xy <= x^2 + 2xy + y^2    
Subtrackt 4xy from both sides    
0 <= x^2 - 2xy + y^2    
0 <= (x - y)^2 which is true, because (x - y)^2 can't be negative    

Proposition If x and y are positive real numbers, then 2 * sqrt(xy) <= x + y.    
Since 0 <= (x - y)^2 holds for all x,y in Z.    
Then 0 <= x^2 - 2xy + y^2      
4xy <= x^2 + 2xy + y^2    
4xy <= (x + y)^2      
Because for all positive x, y in Z it's true that x <= y, then sqrt(x) <= sqrt(y).    
2 * sqrt(xy) <= x + y.    

Example:

Proposition If n in N , then 1 + (-1)^n * (2n - 1) is a multiple of 4.    
There are two cases:    
1) when n is even, n = 2k, k in N.   
2) when n is odd, n = 2k + 1, k in N.    

For the first case we have 1 + 1 * (2 * 2k - 1) = 1 + 4k - 1 = 4k.   
4k is a multiple of 4.   

For the second case we have 1 + ((-1)^(2k + 1)) * (2 * (2k + 1) - 1) = 1 + (-1) * (4k + 2 - 1) = -4k   
-4k is a multiple of 4.     


Example:

Proposition Every multiple of 4 equals 1 + (-1)^n * (2n - 1) for some n in N.    
There is such number k, that is divisible by 4 (k is a multiple of 4) and it can be represented as 1 + (-1)^n * (2n - 1).    

Exercises for Chapter 4    
Use the method of direct proof to prove the following statements.    
1. If x is an even integer, then x^2 is even.   
x = 2a by definition, then x^2 = (2a)^2 = 4a^2 = 2(2a^2).    
So x^2 = 2b, where b = 2a^2.    
By definition of an even number x^2 is even.    


2. If x is an odd integer, then x^3 is odd.
x = 2a + 1 by definition of an odd number.    
Then x^3 = (2a + 1)^3 = (2a)^3 + 3(2a)^2 + 3(2a) + 1 = 8a^3 + 12a^2 + 6a + 1 =     
= 2(4a^3 + 6a^2 + 3a) + 1.    
So x^3 = 2b + 1, where b = 4a^3 + 6a^2 + 3a.    


3. If a is an odd integer, then a^2 + 3a + 5 is odd.    
a = 2b + 1 by definition of an odd number.    
(2b + 1)^2 + 3(2b + 1) + 5 = 4b^2 + 4b + 1 + 6b+ 3 + 5 = 4b^2 + 10b + 8 + 1 = 2(2b^2 + 5b + 4) + 1.    
So a^2 + 3a + 5 = 2c + 1, where c = 2b^2 + 5b + 4.    
By definition of an odd number, a^2 + 3a + 5 is odd.    


4. Suppose x, y in Z. If x and y are odd, then xy is odd.    
Let x = 2a + 1, y = 2b + 1.    
Then xy = (2a + 1)(2b + 1) = 4ab + 2a + 2b + 1 = 2(2ab + a + b) + 1.    
So xy = 2c + 1, where c = 2ab + a + b.    


5. Suppose x, y in Z. If x is even, then xy is even.    
Let x = 2a.    
Two cases:    
1) y = 2b.    
Then xy = 2a * 2b = 2(ab).    
So xy = 2c, where c = ab.    
By definition xy is even.    
2) y = 2b + 1.    
Then xy = 2a * (2b + 1) = 4ab + 2a = 2(2ab + a).    
So xy = 2c, where c = 2ab + a.    
By definition xy is even.   
In both cases xy is even, then it's even.    


6. Suppose a, b, c in Z. If a | b and a | c, then a | (b + c).    
By definition, a | b => b = an, a | c => c = am, a | (b + c) => (b + c) = ak.    
(b + c) = an + am = a (mn).    
So (b + c) = ak, where k = mn => a | (b + c).    


7. Suppose a, b in Z . If a | b , then a^2 | b^2.    
a | b => b = an, a^2 | b^2 => b^2 = a^2 m.    
So b = an, and b^2 = a^2 n^2.    
Then b^2 = a^2 m, where m = n^2.    


8. Suppose a is an integer. If 5 | 2a, then 5 | a.    
5 | 2a => 2a = 5n, 5 | a => a = 5m.    
2a is even, then 5n is even, so n must be even too.    
n = 2k, 2a = 5(2k) = 10k, a = 5k.    
Since a = 5k and a = 5m, m = k.    


9. Suppose a is an integer. If 7 | 4a, then 7 | a.    
7 | 4a, then 4a = 7n.    
4a = 2(2a), then 4a is even, so 7n even and n must be even too.    
n = 2k, 4a = 7(2k) = 14k, 2a = 7k, but 2a is even, so 7k is even and k must be even too.    
k = 2r, 2a = 7(2r) = 14r, a = 7r.    
Since 7 | a, then a = 7b, and since a = 7r, then it must be than b = r.    


10. Suppose a and b are integers. If a | b, then a | (3b^3 - b^2 + S5b).    
a | b => b = an.    
a | (3b^3 - b^2 + 5b) => 3b^3 - b^2 + 5b = am.    


11. Suppose a, b, c, d in Z . If a | b and c | d, then ac | bd.     
a | b => b = an, c | d => d = cm, ac | bd => bd = ack.    
bd = an * cm = ac(nm) => bd = ack, where k = nm.    


13. Suppose x, y in R. If x^2 + 5y = y^2 + 5x, then x = y or x + y = 5.    
x^2 - y^2 = 5x - 5y.    
(x + y)(x - y) = 5(x - y).   
1) If (x - y) not equal to 0, then x + y = 5.    
2) If (x - y) is equal to zero, then x - y = 0, => x = y.    


14. If n in Z , then 5n^2 + 3n + 7 is odd. (Try cases.).    
There are three cases:    
1) When n = 0.    
5n^2 + 3n + 7, 7 is odd.    
2) When n is even.    
n = 2a.    
5(2a)^2 + 3(2a) + 7 = 20a^2 + 6a + 6 + 1 = 2(10a^2 + 3a + 3) + 1.    
So 5n^2 + 3n + 7 = 2b + 1, where b = (10a^2 + 3a + 3).    
3) When n is odd.    
n = 2a + 1.     
5(2a + 1)^2 + 3(2a + 1) + 7 = 5(4a^2 + 4a + 1) + 6a + 3 + 7 = 20a^2 + 20a + 5 + 6a + 10 =     
= 20a^2 + 26a + 14 + 1 = 2(10a^2 + 13a + 7) + 1.     
So 5n^2 + 3n + 7 = 2c + 1, where c = (10a^2 + 13a + 7).     



15. If n in Z , then n^2 + 3n + 4 is even. (Try cases.).     
1) When n = 0.    
4 is even.    
2) When n is even.    
n = 2a.    
(2a)^2 + 3(2a) + 4 = 4a^2 + 6a + 4 = 2(2a^2 + 3a + 2).     
n^2 + 3n + 4 = 2b, where b = (2a^2 + 3a + 2).     
3) When n is odd.     
n = 2a + 1.    
(2a + 1)^2 + 3(2a + 1) + 4 = 4a^2 + 4a + 1 + 6a + 3 + 4 = 4a^2 + 10a + 8 = 2(2a^2 + 5a + 4).    
n^2 + 3n + 4 = 2c, where c = (2a^2 + 5a + 4).    



16. If two integers have the same parity, then their sum is even. (Try cases.).    
1) If both integers are even.    
x = 2a, y = 2b.    
2a + 2b = 2(a + b).    
x + y = 2c, where c = (a + b).    
2) If both integers are odd.    
x = 2a + 1, y = 2b + 1.    
2a + 1 + 2b + 1 = 2a + 2b + 2 = 2(a + b + 1).    
x + y = 2d, where d = (a + b + 1).    



17. If two integers have opposite parity, then their product is even.    
Let x = 2a, y = 2b + 1.    
xy = 2a * (2b + 1) = 4ab + 2a = 2(2ab + a).    
xy = 2c, where c = (2ab + a).    



18. Suppose x and y are positive real numbers. If x < y, then x^2 < y^2.    
x^2 < y^2.    
x^2 - y^2 < 0.    
(x - y)(x + y) < 0.    
Because x and y are positive we can divide both sides by (x + y).    
x - y < 0.    
x < y.     



19. Suppose a, b and c are integers. If a^2 | b and b^3 | c , then a^6 | c.    
b = xa^2, c = yb^3.    
c = y(xa^2)^3 = yx^3a^6.    
So c = a^6z, where z = yx^3.    



20. If a is an integer and a^2 | a, then a in { -1, 0, 1 }.    
a = xa^2.    
xa^2 - a = 0.    
a(xa - 1) = 0.    
Either a = 0, or xa - 1 = 0.    
In the first case a in { 0 }.    
In the second case xa = 1.    
a = 1/x.    
So x is either -1, or 1.    
That means a in { -1, 0, 1 }.    



25. If a, b, c in N and c <= b <= a, then (a choose b)(b choose c) = (a choose (b-c))((a-b+c) choose c)
(a!/(b!(a-b)!))(b!/(c!(b-c)!)) = (a!/(b-c)!)((a-b+c)!/(c!(a-b+c)!(a-b)!)) = (a!/(b-c)!(a-b+c)!)((a-b)!c!) =     
= (a!/((b-c)!(a-b+c)!))(a-b+c)!/(c!(a-b+c-c)!)     
