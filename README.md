FIXED POINT ITERATION


Ivy Muthoni, Valma Mucera, Glen Ochieng

Fixed point iteration is a method of computing fixed points of a function
A fixed point of a function $f(x)$ is a point $x$ where $f(x) = x$.\newline
This is true only when $f(x)$ is continuous


    Applications
 Fixed point iteration has multiple applications in iterative methods including:
 Newton's method, reframed as a fixed point iteration
 This is what we will apply in code
 Halley's method\newline
 This is similar to Newton's method but used for functions with one real variable with a continuous second derivative
 Runge Kutta methods and numerical ordinary diferrential equation solvers
       
      As root finder
Finding the roots of an equation

    Algorithm
    
   Identify the function $f(x)$
        Find points a and b such that$ a < b$ where $f(a)<0$ and $f(b)>0$
        Select $x_0$(initial guess) by getting average of a and b: $$x_0 = \frac{a + b}{2}$$
        Define function $g(x)$ which is obtained from $f(x) = 0$ such that $x = g(x)$ and
        $\left\lvert g\prime(x)  < 1\right\rvert$
  

     Finding the roots of an equation
   
  Calculate $x_1$ such that $$x_1 = g(x_0) , x_2 = g(x_1), x_3 ... x_n$$.
  Repeat the above till$$f(x_i) - f(x_{i-1}) = 0$$
  The root will be at $x_n$.
  
     Sample equations
  
   $x^3 - x - 1$
   
   
   $x^3-2x-5$
   
   
   $x^4-2x^3-5x-2$
    
   
