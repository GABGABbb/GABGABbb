# Gabriel-Singer
We are interested here in the numerical side of the isoperimetric problem for polygons. We deal with the particular case of the triangle, the quadrilateral and the pentagon. 
The codes are written in Python and available in the file "Python_Isoperimetric_Gradient_Descent.md".
The main result is:
\begin{theorem}
   Let $n\geq 1$ and $Z$ a polygon with $n$ sides, we have 
    $$\frac{P(Z)^{2}}{V(Z)} \geqslant 4n\tan{\frac{\pi}{n}}.$$
     With equality if and only if $Z$ is a regular polygon.
     $P$ denotes the perimeter and $V$ the aera
\end{theorem}
Proof of this theorem can be found in "V.Blasjo The Isoperimetric Problem,
The American Mathematical Monthly, 112:6, 526-566."

We know by previous theorem that for $Z$ a polygn with $n$ sides, we have the following inequality : 
$$\frac{P(Z)^{2}}{V(Z)}\geq 4n\tan{\frac{\pi}{n}}:=m_{\star}(n)$$

The complexity of the first algorithm is not too big.
begin{proposition}
If we denote $d$ the number of variables in the function we are trying to minimize and $I$ the number of iterations. 
Then,
    The complexity of the first algorithm is $$O\left(d*I\right).$$
\end{proposition}
\begin{proof}
For each iteration $k\in [1,I]$ of the for loop there are at most $d$ components of the gradient norm to check in the if loop, hence the formula.
\end{proof}
