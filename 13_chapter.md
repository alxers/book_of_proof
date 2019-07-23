Proofs in Calculus (3rd edition)      


Exercises for Section 13.2      

.2. Prove that lim(x-> - 1)(4x + 6) = 2.      
|4x + 6 - 2| = 4|x + 1|.      
let delta = epsilon/4, then 0 < |x - (-1)| < delta      
|4x + 6 - 2| = 4|x + 1| < 4delta = 4 * epsilon/4 = epsilon      
For all epsilon > 0 exists such delta = epsilon/4 such that 0 < |x + 1| < delta implies |4x + 6 - 2| < epsilon.      


.4. Prove that lim(x -> 8)(2x - 7) = 9.      
|2x - 16| = 2|x - 8|      
let delta = epsilon/2, then 0 < |x - 8| < delta      
|2x - 7 - 9| = 2|x - 8| < 2delta = 2 * epsilon/2 = epsilon      
For all epsilon > 0, exists such delta > 0, such that 0 < |x - 8| < 2delta, |2x - 7 - 9| < epsilon.       


.6. Prove that lim(x -> 1)(4x^2 + 1) = 5.       
|4x^2 + 1 - 5| = 4|x^2 - 1| = 4|(x - 1)(x + 1)|      
When x is small, x - 1 is close to 1, x + 1 close to 2.      
If |x - 1| <= 1, then |x + 1| = |(x - 1) + 2| <= |x - 1| + |2| <= 1 + 2 = 3.     
So if |x - 1| <= 1, then |x + 1| <= 3      
Then |f(x) - L| = |4x^2 + 1 - 5| = |x - 1||x + 1| < 4|x - 1|     
Take delta to be smaller then both 1 and epsilon/3      
Then 0 < |x - 1| < delta implies |4x^2 + 1| < 4|x - 1| < 3delta < 3 * epsilon/3 = epsilon.      



Exercises for Section 13.3       
Prove that the following limits do not exits.      

.2. lim(x -> 0)(|x|/x).      
Suppose for the sake of contradiction that lim(x -> 0)(|x|/x) = L.      
Let epsilon = 1, so there is delta > 0, for which 0 < |x - 0| < delta implies ||x|/x - L| < 1.       
Choose x that is smaller then delta and |x|/(1 + L).      
Then 0 < |x - 0| < delta, so ||x|/x - L| < epsilon      
Also x < |x|/(1 + L), 1 < |x|/x(1 + L), 1 + L < |x|/x, 1 < |x|/x - L      
We get ||x|/x - L| < 1 and 1 < ||x|/x - L|. Contradiction.      


.4. lim(x -> pi/2)cos(1/x).       
Suppose for the sake of contradiction that lim(x -> pi/2)cos(1/x) = L.       
Let epsilon = 1/4.      
Then there is a delta > 0, for which 0 < |x - 0| < delta implies |cos(1/x) - L| < 1/4     
Select k in N large enough so that 1/kpi < delta      
As 0 < |1/kpi - pi/2| < delta, we have |cos(1/1/kpi) - L| < 1/4      
|cos(kpi - pi/2) - L| = |sin(kpi) - L| = |0 - L| = |L| < 1/4       
Now take l in N large enough so that 1/2lpi < delta.       
Then 0 < |1/2lpi - 0| < delta      
So we have |cos(1/1/2lpi) - L| < 1/4      
|cos(2lpi) - L| = |1 - L| < 1/4      
Above showed |L| < 1/4 and |1 - L| < 1/4     
1 = |L + (1 - L)| <= |L| + |1 - L| < 1/4 + 1/4 = 1/2      
1 < 1/2 - contradiction.       



Exercises for Section 13.4      

.2. Given two or more functions f_1, f_2, ..., f_n, suppose that lim(x->c)f_i(x) exists for each 1 <= i <= n. Prove that lim(x->c)(f_1(x)f_2(x)...f_n(x)) = (lim(x->c)f_1) * (lim(x->c)f_2) * ... * (lim(x->c)f_n).      
a) Base case, let n = 1, then lim(x->c)f_1 = lim(x->c)f_1.      
b) Let n = k+1, then lim(x->c)(f_1(x)f_2(x)...f_k+1(x) = lim(x->c)(f_1(x)f_2(x)...) * f_k+1(x)) = lim(x->c)(f_1(x)f_2(x)...f_k(x)) * lim(x->c)f_k+1(x) = lim(x->c)f_1(x) * lim(x->c)f_2(x) ... * lim(x->c)f_k+1(x).       


.4.
