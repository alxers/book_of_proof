Counting

A list is an ordered sequence of objects.
(a, b, c, d, e) != (b, a, c, d, e)

A list is somewhat like a set, but set is unordered
{ a, b, c, d, e } = { b, a, c, d, e }

It's often needed to count up the number of possible lists that satisfy some condition or property.
F.e. we need to make a list of length three such that the first entry must be in { a, b, c }, the second must be in { 5, 7 }, and the third must be in { a, x }.

How many such lists are there? 3 * 2 * 2 = 12 (multiplication principle)

The total number of different lists that can be made is the product a_1 * a_2 * a_3 ... a_n

There are two types of list-counting problems.
1. Repetition allowed.
2. Repetition is not allowed.

Example 3.2 Consider making lists from symbols A, B, C, D, E, F, G
(a) How many length-4 lists are possible if repetition is allowed?
(b) How many length-4 lists are possible if repetition is not allowed?
(c) How many length-4 lists are possible if repetition is not allowed and list must contain an E?
(d) How many length-4 lists are possible if repetition is allowed and list must contain an E?

Solutions:
(a) Image the list as containing four boxes filled with selections from letters A, B, C, D, E, F, G

( _ , _ , _ , _ )
  7   7   7   7  choices

7^4 = 2401

(b)

( _ , _ , _ , _ )
  7   6   5   4

7 * 6 * 5 * 4 = 840

(c)

( _ , _ , _ , _ )
  E   6   5   4

( _ , _ , _ , _ )
  6   E   5   4

( _ , _ , _ , _ )
  6   5   E   4

( _ , _ , _ , _ )
  6   5   4   E

(6 * 5 * 4) * 4 = 480

(d)

Wrong method:

( _ , _ , _ , _ )
  E   7   7   7

( _ , _ , _ , _ )
  7   E   7   7

( _ , _ , _ , _ )
  7   7   E   7

( _ , _ , _ , _ )
  7   7   7   E

7^3 * 4 = 1372

This is not correct, because f.e. list (E, E, A, B) counted multiple times

The correct way to solve this problem is to count all possible lists (like in (a)), then subtract all lists which do not contain an E.

1) All possible lists 7^4 = 2401
2) All lists without E: 6^4 = 1296
3) 2401 - 1296 = 1105
