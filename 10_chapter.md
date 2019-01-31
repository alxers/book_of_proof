Mathematical Induction.     

Outline for Proof by Induction.     
Proposition The statements S_1, S_2, S_3, ... are all true.     

Proof. (Induction)     
(1) Prove that the first statement S_1 is true.     
(2) Given any integer k >= 1, prove that the statement S_k => S_k+1 is true.     
It follows by mathematical induction that every S_n is true.     


Example:     
Proposition. If n in N, then 1+3+5+7+...+(2n-1) = n^2.     
Proof.     
(1) Observe that if n = 1, this statement is 1 = 1^2, which is true.     
(2) We must prove S_k => S_k+1 for any k >= 1.     
That is if 1+3+5+7+...+(2k - 1) = k^2, then 1+3+5+7+...+(2(k+1) - 1) = (k + 1)^2.     
Direct proof. Suppose 1+3+5+7+...+(2k - 1) = k^2.     
Then 1 + 3 + 5 + 7 + ... + (2 (k + 1) - 1) =       
1 + 3 + 5 + 7 + ... + (2k - 1) + (2 (k + 1) - 1) =     
(1 + 3 + 5 + 7 + ... + (2k - 1)) + (2 (k + 1) - 1) =      
k^2 + (2 (k + 1) - 1) = k^2 + 2k + 1 = (k + 1)^2      
This proves that S_k => S_k+1.     
It follows by induction that 1 + 3 + 5 + 7 + ... + (2n - 1) = n^2 for every n in N.     


Proposition If n is a non-negative integer, then 5 | (n^2 - n).     
Basis step:
(1) If n = 0, 0 = 5x.    
(2)
