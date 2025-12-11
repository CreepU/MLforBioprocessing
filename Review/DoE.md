# Design of Experiments

Design of Experiments (DOE) is a systematic, statistical approach to planning, conducting, and analyzing controlled tests to understand how multiple input variables (factors) affect an output variable (response).

### Screening

DOE screening is a critical first step in a Design of Experiments (DOE) process, used to efficiently identify the most important input variables (factors) affecting a process from a large pool of potential factors, using fewer experimental runs than a full factorial design.

According to this formula, we absorb the high dimensional effects into the error term $\epsilon$, ex. $x_1^2,x1*x2$. In this step, we assume this model is linear in all parameters. However, this is not the case in reality; therefore, this method only provides an approximation for selecting the most influential parameters.

$y=\beta_0+\sum_{i=0}^k\beta_ix_i+\epsilon$

y: Response
$\beta$: main effect coefficient
x: coding parameter
$\epsilon$: error

In this [Orthognal](Orthogonal.md) design we use 1 or -1 to represent the real world value of parameters. For example, we set two values for pH. Low value is 6.9, which is -1 and High value is 7.3, which is +1. 

For n experiments, k parameters, $\vec{y}=X\vec{\beta}+\vec{\epsilon}$, and we can use [Least Square](LeastSquare.md) to get the result. 

From least square, the result is $\vec{\beta}=\frac{1}{n}X^T\vec{y}$. For every parameter like $\beta_n(n=1,2,...)$, so $\beta_i=\frac{1}{n}\sum x_{r_i}y_r$

And we define main effect as $Effect_i = \bar{y}(x_i=+1)-\bar{y}(x_i=-1)=\frac{2}{n}\sum x_{r_i}*y_r=2\beta_i$.

#### Full Factorial

