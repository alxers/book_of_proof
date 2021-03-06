Set is a collection of things
If X is a finite set, its cardinality (size) is the number of elements it has, denoted as |X|.

Set-builder notation:
E = { ... -6, -4, -2, 0, 2, 4, 6 ... }
[!set_builder][img/set_builder_1.png]

E equals the set of all things of form 2n, such that n is an element of Z

*Exercises for Section 1.1 (page 7)*
A. Write each of the following sets by listing their elements between braces.

1. { 5x-1 : x in Z }

	{ ... -11, -6, -1, 4, 9, ... }

3. { x in Z : -2 <= x < 7 }

	{-2, -1, 0, 1, 2, 3, 4, 5, 6}

5. { x in R : x^2 = 3 }

	{ +sqrt(3), -sqrt(3) }

7. { x in R : x^2 + 5x = -6 }

	{ -3, -2 }

9. { x in R : sin(pi\*x) = 0 }

	{ Z } https://www.wolframalpha.com/input/?i=sin(pi*x)%3D0

11. { x in Z : |x| < 5 }

	{ -4, -3, -2, -1, 0, 1, 2, 3, 4 }

14. { 5x : x in Z, |2x| <= 8 }

	{ -20, -15, -10, 0, 10, 15, 20 } 

16. { 6a + 2b : a, b in Z }

	{ Z } ( 6a + 2b is a linear combination => can express any number in Z) ?

B. Write each of the following sets in set-builder notation.

17. { 2, 4, 8, 16, 32, 64, ... }

	{ 2^x : x in N }

18. { 0, 4, 16, 36, 64, 100, ... }

	{ 4(x - 1)^2 : x in N }

19. {..., -6, -3, 0, 3, 6, 9, 12, 15, ... }

	{ 3x : x in Z }

20. { ..., -8, -3, 2, 7, 12, 17, ... }

	{ 5x - 13 : x in Z }

21. { 0, 1, 4, 9, 16, 25, 36, ... }

	{ |n|^x : x in Z, n in N }
	{ (x - 1)^2 : x in N }

22. { 3, 6, 11, 18, 27, 38, ... }

	{ x^2 + 2 : x in N }

23. { 3, 4, 5, 6, 7, 8 }

	{ x in N : 2 < x < 9 }

25. { ..., 1/8, 1/4, 1/2, 1, 2, 4, 8, ... }

	{ 2^x : x in Z }

28. { ..., -3/2, -3/4, 0, 3/4, 3/2, 9/4, 3, 15/4, 9/2, ... }

	? The next el is prev_el * ((x+1)/x), f.e. 3/4*(2/1) = 3/2, 3/2*(3/2) = 9/4, 9/4*(4/3) = 3, ...

	{ 3x/4 : x in Z }

C. Find the following cardinalities.

29. | {{1}, {2, {3, 4}}, empty_set} | = 3 (empty_set = {})

33. | { x in Z : |x| < 10 } | = | { -9, -8, -7, -6, -5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 } | = 19

36. | { x in N : x^2 < 10 } | = | { 1, 2, 3 } | = 3

37. | { x in N : x^2 < 0 } | = | {} | = | empty_set | = 1

38. | { x in N : 5x <= 20 } | = | { 5, 10, 15, 20 } | = 4


The Cartesian Product

Given two sets A and B, it's possible to "mulitply" them. A x B will produce a new set. This operation is called the Cartesian product.

Definition. An ordered pair is a list (x, y) of two things.
F.e. (2, 4) and (4, 2) are different ordered pairs.
Ordered pairs don't have to be numbers.

Definition. The Cartesian product of two sets A and B is another set, denoted as A x B and defined as A x B = {(a, b) : a in A, b in B}.

Cartesian powers of sets.
A^n is a cartesian product of A with itself n times:
A^n = A x A x ... x A = { (x1, x2,..., x_n) : x1, x2,..., x_n in A }.

Exercises for Section 1.2

1. A = { 1, 2, 3, 4 }, B = { a, c }

(a) A x B = { (1, a), (1, c), (2, a), (2, c), (3, a), (3, c), (4, a), (4, c) }    
(b) B x A = { (a, 1), (a, 2), (a, 3), (a, 4), (c, 1), (c, 2), (c, 3), (c, 4) }    
(c) A x A = { (1, 1), (2, 2), (3, 3), (4, 4) }    
(e) {} x B = {}    
(h) B^3 = B x B x B = { (a, a), (a, c), (c, a) } x { a, c } = { (a, (a, a)), (c, (a, a)), (a, (a, c)), (c, (a, c)), (a, (c, a)), (c, (c, a)) }    

2. A = { pi, e, 0 }, B = { 0, 1 }    
(a) A x B = { (pi, 0), (pi, 1), (e, 0), (e, 1), (0, 0), (0, 1) }   


Exercises for Section 1.3    
*For the set of n elements there are 2^n subsets*

B = { 1, 2, { 1, 3 } }
{ 1, 3 } is NOT a subset of B. It can't be made by selecting elements from B, as 3 is not an element of B.
{ 1, 3 } not set_in B, but { 1, 3 } in B. Also { { 1, 3 } } set_in B

1 is not a subset of { 1, { 1 } }, because 1 is not a set
1 is an element of set { 1, { 1 } }
{ 1 } is a subset of { 1, { 1 } }

A. List all the subsets of the following sets.    
1. { 1, 2, 3, 4 }    
{}, { 1 }, { 2 }, { 3 },    
{ 4 }, { 1, 2 } { 1, 3 }, { 1, 4 },           
{ 2, 3 }, { 2, 4 }, { 3, 4 }, { 1, 2, 3 },           
{ 1, 2, 4 } { 1, 3, 4 }, { 2, 3, 4 }, { 1, 2, 3, 4 }        

2. { 1, 2, {} }
{}, { 1 }, { 2 }, { {} }, { 1, 2 }, { 1, {} }, { 2, {} }, { 1, 2, {} }    

3. { { R } }    
{}, { { R } }    

4. {}    
{}    

5. {{}}    
{}, {{}}    

6. { R, Q, N }   
{}, { R }, { Q }, { N }, { R, Q }, { R, N }, { Q, N }, { R, Q, N }    

7. { R, { Q, N } }    
{}, { R }, { { Q, N } }, { R, { Q, N } }     

B. Write out the following sets by listing their elements between braces.

9. { X : X set_in { 3, 2, a } and |X| = 2 }    
{ 3, a } (a set of any two elements)?    

10. { X set_in N : |X| <= 1 }    
{ 1 }    

11. { X : X set_in { 3, 2, a } and |X| = 4 }    
{ {}, 3, 2, a } ?    

12. { X : X set_in { 3, 2, a } and |X| = 1 }    
{ a }    

C. Decide if the following are true or false. Explain

13. R^3 set_in R^3    
True, each set is its own subset    

14. R^2 set_in R^3
True, R^2 is a plane in R^3

15. { (x, y) : x - 1 = 0  } set_in { (x, y) : x^2 - x = 0 }    
True
x = 1, y = any    
1^2 - 1 = 0

First set { (1, y) : for any y }       
Second set { (1, y), (0, y) : for any y }    

16. { (x, y) : x^2 - x = 0  } set_in { (x, y) : x - 1 = 0 }    
False    


Power sets.    
If A is a set, the power set of A is another set P(A) - the set of all subsets of A.
P(A) = { X : X set_in A }

Example:    
A = { 1, 2, 3 }    
P(A) = { {}, { 1 }, { 2 }, { 3 }, { 1, 2 }, { 1, 3 }, { 2, 3 }, { 1, 2, 3 } }    

If A is a finite set, then |P(A)| = 2^|A|    


Exercises for Section 1.4    

A. Find the indicated sets.    
1. P({ { a, b }, { c } }) = { {}, { { a, b } }, { { c } }, { { a, b }, { c } } }    

3. P({ { {} }, 5 }) = { {}, { {} }, { 5 }, { {}, 5 } }    

5. P(P({ 2 })) = P({ {}, { 2 } }) = { {}, { {} }, { 2 }, { {}, { 2 } } }    

6. P({ 1, 2 }) x P({ 3 }) = { {}, { 1 }, { 2 }, { 1, 2 } } x { {}, { 3 } } = 
= { ({}, {}), ({}, { 3 }), ({ 1 }, {}), ({ 1 }, { 3 }), ({ 2 }, {}), ({ 2 }, { 3 }), ({ 1, 2 }, {}), ({ 1, 2 }, { 3 }) }    

9. P({ 1, 2 } x { 0 }) = P({ (1, 0), (2, 0) }) = { {}, { (1, 0) }, { (2, 0) }, { (1, 0), (2, 0) }}    

10. { X in P({ 1, 2, 3 }) : |X| <= 1 } =    
= { X in { {}, { 1 }, { 2 }, { 3 }, { 1, 2 }, { 1, 3 }, { 2, 3 }, { 1, 2, 3 } } : |X| <= 1 } = { {}, { 1 }, { 2 }, { 3 } }    

11. { X set_in P({ 1, 2, 3 }) : |X| <= 1 }    
All subsets of P({ 1, 2, 3 }) are
{ {} }, { { 1 } }, { { 2 } }, { { 3 } }, { { 1, 2 } }, { { 2, 3 } }
{ { 1, 2, 3 } }    
So X is all of the above, all this sets cardinality is 1
The answer is 
{ { {} }, { { 1 } }, { { 2 } }, { { 3 } }, { { 1, 2 } }, { { 2, 3 } }, { { 1, 3 } }, { { 1, 2, 3 } } }    

12. { X in P({ 1, 2, 3 }) : 2 in X }
P({ 1, 2, 3 }) = { {}, { 1 }, { 2 }, { 3 }, { 1, 2 }, { 1, 3 }, { 2, 3 }, { 1, 2, 3 } }

{ { 2 }, { 1, 2 }, { 2, 3 }, { 1, 2, 3 } }    

Suppose that |A| = m and |B| = n. Find the following cardinalities.    
13. |P(P(P(A)))|

Because |P(A)| = 2^|A|

2^|P(P(A))|
2^(2^|P(A)|)
2^(2^(2^|A|))
2^(2^(2^m))


15. |P(A x B)| = 2^|(A x B)|

Because |A x B| = |A| * |B| (see cartesian product properties, cardinality)

2^|A x B| = 2^(|A| * |B|) = 2^(m * n)


16. |P(A) x P(B)| = |P(A)| * |P(B)| = 2^|A| * 2^|B| = 2^m * 2^n = 2^(m+n)    

17. |{ X in P(A) : |X| <= 1 }| ?

18. |P(A x P(B))| = 2^(|(A x P(B))|) = 2^(|A| * |P(B)|) = 2^(m * 2^|B|) = 2^(m * 2^(n))

20. |{ X set_in P(A) : |X| <= 1}|
All subsets of P(A) are { {} }, { A1 }, { A2 } ... { A }
X is all of them, all this sets cardinality is 1
=> |{ { {} }, { A1 }, { A2 } ... { A } }| = 1
or |{ 2^|A| }| = |{ 2^m }| which is still eq to 1
?


1.5 Union, Itersection, Difference

Definition 1.5 Suppose A and B are sets

The union of A and B = { x : x in A or x in B }
The intersection of A and B = { x : x in A and x in B }
The difference of A and B is the set A - B = { x : x in A and x not_in B }

Exercises for Section 1.5

1. Suppose A = { 4, 3, 6, 7, 1, 9 }, B = { 5, 6, 8, 4 }, C = { 5, 8, 4 }

(a) A union B = { 4, 3, 6, 7, 1, 9, 5, 8 }
(b) A intersection B = { 4, 6 }
(c) A - B = { 3, 7, 1, 9 }
(d) A - C = { 3, 6, 7, 1, 9 }
(e) B - A = { 6 }
(f) A intersection C = { 4 }
(i) C - B = {}

2. Suppose A = { 0, 2, 4, 6, 8 }, B = { 1, 3, 5, 7 }, C = { 2, 8, 4 }

(a) A union B = { 0, 1, 2, 3, 4, 5, 6, 7, 8 }
(b) A intersection B = {}
(c) A - B = {}
(i) C - B = { 2, 8, 4 }

3. Suppose A = { 0, 1 } and B = { 1, 2 }

(a) (A x B) intersection (B x B) = { (0, 1), (0, 2), (1, 1), (1, 2) } intersection { (1, 1), (1, 2), (2, 1), (2, 2) } = 
= { (1, 1), (1, 2) }
(d) (A intersection B) x A = { 1 } x { 0, 1 } = { (1, 0), (1, 1) }
(f) P(A) intersection P(B) = { {}, { 0 }, { 1 }, { 0, 1 } } intersection { {}, { 1 }, { 2 }, { 1, 2 } } = { {}, { 1 } }
(h) P(A intersection B) = P({ 1 }) = { {}, { 1 } }
(i) P(A x B) = P({ (0, 1), (0, 2), (1, 1), (1, 2) })

4. Suppose A = { b, c, d } and B = { a, b }
(a) (A x B) intersection (B x B) = { (b, a), (b, b), (c, a), (c, b), (d, a), (d, b) } intersection { (a, a), (a, b), (b, a), (b, b) } = { (b, b) }
(b) (A intersection B) x A = { b } x { a, b }
(f) P(A) intersection P(B) = { {}, { b }, { c }, { d }, { b, c }, { b, d }, { c, d }, { b, c, d } } intersection { {}, { a }, { b }, { a, b } } = { {}, { b } }


1.6 Complement

N - is a set of natural numbers and f.e. P = { 2, 3, 5, 7, 11, ... }
P set_in N, the larger set N is called *universal set* or *universe* for P.
In the absence of specifics, if A is a set (we don't know what's in it), then its universal set is often denoted as U.

Definition 1.6
Let A be a set with a universal set U. The *complement* of A(complement), is a set A(complement) = U - A.

Example 1.7 
If P is the set of prime numbers, then P(complement) = N - P = { 1, 4, 6, 8, 10, ... }
Thus P(complement) is the set of composite numbers and 1.


Exercises for Section 1.6

1. Let A = { 4, 3, 6, 7, 1, 9 }, B = { 5, 6, 8, 4 }, universal set U = { 0, 1, 2, ..., 10 }. Find:
(a) A(complement) = U - A = { 0, 2, 5, 8, 10 }
(c) A intersection A(complement) = {}
(d) A union A(complement) = U
(e) A - A(complement) = A
(f) A - B(complement) = { 4, 3, 6, 7, 1, 9 } - { 0, 1, 2, 3, 7, 9, 10 } = { 4, 6 }
(g) A(complement) - B(complement) = { 0, 2, 5, 8, 10 } - { 0, 1, 2, 3, 7, 9, 10 } = { 5, 8 }
(i) (A(complement) intersection B)(complement) = { 5, 8 }(complement) = { 0, 1, 2, 3, 4, 6, 7, 9, 10 }

2. Let A = { 0, 2, 4, 6, 8 }, B = { 1, 3, 5, 7 }, U = { 0, 1, 2, 3, 4, 5, 6, 7, 8 }
(a) A(complement) = U - A = { 1, 3, 5, 7 }
(b) B(complement) = U - B = { 0, 2, 4, 6, 8 }
(c) A intersection A(complement) = {}
(d) A union A(complement) = {}
(e) A - A(complement) = { 0, 2, 4, 6, 8 }
(f) A - B(complement) = {}
(g) A(complement) - B(complement) = { 1, 3, 5, 7 }
(h) (A intersection B)(complement) = {}(complement) = U - {} = U
(i) A(complement) x B = B^2

1.8 Indexed Sets
Definitions:
Union(from i=1 to n) A_i = A_1 union A_2 union ... union A_n
Union(alpha in I) A_alpha = { x : x in A_alpha for at least one set A_aplha with alpha in I }


Exercises for Section 1.8

1. Suppose A_1 = { a, b, d, e, g, f }, A_2 = { a, b, c, d }, A_3 = { b, d, a }, A_4 = { a, b, h }

(a) Union(from i=1 to 4) A_i = { a, b, c, d, e, f, g, h }
(b) Intersection(from i=1 to 4) A_i = { a, b }

3. For each n in N, let A_n = { 0, 1, 2, 3, ..., n }
(a) Union(i in N) A_i = A_1 union A_2 union ... union A_n = { 0, 1, 2, 3, ..., n }
(b) Intersection(i in N) A_i = { 0, 1 }

4. For each n in N, let A_n = { -2n, 0, 2n }
(a) Union(i in N) A_i = { all positive and negative even numbers with 0 }
(b) Intersection(i in N) A_i = { -2, 0, 2 }

5. (a) Union(i in N)[i, i+1] = { [1, 2], [2, 3], ... } ?
(b) Intersection(i in N)[i, i+1] = {}

* Union(i in [0, 2])[1, 2] x { i } = [1, 2] x [0, 2]

8. (a) Union(alpha in R) { alpha } x [0, 1] = R ?
(b) Intersection(alpha in R) { alpha } x [0, 1] = {} ?

9. (a) Union(X in P(N)) X = { 1 }, { 2 }, { 3 }, ..., = N
(b) Intersection(X in P(N)) X = {}

10. (a) Union(x in [0, 1]) [x, 1] x [0, x^2] = [0, 1] x [0, 0] union [1, 1] x [ 0, 1] ?

11. Is Intersection(alpha in I) A_alpha set_in Union(alpha in I) A_alpha always true for any collection of sets A_alpha with index set I?
If Intersection(alpha in I) A_alpha = {} then {} might not be set_in A_alpha set_in Union(alpha in I) A_alpha

12. If Intersection(alpha in I) A_alpha = Union(alpha in I) A_alpha, then A_alpha is the same set?

13. If J != {} and J set_in I, does it follow that Union(alpha in J) A_alpha set_in Union(alpha in I) A_alpha ? What about Intersection(alpha in J) A_alpha set_in Intersection(alpha in I) A_alpha    ?
