Practical 5:

Mathematical Expectation and Variance- 
a. Mean of discrete and continuous Probability distribution 
b. S.D. and variance of discrete and continuous Probability distribution 

mean(1:6)
mean(sample(1:6, 
           10000, 
           replace = T))
var(1:6)
f <- function(x) 3 / x^4
g <- function(x) x * f(x)
h <- function(x) x^2 * f(x)
area <- integrate(f, 
                 lower = 1, 
                 upper = Inf)
EX <- integrate(g,
                lower = 1,
                upper = Inf)
EX
VarX <- integrate(h,
                  lower = 1,
                  upper = Inf)
VarX
