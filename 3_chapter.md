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

Example 3.3 This problem involves making lists of length seven from the symbols 0, 1, 2, 3, 4, 5 and 6.
(a) How many such lists are there if repetition is not allowed?
(b) How many such lists are there if repetition is not allowed and the
first three entries must be odd?
(c) How many such lists are there in which repetition is allowed, and the list must contain at least one repeated number?

Solutions:
(a) 7! = 5040
(b) Set { 0, 1, 2, 3, 4, 5, 6 } contains three odd and four even numbers. First three 3! * other even 4!
3! * 4! = 144
(c) There are 7^7 = 823543 lists where repetition is allowed. And 7! = 5040 where repetition is not allowed.
7^7 - 7! = 818503 lists with at least one repetition (or more).

Exercises for Section 3.1

1. Consider lists made from the letters T,H,E,O,R,Y, with repetition allowed.
(a) How many length-4 lists are there?
(b) How many length-4 lists are there that begin with T ?
(c) How many length-4 lists are there that do not begin with T ?

(a) 6^4 = 1296
(b) 6^3 = 216 (?) check answer
(c) 1296 - 216 = 1080

2. Airports are identified with 3-letter codes. For example, the Richmond, Virginia airport has the code RIC, and Portland, Oregon has PDX. How many different
3-letter codes are possible?

( _ , _ , _ ) with repetition
  26  26  26

( _ , _ , _ ) without repetition
 26  25  24


 3. How many lists of length 3 can be made from the symbols A,B,C,D,E,F if

(a) repetition is allowed.
(b) repetition is not allowed.
(c) repetition is not allowed and the list must contain the letter A
(d) repetition is allowed and the list must contain the letter A

(a) 
( _ , _ , _ )
  6   6   6

6^3

(b)
( _ , _ , _ )
  6   5   4

6 * 5 * 4

(c)
( _ , _ , _ )
  A   5   4
( _ , _ , _ )
  5   A   4
( _ , _ , _ )
  5   4   A

5 * 4 * 3

(d)

All lists with rep. allowed = 6^3
Lists that do not contain 'A' = 5^3

6^3 - 5^3 = 91


4. Five cards are dealt off of a standard 52-card deck and lined up in a row. How
many such line-ups are there in which all 5 cards are of the same suit?

( _ , _ , _ , _ , _ )
  52  51  50  49  48

52 * 51 * 50 * 49 * 48 = all possible without rep.

there are 13 cards of the same suit

( _ , _ , _ , _ , _ )
  13  12  11  10  9

13 * 12 * 11 * 10 * 9 = 154440 ?

5. Five cards are dealt off of a standard 52-card deck and lined up in a row. How
many such line-ups are there in which all 5 cards are of the same color (i.e.,
all black or all red)?

There are 26 black and 26 red cards

( _ , _ , _ , _ , _ )
  26  25  24  23  22

6. Five cards are dealt off of a standard 52-card deck and lined up in a row. How many such line-ups are there in which exactly one of the 5 cards is a queen?

There are 4 queens in a deck

( _ , _ , _ , _ , _ )
  Q   48  47  46  45

(48 * 47 * 46 * 45) * 4 = 18_679_680


7. This problem involves 8-digit binary strings such as 10011011 or 00001010
(i.e., 8-digit numbers composed of 0’s and 1’s).
(a) How many such strings are there?
(b) How many such strings end in 0?
(c) How many such strings have the property that their second and fourth digits are 1’s?
(d) How many such strings have the property that their second or fourth digits are 1’s?

(a)

( _ , _ , _ , _ , _ , _ , _ , _ )
  2   2   2   2   2   2   2   2 

2^8 = 256

(b)

2^7 = 128

(c)

( _ , _ , _ , _ , _ , _ , _ , _ )
  2   1   2   1   2   2   2   2

2^6 = 64

(d)

2^7 ?

8. This problem concerns lists made from the symbols A,B,C,D,E.
(a) How many such length-5 lists have at least one letter repeated?
(b) How many such length-6 lists have at least one letter repeated?

<!-- (a)

( _ , _ , _ , _ , _ )
  5   5   5   5   1

5^4 = 625

(b)

( _ , _ , _ , _ , _ , _ )
  5   5   5   5   5   1

5^5 = 3125 -->

not correct?

(a)

5^5 the amount of lists with repetition allowed
5! the amount of lists with no repetition

5^5 - 5! = 3005 with at least one letter repeated

(b)

6^6 - 6! = 45936

9. This problem concerns 4-letter codes made from the letters A,B,C,D,...,Z.
(a) How many such codes can be made?
(b) How many such codes have no two consecutive letters the same?

(a)

( _ , _ , _ , _ )
  26  26  26  26

26^4 = 456976

(b)

Either:

( _ , _ , _ , _ )
  1  26  26  26

or

( _ , _ , _ , _ )
  26  1  26  26

or

( _ , _ , _ , _ )
  26  26  1  26

or 

( _ , _ , _ , _ )
  26  26  26  1

26^3 * 4 = 70304


10. This problem concerns lists made from the letters A,B,C,D,E,F,G,H,I,J.
(a) How many length-5 lists can be made from these letters if repetition is not allowed and the list must begin with a vowel?
(b) How many length-5 lists can be made from these letters if repetition is not allowed and the list must begin and end with a vowel?
(c) How many length-5 lists can be made from these letters if repetition is not allowed and the list must contain exactly one A?

vowels A, E, I = 3
consonants B, C, D, F, G, H, J = 7

(a)

( _ , _ , _ , _ , _ )
  3   9   8   7   6    (2+7=9)

(b)

( _ , _ , _ , _ , _ )
  3   8   7   6   2

(c)

( _ , _ , _ , _ , _ )
  1   9   8   7   6


11. This problem concerns lists of length 6 made from the letters A,B,C,D,E,F,G,H.
How many such lists are possible if repetition is not allowed and the list contains two consecutive vowels?

( _ , _ , _ , _ , _ , _ )
  V   V

?


12. Consider the lists of length six made with the symbols P, R, O, F, S, where repetition is allowed. (For example, the following is such a list: (P,R,O,O,F,S).)
How many such lists can be made if the list must end in an S and the symbol O is used more than once?