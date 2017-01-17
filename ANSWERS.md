# In Class Assignment \#3

The code written for this assignment can be found in `ica_03_ranta.ipynb`. The function that was found to break all root-finding methods (i.e. bisection, Secant, and Brent's) was f(x) = |x|^(1/3), when 
the interval given was -2 to 1. The reason this broke the bisection and Brent's methods was because the interval had the same sign value at both endpoints, making it seem like there was no root to be 
found within that interval. For the Newton/Secant method, this function broke the method because the derivate was discontinuous across the interval. In general, the bisection method is the most robust 
and, provided a proper interval is given, will always find a root of the function in a given interval; however, it make take a longer computation time to reach the solution. The Newton/Secant method 
works reasonably well AS LONG AS the function has a continuous, non-ocsillatory derivatives (or, in general, "well-behaved derivatives"). Brent's method should work in all cases as well provided that a 
proper interval is given (i.e. where the function's value at the endpoints are of different sign values).

Overall, the bisection method (and the Brent's method) is the most robust and "effectively unbreakable", as long as it is implemented properly.
