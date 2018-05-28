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

vowels A, E, I = 3
consonants B, C, D, F, G, H = 6

( _ , _ , _ , _ , _ , _ )
  3   2   7   6   5   4
  V   V

( _ , _ , _ , _ , _ , _ )
  7   3   2   6   5   4
      V   V

( _ , _ , _ , _ , _ , _ )
  7   6   3   2   5   4
          V   V

( _ , _ , _ , _ , _ , _ )
  7   6   5   3   2   4
              V   V

( _ , _ , _ , _ , _ , _ )
  7   6   5   4   3   2
                  V   V

(7 * 6 * 5 * 4 * 3 * 2) * 5 = 25200


12. Consider the lists of length six made with the symbols P, R, O, F, S, where repetition is allowed. (For example, the following is such a list: (P,R,O,O,F,S).)
How many such lists can be made if the list must end in an S and the symbol O is used more than once?


Exercises for Section 3.2
1. What is the smallest n for which n! has more than 10 digits?

13

2. For which values of n does n! have n or fewer digits?
1! = 1

3. How many 5-digit positive integers are there in which there are no repeated digits and all digits are odd?

odd digits - 1 3 5 7 9
_ _ _ _ _
5 4 3 2 1

5! = 120

6. There are two 0 ’s at the end of 10! = 3, 628, 800 . Using only pencil and paper,
determine how many 0 ’s are at the end of the number 100! .

7. Compute how many 9-digit numbers can be made from the digits 1, 2, 3, 4, 5, 6, 7, 8, 9
if repetition is not allowed and all the odd digits occur first (on the left) followed by all the even digits (i.e. as in 137598264 , but not 123456789 ).


Exercises for Section 3.3
1. Suppose a set A has 37 elements. How many subsets of A have 10 elements?
How many subsets have 30 elements? How many have 0 elements?

n = 37
k = 10

37! / (10! (37-10)!) = 37! / ( 10! 27! ) = 348 330 136
37! / (30! (37-30)!) = 37! / (30! 7!) = 10295472
37! / (0! (37-0)!) = 37! / 37! = 1

2. Suppose A is a set for which |A| = 100. How many subsets of A have 5 elements?
How many subsets have 10 elements? How many have 99 elements?

100! / (5! * 95!) = 75287520
100! / (10! * 90!) = 17310309456440
100! / (99! * 1!) = 100

3. A set X has exactly 56 subsets with 3 elements. What is the cardinality of X ?

|X| = a
a! / (3! (a - 3)!) = 56

6(a-3)! * 56 = a!
336(a-3)! = a!
336 = a!/(a-3)!

a! = a(a-1)!
(a-1)! = (a-1)(a-2)!
(a-2)! = (a-2)(a-3)!

a! = a(a-1)(a-2)(a-3)!

336 = a(a-1)(a-2)(a-3)! / (a-3)!
336 = a(a-1)(a-2)

a = 8

4. Suppose a set B has the property that |{X : X in P(B), |X| = 6 }| = 28. Find |B|.

x! / (6! * (x - 6)!) = 28
x = 8

5. How many 16-digit binary strings contain exactly seven 1’s? (Examples of such strings include 0111000011110000 and 0011001100110010 , etc.)

n = 16
k = 7

16! / (7! (16-7)!) = 11 440

6. |{ X in P({0, 1, 2, 3, 4, 5, 6, 7, 8, 9 }): |X| = 4 }| =

How many subsets of length 4 can be made of set of length 10

n = 10
k = 4

10! / (4! * (10-4)!) = 210

7. |{ X in P({0, 1, 2, 3, 4, 5, 6, 7, 8, 9 }): |X| < 4 }| =

Count X sets < 4, so they contain 0, 1, 2, 3 elements.
How many subsets of length 3 + how many subsets of length 2 + how many subsets of length 1 + 1 (for one empty subset)

10! / (3! * (10-3)!) +
10! / (2! * (10-2)!) +
10! / (1! * (10-1)!) + 1 = 176

8. This problem concerns lists made from the symbols A,B,C,D,E,F,G,H,I.

(a) How many length- 5 lists can be made if repetition is not allowed and the list is in alphabetical order? (Example: BDEFI or ABCGH, but not BACGH.)
(b) How many length- 5 lists can be made if repetition is not allowed and the list is not in alphabetical order?

(a) Total amount of 5 length lists made from A,B,C,D,E,F,G,H,I

_ , _ , _ , _ , _
9   8   7   6   5

9 * 8 * 7 * 6 * 5 = 15120

9!/(5!(9-5)!) = 126 ?


(b) if (a) is correct, then 15120 - 126 = 14994

9. This problem concerns lists of length 6 made from the letters A,B,C,D,E,F, without repetition. How many such lists have the property that the D occurs before the A?

D_ _ _ _ _
 5 4 3 2 1 = 4! * 5

_ D _ _ _ _
4   4 3 2 1 = 4! * 4

_ _ D _ _ _
4 3   3 2 1 = 4! * 3

_ _ _ D _ _
4 3 2   2 1 = 4! * 2

_ _ _ _ D _
4 3 2 1   1 = 4! * 1

4!(5+4+3+2+1) = 360


10. A department consists of 5 men and 7 women. From this department you select
a committee with 3 men and 2 women. In how many ways can you do this?

5   7
  +    = (5!/(3!2!)) + (7!/(2!5!)) = 31
3   2


11. How many positive 10-digit integers contain no 0's and exactly three 6's?

The amount of 6's in 10-digit integer 10!/(3!7!)
Multiplied by 8^7


Examples from chapter 3.3

Example 3.4

How many 4-element subsets does { 1, 2, 3, 4, 5, 6, 7, 8, 9 } have?
The answer is (9 4) = 9!/(4! * (9-4)!) = 126

Example 3.5 A single 5-card hand is dealt off of a standard 52-card deck.
How many different 5-card hands are possible?
To answer this, think of the deck as being a set D of 52 cards. Then a
5-card hand is just a 5-element subset of D.
52!/(5! * (52-5)!) = 2 598 960

Example 3.6 This problem concerns 5-card hands that can be dealt off of a 52-card deck. How many such hands are there in which two of the cards are clubs and three are hearts?

Solution: Think of such a hand as being described by a list of length
two of the form:
c - clubs
h - hearts
_ _  _ _ _
c c  h h h

where the first entry is a 2-element subset of the set of 13 club cards, and
the second entry is a 3-element subset of the set of 13 heart cards. There are
13!/(2! * 11!) choices for the first entry and 13!/(3! * 10!) for the second, so
by the multiplication principle there are 13!/(2! * 11!) * 13!/(3! * 10!) = 22 308


Exercises for Section 3.4

1. Write out Row 11 of Pascal’s triangle.
1th row - 0th power
2nd row - 1st power

8th row              1 7 21 35 35 21 7 1
9th row             1 8 28 56 70 56 28 8 1
10th row           1 9 36 84 126 126 84 36 9 1
11th row         1 10 45 120 210 252 210 120 45 10 1
12th row       1 11 55 165 330 462 462 330 165 55 11 1
13th row     1 12 66 220 495 792 924 792 495 220 66 12 1
14th row   1 13 78 286 715 1287 1716 1716 1287 715 286 78 13 1

2. Use the binomial theorem to find the coefficient of x^8 y^5 in (x+y)^13
14th row 1x^(13) 13x(12)y 78x(11)y^(2) 286x^(10)y^(3) 715x^(9)y^(4) 1287x^(8)y^(5) 1716 1716 1287 715 286 78 13 1
The coefficient is 1287

3. Use the binomial theorem to find the coefficient of x^8 in (x+2)^13
1287x^(8)2^(5)
The coefficient is 41184

4. Use the binomial theorem to find the coefficient of x^6 y^3 in (3x-2y)^9
 1x^(9) 9x^(8)y 36x^(7)y^(2) 84x^(6)y^(3) 126 126 84 36 9 1
 
 84(3x)^(6)(2y)^(3)
 -489888 

5. Use the binomial theorem to show Sigma from k=0 to n (n choose k) = 2^n
(k=0, n=0) = 2^0 = 1
(k=0, n=1) + (k=1, n=1) = 2^1 = 2
(k=0, n=2) + (k=2, n=1) + (k=2, n=2) = 2^2 = 4

6. Use Definition 3.2 (page 74) and Fact 1.3 (page 12) to show Sigma from k=0 to n (n choose k) = 2^n

Definition 3.2 If n and k are integers, then (n choose k) denotes the number of subsets that can be made by choosing k elements from a set with n elements.

Fact 1.3 If a finite set has n elements, then it has 2^n subsets.

If n and k are integers, then Sigma from k=0 to n is a finite set, then by fact 1.3 it has 2^n subsets (wrong)
* infinite number of integers, set if infinite integers can't be finite?

