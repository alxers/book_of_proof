Functions     


Definition 12.1 Suppose A and B are sets. A function f from A to B (denoted as f : A -> B) is a relation f set_in A x B from A to B, satisfying theproperty that for each a in A the relation f contains exactly one ordered pair of form (a,b). The statement (a,b) in f is abbreviated f(a) = b.     


Definition 12.2 For a function f : A -> B, the set A is called the domain off. (Think of the domain as the set of possible "input values" for f.) Theset B is called the codomainoff. The range of f is the set { f(a) : a in A } = { b : (a, b) in f }. (Think of the range as the set of all possible "output values" for f. Think of the codomain as a sort of "target" for the outputs.).       


Exercises for Section 12.1.      
.1. Suppose A = { 0, 1, 2, 3, 4 }, B = { 2, 3, 4, 5 } and f = { (0, 3), (1, 3), (2, 4), (3, 2), (4, 2) }. State the domain and range of f. Find f(2) and f(1).      
Domain = A, range = { 2, 3, 4 }, f(2) = 4, f(1) = 3.     


.2. Suppose A = { a, b, c, d }, B = { 2, 3, 4, 5, 6 } and f = { (a, 2), (b, 3), (c, 4), (d, 5) }. State the domain and range off. Find f(b) and f(d).      
Domain = A, range = { 2, 3, 4, 5 }, f(b) = 3, f(d) = 5.       


.3. There are four different functions f : { a, b } -> { 0, 1 }. List them. Diagrams suffice.     
f_1 = { (a, 0), (b, 0) }, f_2 = { (a, 1), (b, 0) }, f_3 = { (a, 0), (b, 1) } f_4 = { (a, 1), (b, 1) }.     


.5. Give an example of a relation from { a, b, c, d } to { d, e } that is not a function.     
f = { (a, d), (b, e) }. By definition of a function it should be for all a in A. (???).     


.6. Suppose f : Z -> Z is defined as f = { (x,4x+5) : x in Z }. State the domain, codomainand range off. Find f (10).     
Domain = A, codomain = Z, range f(x) = 4x + 5 {..., 9, 13, 17, ... } (???).     
f(10) = 45.      


.7. Consider the set f = { (x, y) in Z x Z : 3x + y = 4 }. Is this a function from Z to Z? Explain.      
It's a function.     
y = 4 - 3x.     


.8. Consider the set f = { (x, y) in Z x Z : x + 3y = 4 }. Is this a function from Z to Z? Explain.   
y = (4 - x)/3.     
Not from Z to Z.      


.9. Consider the set f = { (x^2, x) : x in R }. Is this a function from R to R? Explain.     
It's possible to have x = 2, x^2 = 4, x = -2, x^2 = 4.     
y definition of a function it should be that for all a in A there is exactly one ordered pair (a, b).      
So f is not a function.      


.10. Consider the set f = { (x^3, x) : x in R }. Is this a function from R to R? Explain.     
f is a function.      


.11. Is the set theta = { (X,|X|) : X set_in Z_5 } a function? If so, what is its domain and range?     



Functions Exercises for Section 12.2.       

.2. Consider the logarithm function ln : (0, inf) -> R. Decide whether this function is injective and whether it is surjective.     
a) Injective. Suppose a, a' in (0, inf) and f(a) = f(a').     
ln(a) = ln(a').     
e^(ln(a)) = e^(ln(a')).     
a = a'.     
b) Surjective. For all b in R, exists such a in (0, inf) such that f(a) = b.     
a = e^b.     
ln(e^b) = b.     


.4. A function f : Z -> Z x Z is defined as f(n) = (2n, n+3). Verify whether this functionis injective and whether it is surjective.     
a) Injective. Suppose a, a' in Z and f(a) = f(a').     
(2a, a + 3) = (2a', a' + 3).     
2a = 2a'.     
a + 3 = a' + 3.     
a = a'.     
b) Surjective. For all (b, c) in Z x Z exists such x in Z such that f(x) = (b, c).     
(2x, x + 3) = (b, c).      
2x = b.     
x + 3 = c.     
x - 3 = b - c.     
x = b - c + 3.     
f(b - c + 3) = (2(b - c + 3), b - c + 3 + 3).     
f(x) != (b, c).     
( b) is probably incorrect).     

.6. A function f : Z x Z -> Z is defined as f(m, n) = 3n - 4m. Verify whether this function is injective and whether it is surjective.      
a) Injective
b) Consider arbitrary element b in Z. We need to show that there is some x, y in Z, for which f(x, y) = b.     



.8. A function f : Z x Z -> Z x Z is defined as f(m, n) = (m + n, 2m + n). Verify whether this function is injective and whether it is surjective.     
a) Suppose (m, n), (k, l) in Z x Z and f(m, n) = f(k, l).     
Then (m + n, 2m + n) = (k + l, 2k + l).     
m + n = k + l.     
2m + n = 2k + l.     
m = k => n = l.     
f is injective.     
b) Consider (b, c) in Z x Z.    
Show that there is some (x, y) in Z x Z for which f(x, y) = (b, c).     
f(x, y) = (x + y, 2x + y).     
(x + y, 2x + y) = (b, c).     
x + y = b.     
2x + y = c.     
2(b - y) + y = c.     
2b - 2y + y = c.     
2b - y = c.     
2b - c = y.     
x = b - y, y = 2b - c.     
x = b - (2b - c).     
x = -b + c.     
(x, y) = (-b + c, 2b - c).     
f(-b + c, 2b - c) = (-b + c + 2b - c, 2(-b + c) + 2b - c) = (b, c).     
f is surjective.     



.10. Prove the function f : R - {1} -> R - {1} defined by f(x)=((x+1)/(x-1))^3 is bijective.     
a) Injective. Suppose a, a' in R - {1} and f(a) = f(a').      
We need to show that a = a'.     
((a+1)/(a-1))^3 = ((a'+1)/(a'-1))^3.     
(a + 1)(a' - 1) = (a - 1)(a' + 1).     
aa' - a + a' - 1 = aa' + a - a' - 1.     
-2a = -2a'
a = a'.     
f is injective.     
b) Surjective. For all b in R - {1}, exists such a in R - {1} for which f(a) = b.     
((a+1)/(a-1))^3.      
(a + 1)/(a - 1) = b^(1/3).     
a + 1 = (a - 1) * b^(1/3).     
a + 1 = b^(1/3) * a - b^(1/3).     
a - ab^(1/3) = -b^(1/3) - 1.     
a(1 - b^(1/3)) = -b^(1/3) - 1.     
a = (-b^(1/3) - 1)/(1 - b^(1/3)).     
Since b != 1, such a exists.     
f is surjective.     


.12. Consider the function theta : {0,1} x N -> Z defined as theta(a,b) = a - 2ab + b. Is theta injective? Is it surjective? Bijective? Explain.     
a) Suppose a,a', b, b' in { 0, 1 } x N and f(a, b) = f(a', b').     
a - 2ab + b = a' - 2a'b' + b'.     
a + b(-2a + 1) = a' + b'(-2a' + 1).     
a, a' in { 0, 1 } => b = b'.     
a = a'.     
b) c = 0, c in Z, since b != 0, f(a, b) != c.     
(probably wrong).     


.16. This question concerns functions f : { A, B, C, D, E } -> { 1, 2, 3, 4, 5, 6, 7 }. How many such functions are there? How many of these functions are injective? How manyare surjective? How many are bijective?      
f(A), f(B), f(C), f(D), f(E)
 7     7     7     7     7       
7^5 functions.      
A B C D E      
7 6 5 4 3      
Injective functions = 7 * 6 * 5 * 4 * 3.     
Surjective = 0.     
Bijective = 0.      


.18. Prove that the function f : N -> Z defined as f(n) = ((-1)^n(2n - 1) + 1)/4     
a) Injective. Suppose a, a' in N and f(a) = f(a').      
((-1)^a(2a - 1) + 1)/4 = ((-1)^a'(2a' - 1) + 1)/4      
(-1)^a(2a - 1) = (-1)^a'(2a' - 1).       
(-1)^a = (-1)^a' - they have the same sign.      
a = a'.      
(check a) step).     
b) Surjective. For all b in Z, exists such a in N for which f(a) = b.     
((-1)^a(2a - 1) + 1)/4 = b.     
(-1)^a(2a - 1) = 4b - 1.     
Two options here, a - even, a - odd.     
Suppose a is even.     
2a - 1 = 4b - 1.     
2a = 4b.      
a = 2b.      
Suppose a is odd.      
-2a + 1 = 4b - 1.     
-2a = 4b - 2.      
a = 1 - 2b.     
When a is odd, then f(a) in (-inf, 0].     
When a is even, then f(a) in [1, +inf).      




The Pigeonhole Principle (function).     
Suppose A and B are finite sets and f : A -> B is any function.     
1. If |A| > |B|, then f is not injective.     
2. If |A| < |B|, then f is not surjective.     



Exercises for Section 12.3.      
.4. Consider a square whose side-length is one unit. Select any five points from inside this square. Prove that at least two of these points are withi sqrt(2)/2 units of each other.      
Divide square into 4 parts. At least two points has to be in one little square.      
Max distance within square is its diagonal.     
c^2 = 0.5^2 + 0.5^2.     
c = sqrt(2)/2.       


.6. Given a sphere S, agreat circle of S is the intersection of S with a plane through its center. Every great circle divides S into two parts. A hemisphere is the union of the great circle and one of these two parts. Prove that if five points are placed arbitrarily on S, then there is a hemisphere that contains four of them.       
Divide sphere into two parts by plane.      
Make a plain using center and two arbitraty points.      
We get two hemispheres and 3 points left.      
Two of them must end up on one hemisphere.     
So one closed hemisphere must contain 4 points.      



Exercises for Section 12.4.      
.2. Suppose A = {1,2,3,4}, B = {0,1,2}, C = {1,2,3}. Let f:A -> B be f = {(1,0),(2,1),(3,2),(4,0)}, and g:B -> C be g = {(0,1),(1,1),(2,3)}. Find g o f.     
g o f : A -> C = { (1, 1), (2, 1), (3, 3), (4, 1) }.       


.6. Consider the functions f,g : R -> R defined as f(x)=1/(x^2+1) and g(x)=3x+2. Find the formulas for g o f and f o g.      
g o f = 3/(x^2 + 1) + 2, f o g = 1/((3x+2)^2 + 1).      


.8. Consider the functions f,g : ZxZ -> ZxZ defined as f(m,n)=(3m-4n,2m+n) and g(m,n)=(5m+n,m). Find the formulas for g o f and f o g.       
g o f = g(3m - 4n, 2m + n) = (5(3m-4n) + n, 3m - 4n).       
f o g = f(5m + n, m) = (3(5m + n) - 4m, 2(5m + n) + m).      


.10. Consider the function f:R^2 -> R^2 defined by the formula f(x,y)=(x y,x^3). Find a formula for f o f.     
f(xy, x^3) = (xy * x^3, x^3y^3).      




Exercises for Section 12.5.      
.2. In Exercise 9 of Section 12.2 you proved that f:R-{2} -> R-{5} defined by f(x)=(5x+1)/(x-2) is bijective. Now find its inverse.      
y = (5x+1)/(x-2).     
x = (5y+1)/(y-2)      
x(y - 2) = 5y + 1       
xy - 2x = 5y + 1       
-2x - 1 = 5y - xy      
-2x - 1 = y(5 - x)      
(-2x - 1)/(5 - x) = y.      


.4. The function f:R -> (0, inf) defined as f(x)=e^(x^3+1) is bijective. Find its inverse.      
y = e^(x^3 + 1)      
x = e^(y^3 + 1)       
ln(x) = ln(e^(x^3 + 1))      
ln(x) = y^3 + 1       
ln(x) - 1 = y^3       
(ln(x) - 1)^(1/3) = y.       


.6. The function f:ZxZ -> ZxZ defined by the formula f(m,n)=(5m+4n,4m+3n)is bijective. Find its inverse.       
(x, y) = f(m, n)      
(m, n) = f(x, y)      
(m, n) = (5x + 4y, 4x + 3y)      
5x + 4y = m      
4x + 3y = n       
x + y = m - n       
x = m - n - y      
4(m - n - y) + 3y = n      
4m - 4n - 4y + 3y = n       
-y = n + 4n - 4m      
y = 4m - 5n      
x = -3m + 4n      
f^(-1)(m, n) = (-3m + 4n, 4m - 5n).      



Exercises for Section 12.6.      


.2. Consider the function f : {1,2,3,4,5,6,7} -> {0,1,2,3,4,5,6,7,8,9} given as f={(1,3),(2,8),(3,3),(4,1),(5,2),(6,4),(7,6)}. Find: f({1,2,3}),f({4,5,6,7}),f(empty_set),f^(-1)({0,5,9}) and f^(-1)({0,3,5,9}).      
f({ 1, 2, 3}) = { 3, 8 }.      
f({ 4, 5, 6, 7 }) = { 1, 2, 4, 6 }.      
f(empty_set) = empty_set.      
f^(-1)({ 0, 5, 9 }) = empty_set.     
f^(-1)({ 0, 3, 5, 9 }) = { 1, 3 }.     


.8. Given a function f:A -> B and subsets W,X set_in A, then f(W intersection X)=f(W) intersection f(X) is false in general. Produce a counterexample.      
Let W = { 1, 2 }, X = { 1, 3 }.     
W intersection X = { 1 }.      
Let A = { 1, 2, 3 }, B = { 0, 1, 2 }.      
f = { (1, 0), (2, 1), (3, 1) }.       
Then f(W intersection X) = 0.      
f(W) = {0, 1}.      
f(X) = {0, 1}.      
f(W) intersection f(X) = { 0, 1 }.     
f(W intersection X) != f(W) intersection f(X).       


