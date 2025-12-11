# Newton Fractal

**Topic:** Visualizing Newton's Method
**Subject:** Calculus I / Numerical Methods

## What is Newton's Method?

Newton's method is an iterative technique used to approximate the roots (zeroes) of a real-valued function. It uses the tangent line of the function at the current point to estimate the next point.

**The Iterative Formula:**

$$
x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}
$$

**Where:**
*   $x_n$: The current guess for the root.
*   $x_{n+1}$: The next, better approximation.
*   $f(x_n)$: The function's value at $x_n$.
*   $f'(x_n)$: The derivative (slope) at $x_n$.

## Newton Fractals

When Newton's method is applied to complex functions $z \in \mathbb{C}$, the starting point $z_0$ determines which root the method converges to. The plane is divided into regions, or **basins of attraction**, corresponding to each root.

### The Boundary of Chaos

The boundary between these regions is often fractal. This means the pattern is infinitely complex and self-similar. Small changes in the starting position can cause the method to converge to a completely different root—a hallmark of **chaos** and sensitivity to initial conditions.

### Visualizations

#### 1. Detailed View: The Edge of Stability
![Fractal Zoom](./img/Screenshot%202025-12-11%20161417.png)


#### 2. Standard Newton Fractal: Basins of Attraction
![Newton Fractal](./img/newton_fractal.png)
*This image shows the entire set of basins for a polynomial. Each color represents the specific root that the method converges to. The fractal boundary is the set of initial points that fail to converge or lie on the "fence" between roots.*
