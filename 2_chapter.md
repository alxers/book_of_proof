Logic

*Statement.*
A statement is a sentence or a mathematical expression that is either definitely true or definitely false.

Exercises for Section 2.1

Decide wheter or not the following are "statements". If it's a statement, say if it's true or false.

1. Every real number is an even integer. 
False statement.

2. Every even integer is a real number.
True statement.

3. If x an y are real numbers and 5x = 5y, then x = y.
True statement.

4. Sets Z and N.
Not a statement.

5. Sets Z and N are infinite.
True statement.

6. Some sets are finite.
True statement.

7. The derivative of any polynomial of degree 5 is a polynomial of degree 6.
False statement.

8. N not_in P(N).
False statement.

9. cos(x) = -1
Not a statement, open statement (we don't know x)

10. (R x N) intersection (N x R) = N x N.
Statement

11. The integer x is a multiple of 7.
Not a statement.

12. If the integer x is a multiple of 7, then it is divisible by 7.
True statement.

13. Either x is a multiple of 7, or it's not.
True statement.


Exercises for Section 2.2

Express each statement or open sentence in one of the forms P ^ Q, P v Q, or ~ P

1. The number 8 is both even and a power of 2.
P: number 8 is even
Q: number 8 is a power of 2

P ^ Q

2. The matrix A is not invertible.
P: the matrix A is invertible

~ P

3. x != y
P: x = y

~ P

4. x < y
P: x < y

P

5. y >= x
P: y > x
Q: y = x

P v Q

6. There is a quiz scheduled for Wednesday or Friday.
P: Quiz is scheduled for Wednesday
Q: Quiz is scheduled for Friday

P v Q

7. The number x equals zero, but the number y does not.
P: number x equals to zero
Q: number y equals to zero

P ^ (~ Q)

8. A least one of the numbers x and y equals to 0.
P: number x equals to zero
Q: number y equals to zero

P v Q

9. x in A - B

10. x in A intersection B

11. A in { X in P(N) : |X(complement)| < inf }


Exercises for Section 2.3

Without changing their meanings, convert each of the following sentences into a sentence having for form "If P, then Q"

1. A matrix is irrevertible provided that its determinant is not zero.
If determinant is not zero then a matrix is irrevertible.

2. For a function to be continuous, it is sufficient that it is differentiable.
If function is differentiable, then it's continuous.

3. For a function to be integrable, it is necessary that it is continuous.
If function is continuous, then it's integrable.

4. A function is rational if it is a polynomial.
If function is polynomial, then it is rational.

5. An integer is divisible by 8 only if it is divisible by 4.
If intiger divisible by 8, then it's divisible by 4.

6. Whenever a surface has only one side, it is non-orientable.
If surface has only one side, then it's non-orientable.

7. A series converges whenever it converges absolutely.
If series converges, then it's converges absolutely.

8. A geometric series with ratio r converges if |r| < 1.
If |r| < 1, then geometric series converges.

9. A function is integrable provided the function is continuous.
If function is integrable, then it's continuous.

10. The discriminant is negative only if the quadratic equation has no real solutions.
If quadratic equation has no real solutions, then the discriminant is negative.

11. You fail only if you stop writing. (Ray Bradbury)
If you stop writing, then you will fail.

12. People will generally accept facts as truth only if the facts agreee with what they already believe. (Andy Rooney)
If facts agree with what people already believe, then they will accept them.

13. Whenever people agree with me I feel I must be wrong. (Oscar Wilde)
If people agree with me, then I feel I'm wrong.

Exercises for Section 2.4
Without changing their meanings, convert each of the following sentences into a
sentence having the form "P if and only if Q."

1. For matrix A to be invertible, it is necessary and sufficient that det(A) != 0.
Matrix A is invertible if and only if det(A) != 0.

2. If a function has a constant derivative then it's linear, and conversely.
Function has a constant derivative if and only if it linear.
Function is linear if and only if it has a constant derivative. 

3. If xy = 0 then x = 0 or y = 0, and conversely.
xy = 0 if and only if x = 0 or y = 0 

4. If a in Q then 5a in Q, and if 5a in Q then a in Q.
?

5. For an occurrence to become an adventure, it is necessary and sufficient for
one to recount it. (Jean-Paul Sartre).
An occurence is an adventure if and only if one recount it.


Exercises for Section 2.5
Write a truth table the logial statements:

1. P or (Q => R)
T or (T => T) T
T or (T => F) T
T or (F => T) T
T or (F => F) T
F or (T => T) T
F or (T => F) T
F or (F => T) F
F or (F => F) F

2. (Q or R) <=> (R and Q)
(T or T) <=> (T and T) T
(T or F) <=> (F and T) F
(F or T) <=> (T and F) F
(F or F) <=> (F and F) T

3. ~(P => Q)
~(T => T) F
~(T => F) T
~(F => T) F
~(F => F) F

4. ~(P or Q) or (~P)
~(T or T) or (~T) F
~(T or F) or (~T) F
~(F or T) or (~F) F
~(F or F) or (~F) T

6. (P and ~P) and Q
(T and ~T) and T F
(T and ~T) and F F
(F and ~F) and T F
(T and ~T) and F F

9. ~(~P and ~Q)
~(~T and ~T) T
~(~T and ~F) T
~(~F and ~T) T
~(~F and ~F) F

10. Suppose the statement ((P and Q) or R) => (R or S) is false. Find the truth values of P, Q, R and S (can be done without truth table).
((P and Q) or R) must be false
P - false, R - false, Q - true, S - true

11. Suppose P is false and that the statement (R => S) <=> (P and Q) is true. Find the truth values of R and S.

If P is false then (P and Q) is also false
? <=> F evalates to true only when ? is false
(R => S) is false only if R is false and S is true



Exercises for Section 2.6

A. Use truth tables to show that the folowing statements are logcally equvalent.
1. P ^ (Q v R) = (P ^ Q) v (P ^ R)

P Q R
T T T | T ^ (T v T) = (T ^ Q) v (T ^ T) | T T
T T F | T ^ (T v F) = (T ^ T) v (T ^ F) | T T
T F T | T ^ (F v T) = (T ^ F) v (T ^ T) | T T
F T T | F ^ (T v T) = (F ^ T) v (F ^ T) | F F
T F F | T ^ (F v F) = (T ^ F) v (T ^ F) | F F
F F F | F ^ (F v F) = (F ^ F) v (F ^ F) | F F

3. P => Q = (~P) v Q

P Q
T T | T => T = ~T v T | T T
T F | T => F = ~T v F | F F
F T | F => T = ~F v T | T T
F F | F => F = ~F v F | T T

8. ~P <=> Q = (P => ~Q) ^ (~Q => P)

P Q
T T | F <=> T = (T => F) ^ (F => T) | F F
T F | F <=> F = (T => T) ^ (T => T) | T T
F T | T <=> T = (F => F) ^ (F => F) | T T
F F | T <=> F = (F => T) ^ (T => F) | F F

B. Decide whether or not the following pairs of statements are logically equivalent.

9. P ^ Q and ~(~P v ~Q)

P Q
T T | T ^ T and ~(~T v ~T) | T and T
T F | T ^ F and ~(~T v ~F) | F and F
F T | F ^ T and ~(~F v ~T) | F and F
F F | F ^ F and ~(~F v ~F) | F and F

10. (P => Q) v R and ~((P ^ ~Q) ^ ~R)

P Q R
T T T | (T => T) v T and ~((T ^ ~T) ^ ~T) | T and T
T T F | (T => T) v F and ~((T ^ ~T) ^ ~F) | T and T
T F T | (T => F) v T and ~((T ^ ~F) ^ ~T) | T and T
F T T | (F => T) v T and ~((F ^ ~T) ^ ~T) | T and T
T F F | (T => F) v F and ~((T ^ ~F) ^ ~F) | F and F
F F T | (F => F) v T and ~((F ^ ~F) ^ ~T) | T and T
F T F | (F => T) v F and ~((F ^ ~T) ^ ~F) | T and T
F F F | (F => F) v F and ~((F ^ ~F) ^ ~F) | T and T
