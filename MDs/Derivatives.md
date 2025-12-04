**CLASS NOTES: INTRO TO DERIVATIVES**

Topic: *The Power Rule & Basic Differentiation*

Subject: Calculus I

**I. DEFINITION OF A DERIVATIVE**

*Formal Definition (Limit Definition)*

The fundamental mathematical definition of a derivative is based on limits:

$$f'(x) = \lim_{h \to 0} \frac{f(x+h) - f(x)}{h}$$

Concept: The derivative measures the instantaneous rate of change of a function.

Geometrically: It is the slope of the tangent line to the curve at a specific point $(x)$.

Notation:

Lagrange: $f'(x)$ or $y'$

Leibniz: $\frac{dy}{dx}$ or $\frac{d}{dx}[f(x)]$

**II. THE POWER RULE (Shortcut for $x^n$)**

Instead of using the limit definition $\lim_{h \to 0}$, we use the Power Rule for polynomials.

The Formula

$$\frac{d}{dx}(x^n) = n \cdot x^{n-1}$$

Steps

Bring the exponent ($n$) down to the front (multiply).

Subtract $1$ from the exponent.

**III. EXAMPLES**

*A. Basic Polynomials*

Rule: Multiply coeff by power, drop power by 1.

Example 1: $f(x) = x^4$

$$f'(x) = 4x^{4-1} = \mathbf{4x^3}$$

Example 2: $y = 5x^3$

$$y' = 5 \cdot (3x^2) = \mathbf{15x^2}$$

*B. Special Cases (Constants & Linear)*

Constant Rule: Derivative of a constant number is 0.

$$y = 7 \rightarrow y' = 0 \quad \text{(Horizontal line has slope 0)}$$

Linear Rule: Derivative of $x$ is 1.

$$y = x \rightarrow y' = 1$$

$$y = 8x \rightarrow y' = 8$$

*C. Rewriting Required (Negatives & Fractions)*

Tip: Always rewrite the function as $x^n$ before deriving.

1. Negative Exponents (Fractions)

Problem: $f(x) = \frac{1}{x^3}$

Rewrite: $f(x) = x^{-3}$

Differentiate:

$$f'(x) = -3x^{-3-1} = -3x^{-4}$$

Simplify: $f'(x) = \mathbf{-\frac{3}{x^4}}$

2. Rational Exponents (Roots)

Problem: $y = \sqrt{x}$

Rewrite: $y = x^{1/2}$

Differentiate:

$$y' = \frac{1}{2}x^{1/2 - 1} = \frac{1}{2}x^{-1/2}$$

Simplify: $y' = \mathbf{\frac{1}{2\sqrt{x}}}$

**IV. SUM AND DIFFERENCE RULE**

If you have multiple terms, take the derivative of each one separately.

Example:

$$f(x) = 2x^5 - 4x^3 + 7x - 10$$

$$f'(x) = \underbrace{10x^4}_{2\cdot5} - \underbrace{12x^2}_{4\cdot3} + \underbrace{7}_{7\cdot1} - \underbrace{0}_{const}$$

Final Answer:

$$f'(x) = 10x^4 - 12x^2 + 7$$

**V. KEY TAKEAWAYS / CHEAT SHEET**

$\frac{d}{dx}(c) = 0$ (Constants disappear)

$\frac{d}{dx}(cx) = c$ (Linear terms leave just the coefficient)

$\frac{d}{dx}(x^n) = nx^{n-1}$ (Power Rule)

Rewrite roots as fractions ($\sqrt{x} \to x^{1/2}$)

Rewrite denominators as negative powers ($\frac{1}{x} \to x^{-1}$)

**VI. MIXED PRACTICE EXAMPLES**

Here are some slightly harder problems combining the rules above.

1. Polynomial with Fraction Coefficients

$$y = \frac{1}{3}x^6 - x^2 + \pi$$

Step 1: Apply Power Rule. Note that $\pi$ is just a number (constant).

$$y' = \frac{1}{3}(6x^5) - 2x + 0$$

Answer: $\mathbf{y' = 2x^5 - 2x}$

2. Expansion First

$$f(x) = x(x^2 + 4)$$

Step 1: Distribute the $x$ first. (It's easier than using Product Rule later).
Rewrite: $f(x) = x^3 + 4x$

Step 2: Differentiate.

Answer: $\mathbf{f'(x) = 3x^2 + 4}$

3. Complex Rewrite

$$g(x) = \frac{3}{x^2} - 2\sqrt[3]{x}$$

Step 1: Rewrite as powers.

$$g(x) = 3x^{-2} - 2x^{1/3}$$

Step 2: Power Rule.

$$g'(x) = 3(-2x^{-3}) - 2(\frac{1}{3}x^{-2/3})$$

$$g'(x) = -6x^{-3} - \frac{2}{3}x^{-2/3}$$

Answer: $\mathbf{g'(x) = -\frac{6}{x^3} - \frac{2}{3\sqrt[3]{x^2}}}$