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


.4. Prove that if f(x)/g(x) is a rational function (polynomial divided by a polynomial), and g(c) != 0, then lim(x->c)(f(x)/g(x)) = f(c)/g(c).      
f(x) = a_0 + a_1x^1 + a_2x^2 + ... + a_nx^n.     
g(x) = a_0 + a_1x^1 + a_2x^2 + ... + a_nx^n.     
lim(x->c)(f(x)/g(x)) = lim(x->c)f(x)/lim(x->c)g(x) = (lim(x->c)a_0 + lim(x->c)a_1x^1 +...+ lim(x->c)a_nx^n)/(lim(x->c)b_0 + lim(x->c)b_1x^1 +...+ lim(x->c)b_nx^n) = (a_0 + a_1c^1 + a_2c^2 + ... + a_nc^n)/(a_0 + a_1c^1 + a_2c^2 + ... + a_nc^n) = f(c)/g(c)



Exercises for Section 13.6      
Prove the following.     

.2. lim(x->inf)(3x + 2)/(2x - 1) = 3/2.     
For epsilon > 0, exists such N = 1/(epsilon - 3/2), such that x > N, then x > 1/(epsilon - 3/2).       
(epsilon - 3/2)x > 1      
epsilon - 3/2 > 1/x     
epsilon > 1/x + 3/2     
epsilon > 2/2x + 3/2     
epsilon > (3x + 2)/2x     
epsilon > (3x + 2)/(2x - 1)     
So |(3x + 2)/(2x - 1) - 0| < epsilon.       


.6. If both lim(x->inf)f(x) and lim(x->inf)g(x) exist, then lim(x->inf)f(x)g(x) = (lim(x->inf)f(x))(lim(x->inf)g(x)).      
Let lim(x->inf)f(x) = L, lim(x->inf)g(x) = M.       
Take epsilon > 0. We need to find N for which x > N => |(f(x)g(x)) - LM| < epsilon.     
Notice that |(f(x)g(x)) - LM| = |(f(x)g(x) - Lg(x)) + (Lg(x) - LM)| = |g(x)(f(x) - L) + L(g(x) - M)| <= |g(x)||f(x) - L| + |L||g(x) - M| (A).      
Now g(x) = |g(x) - M + M| <= |g(x) - M| + |M| < 1 + |M| (because lim(x->inf)g(x) exists => |g(x) - M| < epsilon, when epsilon = 1 f.e.)      
Because lim(x->inf)f(x) = L, exists such N' > 0 : x > N' => |f(x) - L| < epsilon/(2(1 + |M|))     
Because lim(x->inf)g(x) = M, exists such N'' > 0 : x > N'' => |g(x) - L| < epsilon/(2|L|)      
Then substitute in (A) gives:      
|g(x)||f(x) - L| + |L||g(x) - M| < (1 + |M|) * epsilon/(2(1 + |M|)) + |L| * epsilon/(2|L|) = epsilon/2 + epsilon/2 = epsilon.      


.8. If both lim(x->inf)f(x) and lim(x->inf)g(x) exist, and lim(x->inf)g(x) != 0, then lim(x->inf)(f(x)/g(x)) = lim(x->inf)f(x)/lim(x->inf)g(x).        
Notice that |f(x)/g(x) - L/M| = |(Mf(x) - Lg(x)))/(Mg(x))| = |((Mf(x) - LM) - (Lg(x) - LM))/(Mg(x))| = |(M(f(x) - L) - L(g(x) - M))/(Mg(x))| <= |(f(x) - L)/(g(x))| + |(L(g(x) - M))/(Mg(x))| = |1/g(x)||f(x) - L| + |L/(Mg(x))||g(x) - M| (A)       
Because lim(x->inf)g(x) exsts, |g(x) - M| < epsilon, epsilon = |M|/2.      
Then |g(x)| = |g(x) - M + M| >= |M| - |g(x) - M| > |M| - |M|/2 = |M|/2.       
|g(x)| > |M|/2 => 1/g(x) < 2/|M|.     
Replace in (A)        
|f(x)/g(x) - L/M| < 2/|M||f(x) - L| + 2L/|M^2||g(x) - M|.       
Case 1, suppose L != 0.       
Choose N' > 0, so x > N' => |f(x) - L| < epsilon|M|/4.      
Choose N'' > 0, so x > N'' => |g(x) - L| < epsilon|M^2|/4|L|.      
N = max{ N', N'' }, then        
|f(x)/g(x) - L/M| < 2/|M|epsilon|M|/4 + 2|L|/|M^2|epsilon|M^2|/4|L| = epsilon/2 + epsilon/2 = epsilon.      
Case 2, suppose L = 0.       
Choose N''' > 0, x > N''' => |f(x) - L| < epsilon|M|/2.       
|f(x)/g(x) - L/M| < 2/|M|epsilon|M|/2 = epsilon.      



.10. Prove that lim(x->inf)sin(x) does not exist.        
Suppose lim(x->inf)sin(x) = L, then for all epsioln > 0, exists such N > 0 : x > N => |sin(x) - L| < epsilon.       
|sin(x) - L| <= |1 - L|        
Let epsilon = 1.      
We can choose x = 3pi/2 and x' = pi/2 for which sin(x) = 1 or -1.       
Then |1 - L| < 1 and |-1 - L| < 1.      
-1 < 1 - L < 1 and -1 < -1 - L < 1      
-2 < -L < 0 and 0 < -L < 2, contradiction.      


Exercises for Section 13.7      

.4. Prove that { 1 - 1/2^n } converges to 1.      
Suppose epsilon > 0. Choose an int N > 1/(epsilon * ln2).     
1/2^N < epsilon, 1 < epsilon * 2^N, 1/epsilon < 2^N.      
e^(ln(1/epsilon)) < e^(Nln(2))
1/2^N < epsilon
|1 - 1/2^n - 1| = |-1/2^n| = 1/2^n < 1/2^N < epsilon      



.6. Prove that { (5n^2 + n + 1)/(4n^2 + 2) } converges to 5/4.      
For all epsilon > 0, exist such N > 0 : x > N = > |(5n^2 + n + 1)/(4n^2 + 2) - 5/4| < epsilon.     
|(5n^2 + n + 1)/(4n^2 + 2) - 5/4| = |(4(5n^2 + n + 1) - 5(4n^2 + 2))/4(4n^2 + 2)| = |(20n^2 + 4n + 4 - 20n^2 - 10)/4(4n^2 + 2)| = |(4n - 6)/(4(4n^2 + 2))| = |(2n - 3)/(2(4n^2 + 2))| < epsilon.     
Observe that (2n - 3)/(2(4n^2 + 2)) < (2n - 3)/(8n^2) < 2n/8n^2.       
Let 2n/8n^2 < epsilon, then 1/4^n > 1/epsilon       
4n > 1/epsilon, n > 1/4epsilon      
Therefore, given any epsilon > 0, take an int N > 1/4epsilon. If n > N then      
|(5n^2 + n + 1)/(4n^2 + 2) - 5/4| = (2n - 3)/(2(4n^2 + 2)) < 1/4N < 1/4(1/4epsilon) = epsilon.     
By definition 13.5 it converges to 5/4.     
