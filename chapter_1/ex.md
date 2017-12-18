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


Exercises for Section 1.2    

A. List all the subsets of the following sets.    
1. { 1, 2, 3, 4 }    
{}, { 1 }, { 2 }, { 3 }, { 4 }, { 1, 2 }, { 1, 2, 3 }, { 1, 3 }, { 1, 4 }, { 2, 3 }, { 3, 4 }, { 2, 4 }, { 2, 3, 4 }
