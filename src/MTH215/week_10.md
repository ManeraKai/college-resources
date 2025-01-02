# Week 10

Chapters:
- [Handbook of Differential Equations](https://annas-archive.org/md5/49f513e7bc62370eae64309c5d3309e7)
    - 95 Variation of Parameters
    - 61 Euler Equations

Videos:
- [Dr. Trefor Bazett: Variation of Parameters](https://youtube.com/watch?v=wSMad7QpaqE)
- [The Organic Chemistry Tutor: Cramer's Rule](https://youtube.com/watch?v=vXqlIOX2itM)
- [Dr. Trefor Bazett: Linear Independence of Functions & The Wronskian](https://youtube.com/watch?v=4z5aL3aGVQs)
- [Dr. Trefor Bazett: The Theory of Higher Order Differential Equations](https://youtube.com/watch?v=7vwDp94wEhg)
<!---->
- [blackpenredpen: Variation of Parameters](https://youtube.com/watch?v=BaK4Mkn1k1Y)
- [blackpenredpen:  solving the differential equation \\(y''+y=tan(t)\\) by variation of parameters](https://youtube.com/watch?v=H8DH7KwcuUQ)
<!---->
- [Houston Math Prep: Cauchy-Euler Differential Equations (2nd Order Homogeneous)](https://www.youtube.com/watch?v=ep7xoctAlEY)
- [Houston Math Prep: Cauchy-Euler Differential Equations (2nd Order Non-Homogeneous)](https://www.youtube.com/watch?v=KTx6KXcJwSA)

### Confusion about Variation of Parameters
There's a lot of confusion about how to solve those. Some solve it using Crammer's Rule, some using the Wronksian.

2nd Order Ordinary Differential Equation:

$$
y′′+by′+cy=f(x)
$$

We know that to make a general solution, we would take the sum of a Complementary/Homogeneous Solution and a Particular Solution:

$$
y = y_h + y_p
$$

You first find the Homogeneous Solution \\(y_h\\), which will be
$$
y_h = c_1y_1+c_2y_2
$$

You take \\(y_1\\) and \\(y_2\\) and construct an assumed form of a particular solution
$$
y_p = u_1y_1 + u_2y_2
$$

Where \\(u_1\\) and \\(u_2\\) are functions of x. Technically you can also write them as \\(u_1(x)\\) and \\(u_2(x)\\). This structure is just an assumption. Just like what we did with the method of undetermined coefficients.

After this, you try to take the first and second derivatives of \\(y_p\\).
$$
y_p' = u_1'y_1 + u_1y_1' + u_2'y_2 + u_2y_2'
$$

To try to find a solution, we add a constraint

$$
u_1'y_1 + u_2'y_2 = 0
$$

This will limit our solution, but at the same time, it may give us a solution. Better than nothing.

Our new first derivative of the particular solution becomes

$$
y_p' = u_1y_1' + u_2y_2'
$$

We take the second derivative

$$
y_p'' = u_1'y_1' + u_1y_1'' + u_2'y_2' + u_2y_2''
$$

Now, we put \\(y_p\\), \\(y_p'\\), and \\(y_p''\\) into our original differential equation

$$
\big(u_1'y_1' + u_1y_1'' + u_2'y_2' + u_2y_2''\big) + b\big(u_1y_1' + u_2y_2'\big) + c\big(u_1y_1 + u_2y_2\big)=f(x)
$$

This can be simplified to (watch [blackpenredpen: Variation of Parameters](https://youtube.com/watch?v=BaK4Mkn1k1Y))
$$
u_1(\underbrace{y_1''+by_1'+cy_1}\\_{y_h = 0}) + u_2(\underbrace{y_2''+by_2'+cy_2}\\_{y_h = 0}) + u_1'y_1' + u_2'y_2' = f(x)
$$

$$
u_1'y_1' + u_2'y_2' = f(x)
$$

Now, we have two equations
$$
\begin{split}
u_1'y_1' + u_2'y_2' & = f(x) \\\\
u_1'y_1 + u_2'y_2 & = 0
\end{split}
$$

We know \\(y_1\\), \\(y_1'\\), \\(y_2\\), \\(y_2'\\), and \\(f(x)\\). The only two unknowns are \\(u_1'\\) and \\(u_2'\\). This is a system of 2 equations and 2 unknowns.

You can solve this system of equations using normal algebra, but you can also use Linear Algebra. In particular, you can use Crammer's 2x2 Matrix Rule.

#### Crammer's Rule
Crammer's Rule in our context is (for general context, watch [The Organic Chemistry Tutor: Cramer's Rule](https://youtube.com/watch?v=vXqlIOX2itM))
$$
\begin{align}
u_1' = \frac{D_{u_1'}}{D} \newline \newline
u_2' = \frac{D_{u_2'}}{D}
\end{align}
$$
Where \\(D\\), \\(D_{u_1'}\\), and \\(D_{u_2'}\\) are
$$
\begin{split}
D & = \begin{vmatrix} y_1 & y_2 \\\\ y_1' & y_2' \end{vmatrix} \space & = y_1y_2'-y_2y_1' \\\\\\\\\\
D_{u_1'} & = \begin{vmatrix} 0 & y_2 \\\\ f(x) & y_2' \end{vmatrix} \space & = -y_2f(x) \\\\\\\\\\
D_{u_2'} & = \begin{vmatrix} y_1 & 0 \\\\ y_1' & f(x) \end{vmatrix} \space & = y_1f(x)
\end{split}
$$
Let's substitute our \\(D\\)'s
$$
\begin{align}
u_1' = \frac{-y_2f(x)}{y_1y_2'-y_2y_1'} \newline \newline
u_2' = \frac{y_1f(x)}{y_1y_2'-y_2y_1'}
\end{align}
$$

Then, you take their integral to find \\(u_1\\) and \\(u_2\\)
$$
\begin{align}
u_1 = \int{\frac{-y_2f(x)}{y_1y_2'-y_2y_1'}} \newline \newline
u_2 = \int{\frac{y_1f(x)}{y_1y_2'-y_2y_1'}}
\end{align}
$$

You can now add them to your particular solution
$$
y_p = \int{\frac{-y_2f(x)}{y_1y_2'-y_2y_1'}dx}y_1 + \int{\frac{y_1f(x)}{y_1y_2'-y_2y_1'}dx}y_2
$$

Now, you have a Homogeneous and a Particular solution, you can now construct your general solution
$$
y = \big( c_1y_1+c_2y_2 \big) + \bigg(\int{\frac{-y_2f(x)}{y_1y_2'-y_2y_1'}dx}y_1 + \int{\frac{y_1f(x)}{y_1y_2'-y_2y_1'}dx}y_2 \bigg)
$$

#### Wronksian method
You only have two formulae that you need to memorize
$$
\begin{align}
u_1 = \int{\frac{-y_2f(x)}{W(y_1, y_2)}dx} \newline \newline
u_2 = \int{\frac{y_1f(x)}{W(y_1, y_2)}dx}
\end{align}
$$
Where \\(W(y_1, y_2)\\) is the [Wronksian](https://en.wikipedia.org/wiki/Wronskian) of \\(y_1\\) and \\(y_2\\), which is
$$
W(y_1, y_2) = \begin{vmatrix} y_1 & y_2 \\\\ y_1' & y_2' \end{vmatrix}  = y_1y_2'-y_2y_1'
$$
You may notice that this is the exact same as \\(D\\) in Crammer's Rule, and you would be correct.

Those two methods are basically the same.

For why we write Wronksian: [Dr. Trefor Bazett: Variation of Parameters, 8:14](https://youtube.com/watch?v=wSMad7QpaqE&t=493)

As a myself note, Even if we assumed that \\(y_1\\) and \\(y_2\\) are linearly independent, according to the Wronksian definition, they still can be equal to zero at some points. They satisfy being linearly independent if they were at least non-zero at one point, even if all the other points are zero.
