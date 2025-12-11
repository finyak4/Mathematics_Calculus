# CLASS NOTES: DERIVATIVE RULES & TRIGONOMETRY

**Topic:** Product, Quotient, Chain Rules & Trig
**Subject:** Calculus I

## I. Product Rule

Used when two functions are **multiplied** together: $f(x) \cdot g(x)$.

### The Formula

$$(f \cdot g)' = f'g + fg'$$

**Memorize:** "Derivative of the first times the second, PLUS the first times the derivative of the second."

### Example

$$y = (x^3)(2x + 5)$$

*   $f = x^3 \rightarrow f' = 3x^2$
*   $g = 2x + 5 \rightarrow g' = 2$

$$y' = (3x^2)(2x+5) + (x^3)(2)$$

Simplify:

$$y' = 6x^3 + 15x^2 + 2x^3$$

$$y' = \mathbf{8x^3 + 15x^2}$$

---

## II. Quotient Rule

Used when two functions are **divided**: $\frac{f(x)}{g(x)}$.

### The Formula

$$\left(\frac{f}{g}\right)' = \frac{f'g - fg'}{g^2}$$

**Memorize (Rhyme):**
> "Lo d-Hi minus Hi d-Lo, draw the line and square the Lo."
> *   **Lo:** Bottom function ($g$)
> *   **Hi:** Top function ($f$)
> *   **d-:** Derivative of...

### Example

$$y = \frac{5x^2}{3x + 1}$$

*   $Hi = 5x^2 \rightarrow dHi = 10x$
*   $Lo = 3x+1 \rightarrow dLo = 3$

$$y' = \frac{(3x+1)(10x) - (5x^2)(3)}{(3x+1)^2}$$

Simplify Numerator:

$$y' = \frac{30x^2 + 10x - 15x^2}{(3x+1)^2}$$

$$y' = \mathbf{\frac{15x^2 + 10x}{(3x+1)^2}}$$

*(Usually, you don't need to expand the denominator)*

---

## III. Trigonometric Derivatives

You must memorize these 6 rules.

**The Main Two:**

1.  $\frac{d}{dx}(\sin x) = \cos x$
2.  $\frac{d}{dx}(\cos x) = -\sin x$

**The Other Four:**

3.  $\frac{d}{dx}(\tan x) = \sec^2 x$
4.  $\frac{d}{dx}(\cot x) = -\csc^2 x$
5.  $\frac{d}{dx}(\sec x) = \sec x \tan x$
6.  $\frac{d}{dx}(\csc x) = -\csc x \cot x$

**Pattern Tip:** Derivatives of "Co-" functions (Cosine, Cotangent, Cosecant) always begin with a **Negative** sign.

---

## IV. The Chain Rule

Used for **composite** functions (functions inside functions): $f(g(x))$.

### The Formula

$$\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$$

**Concept:** "Derivative of the OUTSIDE (keep inside same) $\times$ Derivative of the INSIDE."

### Steps

1.  Identify the **Outside** function and the **Inside** function.
2.  Apply Power Rule (or other rule) to the Outside.
3.  Multiply by the derivative of the Inside.

### Example 1 (Power Chain)

$$y = (3x^2 + 1)^7$$

*   Outside: $(\dots)^7$
*   Inside: $3x^2 + 1$

$$y' = 7(3x^2 + 1)^{7-1} \cdot \frac{d}{dx}(3x^2+1)$$

$$y' = 7(3x^2 + 1)^6 \cdot (6x)$$

$$y' = \mathbf{42x(3x^2 + 1)^6}$$

### Example 2 (Trig Chain)

$$y = \sin(4x)$$

*   Outside: $\sin(\dots)$
*   Inside: $4x$

$$y' = \cos(4x) \cdot \frac{d}{dx}(4x)$$

$$y' = \mathbf{4\cos(4x)}$$

---

## V. Key Takeaways / Cheat Sheet

*   **Product:** $f'g + fg'$
*   **Quotient:** $\frac{Lo \cdot dHi - Hi \cdot dLo}{Lo^2}$
*   **Chain:** Out' $\cdot$ In'
*   **Trig Signs:** "Co" implies Negative.

---

## VI. Mixed Practice Examples

**1. Chain Rule with Division (Rewriting)**

$$f(x) = \frac{1}{(2x-3)^4}$$

Rewrite first to avoid Quotient Rule:

$$f(x) = (2x-3)^{-4}$$

Apply Chain Rule:

$$f'(x) = -4(2x-3)^{-5} \cdot (2)$$

$$f'(x) = -8(2x-3)^{-5}$$

Answer: $\mathbf{f'(x) = \frac{-8}{(2x-3)^5}}$

**2. Product Rule + trig**

$$y = x^2 \sin x$$

*   $f = x^2 \rightarrow f' = 2x$
*   $g = \sin x \rightarrow g' = \cos x$

Apply $f'g + fg'$:

$$y' = (2x)(\sin x) + (x^2)(\cos x)$$

Answer: $\mathbf{y' = 2x\sin x + x^2\cos x}$