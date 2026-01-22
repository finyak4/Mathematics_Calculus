# Section 3 — Calculus: Exercises

## Limits of Sequences

### Ex 1.

Calculate the limit of sequences:

**1)**

$$
u_n = \frac{n}{n+1}
$$

**Solution:**
Divide num and den by $n$.

$$
\lim \frac{1}{1+1/n} = \frac{1}{1+0} = 1
$$

**2)**

$$
u_n = \frac{4n-3}{6-5n}
$$

**Solution:**
Divide by $n$.

$$
\lim \frac{4-3/n}{6/n-5} = \frac{4}{-5} = -0.8
$$

**3)**

$$
u_n = \frac{n^2-1}{3-n^3}
$$

**Solution:**
Degree of denominator ($n^3$) is higher. Limit is $0$.

**4)**

$$
u_n = \frac{2n^3-4n-1}{6n+3n^2-n^3}
$$

**Solution:**
Coefficients of highest power ($n^3$) are $2$ and $-1$.
Limit is $2/(-1) = -2$.

**5)**

$$
u_n = \frac{(n-1)(n+3)}{3n^2+5}
$$

**Solution:**
Numerator $\approx n^2$, Denom $\approx 3n^2$. Limit is $1/3$.

**6)**

$$
u_n = \frac{(2n-1)^2}{(4n-1)(3n+2)}
$$

**Solution:**
Num $\approx 4n^2$, Denom $\approx 12n^2$. Limit is $4/12 = 1/3$.

**7)**

$$
u_n = \frac{(2n-1)^3}{(4n-1)^2(1-5n)}
$$

**Solution:**
Num $\approx 8n^3$, Denom $\approx 16n^2 \cdot (-5n) = -80n^3$. Limit is $8/(-80) = -0.1$.

**8)**

$$
u_n = \frac{3}{n} - \frac{10}{\sqrt{n}}
$$

**Solution:**
Both terms go to 0. Limit is $0$.

**9)**

$$
u_n = \frac{(-1)^n}{2n-1}
$$

**Solution:**
Bounded numerator / infinite denominator $\to 0$.

**10)**

$$
u_n = \left(\frac{2n-3}{3n+1}\right)^2
$$

**Solution:**
Base limit is $2/3$. Sq is $(2/3)^2 = 4/9$.

**11)**

$$
u_n = \left(\frac{5n-2}{3n-1}\right)^3
$$

**Solution:**
Base limit $5/3$. cubed is $125/27$.

**12)**

$$
u_n = \frac{(\sqrt{n}+3)^2}{n+1}
$$

**Solution:**
Num $\approx n$. Denom $\approx n$. Ratio of coeffs $1/1 = 1$.

**13)**

$$
u_n = \frac{\sqrt{n}-2}{3n+5}
$$

**Solution:**
Power $1/2$ vs $1$. Limit is $0$.

**14)**

$$
u_n = \frac{n-10}{3}
$$

**Solution:**
$\infty$.

**15)**

$$
u_n = \frac{(-0.8)^n}{2n-5}
$$

**Solution:**
Exponential with base $<1$ goes to 0 faster than $n$. Numerator $\to 0$. Limit is $0$.

...

**25)**

$$
u_n = \sqrt{n+2}-\sqrt{n}
$$

**Solution:**
Multiply by conjugate:

$$
\frac{n+2-n}{\sqrt{n+2}+\sqrt{n}} = \frac{2}{\approx 2\sqrt{n}} \to 0
$$

**26)**

$$
u_n = \sqrt{n^2+n}-n
$$

**Solution:**
Conj:

$$
\frac{n^2+n-n^2}{\sqrt{n^2+n}+n} = \frac{n}{n(\sqrt{1+1/n}+1)} \to \frac{1}{2}
$$

**27)**

$$
u_n = n-\sqrt{n^2+5n}
$$

**Solution:**
Conj:

$$
\frac{n^2-(n^2+5n)}{n+\sqrt{n^2+5n}} = \frac{-5n}{2n} \to -2.5
$$

...

**38)**

$$
u_n = \sqrt[n]{3^n+2^n}
$$

**Solution:**
Factor $3^n$:

$$
3 \sqrt[n]{1+(2/3)^n} \to 3 \cdot 1 = 3
$$

**42)**

$$
u_n = \frac{1+2+...+n}{n^2}
$$

**Solution:**
Sum is $\frac{n(n+1)}{2}$. Limit is:

$$
\frac{n^2}{2n^2} = 1/2
$$

## Limits of Functions

### Ex 1.

Calculate limits:

**1)**

$$
\lim\limits_{x \to 3} \frac{27-x^3}{x-3}
$$

**Solution:**

$$
\frac{(3-x)(9+3x+x^2)}{-(3-x)} \cdot (-1) = -(9+9+9) = -27
$$

**2)**

$$
\lim\limits_{x \to 3} \frac{x^2-4x+3}{2x-6}
$$

**Solution:**

$$
\frac{(x-3)(x-1)}{2(x-3)} = \frac{x-1}{2} \to \frac{2}{2} = 1
$$

...

**15)**

$$
\lim\limits_{x \to 0} \frac{\sin 3x}{4x}
$$

**Solution:**

$$
\frac{3}{4} \frac{\sin 3x}{3x} \to 3/4
$$

**16)**

$$
\lim\limits_{x \to 0} \frac{4x}{3 \sin 2x}
$$

**Solution:**

$$
\frac{4}{3} \frac{1}{2} \frac{2x}{\sin 2x} \to 2/3
$$

**17)**

$$
\lim\limits_{x \to +\infty} \frac{\sin x}{x}
$$

**Solution:**
Bounded/Infinity = $0$.

## Derivatives of Functions

### Ex 1.

Calculate derivatives:

**1)**

$$
y = \frac{1}{3}x^3 - \frac{3}{2}x^4 + \frac{13}{5}x^5 - 2x^6
$$

**Solution:**

$$
y' = x^2 - 6x^3 + 13x^4 - 12x^5
$$

**2)**

$$
y = 5x^{15} - x^2 + \frac{1}{3}x - 2
$$

**Solution:**

$$
y' = 75x^{14} - 2x + \frac{1}{3}
$$

**3)**

$$
y = ax^3 + \frac{b}{x} + c
$$

**Solution:**

$$
y' = 3ax^2 - \frac{b}{x^2}
$$

**7)**

$$
y = \sqrt[3]{x^2} = x^{2/3}
$$

**Solution:**

$$
y' = \frac{2}{3}x^{-1/3} = \frac{2}{3\sqrt[3]{x}}
$$

**20)**

$$
y = \frac{8x^3}{x^3+x-1}
$$

**Solution:**
Quotient rule.
$u = 8x^3, v = x^3+x-1$.
$u' = 24x^2, v' = 3x^2+1$.

$$
y' = \frac{24x^2(x^3+x-1) - 8x^3(3x^2+1)}{(x^3+x-1)^2} = \frac{16x^3-24x^2}{(x^3+x-1)^2}
$$

**52)**

$$
z = 2x+\sin 2x
$$

**Solution:**

$$
z' = 2 + 2\cos 2x
$$

**65)**

$$
y = e^{ax}(a\sin x - \cos x)
$$

**Solution:**
Product rule.

$$
y' = ae^{ax}(a\sin x - \cos x) + e^{ax}(a\cos x + \sin x) = e^{ax}(a^2+1)\sin x
$$

## Integrals

### Ex 1.

Calculate integrals:

**1)**

$$
\int \frac{x\sqrt{x} - x\sqrt[4]{x}}{\sqrt[3]{x}} dx
$$

**Solution:**
Convert to powers: $\frac{x^{1.5} - x^{1.25}}{x^{1/3}} = x^{3/2 - 1/3} - x^{5/4 - 1/3} = x^{7/6} - x^{11/12}$.

$$
\int x^{7/6} dx - \int x^{11/12} dx = \frac{6}{13}x^{13/6} - \frac{12}{23}x^{23/12} + C
$$

**5)**

$$
\int \frac{dx}{\sqrt{3x+1}}
$$

**Solution:**
Subst $u=3x+1, du=3dx$.

$$
\frac{1}{3} \int u^{-1/2} du = \frac{1}{3} \cdot 2u^{1/2} = \frac{2}{3}\sqrt{3x+1} + C
$$

**14)**

$$
\int x e^{-x^2} dx
$$

**Solution:**
$u = -x^2, du = -2x dx$.

$$
-\frac{1}{2} \int e^u du = -\frac{1}{2}e^{-x^2} + C
$$

**41)**

$$
\int x \cos x dx
$$

**Solution:**
Integration by parts. $u=x, dv=\cos x dx$. $du=dx, v=\sin x$.

$$
x \sin x - \int \sin x dx = x \sin x + \cos x + C
$$

**81)**

$$
\int \frac{x^4}{x^2+1} dx
$$

**Solution:**
Polynomial division. $x^4 = (x^2+1)(x^2-1) + 1$.

$$
\int (x^2 - 1 + \frac{1}{x^2+1}) dx = \frac{x^3}{3} - x + \operatorname{arctg} x + C
$$

**115)**

$$
\int \sin^3 x dx
$$

**Solution:**
$\int \sin x (1-\cos^2 x) dx$. $u=\cos x$.

$$
-\int (1-u^2) du = -u + \frac{u^3}{3} = -\cos x + \frac{1}{3}\cos^3 x + C
$$
