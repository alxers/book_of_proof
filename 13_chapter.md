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
