# CLASS NOTES: APPLICATIONS OF DERIVATIVES
 
**Topic:** Extrema, MVT, Concavity & Derivative Tests
 
## I. Minimum and Maximum Values
 
### Definitions
 
*   **Absolute (Global) Maximum:** The highest point on the *entire* domain. $f(c) \ge f(x)$ for all $x$.
*   **Absolute (Global) Minimum:** The lowest point on the *entire* domain. $f(c) \le f(x)$ for all $x$.
*   **Local (Relative) Maximum:** A high point in a *nearby neighborhood* (peak of a hill).
*   **Local (Relative) Minimum:** A low point in a *nearby neighborhood* (bottom of a valley).
 
### The Extreme Value Theorem (EVT)
 
If $f$ is **continuous** on a closed interval $[a, b]$, then $f$ attains an **absolute maximum** value $f(c)$ and an **absolute minimum** value $f(d)$ at some numbers $c$ and $d$ in $[a, b]$.
 
**Method: Finding Absolute Extrema on $[a, b]$**
 
1.  Find the critical numbers of $f$ in $(a, b)$.
2.  Evaluate $f$ at the critical numbers.
3.  Evaluate $f$ at the endpoints ($a$ and $b$).
4.  Compare values: Largest is Max, Smallest is Min.
 
### Example
 
**Problem:** Find the absolute max and min of $f(x) = x^3 - 3x + 1$ on $[0, 3]$.
 
**1. Find Critical Points:**
 
$$f'(x) = 3x^2 - 3$$
 
$$3(x^2 - 1) = 0 \Rightarrow x = \pm 1$$
 
Only $x = 1$ is in the interval $[0, 3]$.
 
**2. Evaluate at Critical Point:**
 
$$f(1) = 1 - 3 + 1 = -1$$
 
**3. Evaluate at Endpoints:**
 
$$f(0) = 1$$
 
$$f(3) = 27 - 9 + 1 = 19$$
 
**4. Compare:**
 
Values are: $-1, 1, 19$.
 
*   **Absolute Max:** $19$ at $x=3$.
*   **Absolute Min:** $-1$ at $x=1$.
 
---
 
## II. The Mean Value Theorem (MVT)
 
### The Theorem
 
If $f$ satisfies two hypotheses:

1.  $f$ is **continuous** on the closed interval $[a, b]$.
2.  $f$ is **differentiable** on the open interval $(a, b)$.
 
Then there is a number $c$ in $(a, b)$ such that:
 
$$f'(c) = \frac{f(b) - f(a)}{b - a}$$
 
OR
 
$$f(b) - f(a) = f'(c)(b - a)$$
 
**Meaning:** There is at least one point where the tangent slope equals the secant (average) slope.
 
### Example
 
**Problem:** Find $c$ satisfying MVT for $f(x) = x^2$ on $[0, 2]$.
 
**1. Find Average Slope:**
 
$$\frac{f(2) - f(0)}{2 - 0} = \frac{4 - 0}{2} = 2$$
 
**2. Set $f'(c)$ equal to Average Slope:**
 
$$f'(x) = 2x \Rightarrow f'(c) = 2c$$
 
$$2c = 2 \Rightarrow c = 1$$
 
**3. Check Interval:** $1$ is in $(0, 2)$.
 
**Answer:** $c = 1$.
 
---
 
## III. First Derivative Test
 
Used to find **Local Extrema**.
 
**Steps:**

1.  Find Critical Numbers $c$.
2.  Use a sign chart to check the sign of $f'$ on intervals around $c$.
 
**The Test:**

*   $f'$ changes $(+) \to (-)$ $\Rightarrow$ **Local Max**.
*   $f'$ changes $(-) \to (+)$ $\Rightarrow$ **Local Min**.
*   No sign change $\Rightarrow$ **No Local Extremum**.
 
### Example
 
**Problem:** Find local extrema for $f(x) = x^3 - 3x^2$.
 
**1. Critical Points:**
 
$$f'(x) = 3x^2 - 6x = 3x(x-2)$$
 
CPs: $x=0, x=2$.
 
**2. Sign Chart:**
 
*   $x < 0$ (Test -1): $f'(-1) = 3(-1)(-3) = (+)$ $\nearrow$
*   $0 < x < 2$ (Test 1): $f'(1) = 3(1)(-1) = (-)$ $\searrow$
*   $x > 2$ (Test 3): $f'(3) = 3(3)(1) = (+)$ $\nearrow$
 
**3. Conclusion:**
 
*   **Local Max** at $x=0$ ($f$ goes Up then Down).
*   **Local Min** at $x=2$ ($f$ goes Down then Up).
 
---
 
## IV. Concavity & The Second Derivative Test
 
### Concavity
 
*   **Concave Up:** $f''(x) > 0$ (Holds water $\cup$).
*   **Concave Down:** $f''(x) < 0$ (Spills water $\cap$).
 
**Inflection Point:** Where concavity changes.
 
### Example
 
**Problem:** Find intervals of concavity and inflection points for $f(x) = x^4 - 4x^3$.
 
**1. Find $f''(x)$:**
 
$$f'(x) = 4x^3 - 12x^2$$
 
$$f''(x) = 12x^2 - 24x = 12x(x-2)$$
 
**2. Sign Chart for $f''$:**
CPs for $f''$: $x=0, x=2$.
 
*   $x < 0$ (Test -1): $f''(-1) = (-)(-) = (+)$ **Concave Up**.
*   $0 < x < 2$ (Test 1): $f''(1) = (+)(-) = (-)$ **Concave Down**.
*   $x > 2$ (Test 3): $f''(3) = (+)(+) = (+)$ **Concave Up**.
 
**3. Inflection Points:**
 
*   At $x=0$ and $x=2$ because concavity changes.
 
### Second Derivative Test
 
An alternative method for **Local Extrema**.
 
*   $f'(c) = 0$ and **$f''(c) > 0$** $\Rightarrow$ **Local Min** (Concave Up).
*   $f'(c) = 0$ and **$f''(c) < 0$** $\Rightarrow$ **Local Max** (Concave Down).
*   $f''(c) = 0$ $\Rightarrow$ **Inconclusive** (Use 1st Derivative Test).
