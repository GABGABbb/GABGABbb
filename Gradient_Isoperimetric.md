# Gabriel-Singer
We are interested here in the numerical side of the isoperimetric problem for polygons. We deal with the particular case of the triangle, the quadrilateral, and the pentagon. 
The codes are written in Python and available in the file "Python_Isoperimetric_Gradient_Descent.md".

The main theoretical result is:

Theorem :

   Let $n\geq 1$ and $Z$ a polygon with $n$ sides, we have 
    $$\frac{P(Z)^{2}}{V(Z)} \geqslant 4n\tan{\frac{\pi}{n}}.$$
     With equality if and only if $Z$ is a regular polygon.
     $P$ denotes the perimeter and $V$ the aera.
     
Proof of this theorem can be found in "V.Blasjo The Isoperimetric Problem,
The American Mathematical Monthly, 112:6, 526-566."

We know by the previous theorem that for $Z$ a polygon with $n$ sides, we have the following inequality : 

$$\frac{P(Z)^{2}}{V(Z)}\geq 4n\tan{\frac{\pi}{n}}:=m_{\star}(n)$$

Proposition:

If we denote $d$ the number of variables in the function we are trying to minimize and $I$ the number of iterations. 
Then,
    The complexity of the gradient descent algorithm is $$O\left(d*I\right).$$
The proof is very standard.
