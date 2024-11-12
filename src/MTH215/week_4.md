# Week 4

Chapters ([Fundamentals of Differential Equations](https://annas-archive.org/md5/56a244ea4a50552e7ba39a4f16bd0d2c)):
- 2.6 Substitutions and Transformations
    - Bernoulli Equations

Videos:
- Bernoulli Differential Equations
    - [Professor Leonard: How to Solve Bernoulli Differential Equations](https://www.youtube.com/watch?v=NjIMGAIPbzg&list=PLDesaqWTN6ESPaHy2QUKVaXNZuQNxkYQ_)

### Ricatti Differential Equations:
Because you are still learning the fundementals of Differential Equations, you will be given a hint to solve Ricatti, a particular solution. Using it, you can find the general solution by a simple substitution. Ricatti then becomes a Linear Differential Equation.
#### Example, use the particular solution \\( y_1 = \frac{-1}{x} \\) to find the general solution of \\( x^2(\frac{dy}{dx}+y^2) = 2 \\)
#### Solution
Always use the formula \\( y = y_1 + \frac{1}{u} \\), then differentiate \\( y \\) with respect to \\( x \\)
$$ y = \frac{-1}{x} + \frac{1}{u} \qquad  \frac{dy}{dx} = \frac{1}{x^2} - \frac{1}{u^2} \cdot \frac{du}{dx} $$
Then solve
$$ x^2 \left[ \Big(\frac{1}{x^2} - \frac{1}{u^2} \cdot \frac{du}{dx} \Big) + \Big( \frac{-1}{x} + \frac{1}{u} \Big)^2 \right] = 2 $$
After simplifying, you'll get
$$ \frac{du}{dx} + \frac{2}{x}u = 1 $$
Which is a Linear Differential Equation.