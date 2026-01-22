# Section 1 — Linear Algebra: Exercises

## Matrices and Basic Operations

### Ex 1.

For matrices

$$
A=\begin{pmatrix}1 & 2\\ 3 & 4\end{pmatrix} \quad \text{and} \quad B=\begin{pmatrix}0 & -1\\ 2 & 1\end{pmatrix}
$$

calculate:

- $A+B$
- $A-B$
- $2A$
- $3B-2A$
- $A\cdot B$
- Check if $A\cdot B = B\cdot A$.

**Solution:**

*   **$A+B$**:
    Add corresponding elements:
    
    $$
    A+B = \begin{pmatrix}1+0 & 2+(-1)\\ 3+2 & 4+1\end{pmatrix} = \begin{pmatrix}1 & 1\\ 5 & 5\end{pmatrix}
    $$

*   **$A-B$**:
    Subtract corresponding elements:
    
    $$
    A-B = \begin{pmatrix}1-0 & 2-(-1)\\ 3-2 & 4-1\end{pmatrix} = \begin{pmatrix}1 & 3\\ 1 & 3\end{pmatrix}
    $$

*   **$2A$**:
    Multiply every element of $A$ by 2:
    
    $$
    2A = \begin{pmatrix}1\cdot2 & 2\cdot2\\ 3\cdot2 & 4\cdot2\end{pmatrix} = \begin{pmatrix}2 & 4\\ 6 & 8\end{pmatrix}
    $$

*   **$3B-2A$**:
    Calculate $3B$ and subtract $2A$:
    
    $$
    3B = \begin{pmatrix}0 & -3\\ 6 & 3\end{pmatrix}
    $$
    
    $$
    3B - 2A = \begin{pmatrix}0 & -3\\ 6 & 3\end{pmatrix} - \begin{pmatrix}2 & 4\\ 6 & 8\end{pmatrix} = \begin{pmatrix}-2 & -7\\ 0 & -5\end{pmatrix}
    $$

*   **$A\cdot B$**:
    Matrix multiplication (row by column):
    
    $$
    A\cdot B = \begin{pmatrix}1\cdot0 + 2\cdot2 & 1\cdot(-1) + 2\cdot1\\ 3\cdot0 + 4\cdot2 & 3\cdot(-1) + 4\cdot1\end{pmatrix} = \begin{pmatrix}4 & 1\\ 8 & 1\end{pmatrix}
    $$

*   **Check commutativity ($B\cdot A$)**:
    
    $$
    B\cdot A = \begin{pmatrix}0\cdot1 + (-1)\cdot3 & 0\cdot2 + (-1)\cdot4\\ 2\cdot1 + 1\cdot3 & 2\cdot2 + 1\cdot4\end{pmatrix} = \begin{pmatrix}-3 & -4\\ 5 & 8\end{pmatrix}
    $$
    
    Since $\begin{pmatrix}4 & 1\\ 8 & 1\end{pmatrix} \neq \begin{pmatrix}-3 & -4\\ 5 & 8\end{pmatrix}$, **$A\cdot B \neq B\cdot A$**.

### Ex 2.

For matrices

$$
A=\begin{pmatrix}1 & 0\\ 0 & 2\end{pmatrix}, \quad B =\begin{pmatrix}2 & 0\\ 0 & 4\end{pmatrix}, \quad C=\begin{pmatrix}4 & 0\\ 0 & 8\end{pmatrix}, \quad D=\begin{pmatrix}8 & 0\\ 0 & 16\end{pmatrix}
$$

check if

$$
A\cdot B\cdot C\cdot D = B\cdot A\cdot D\cdot C = D\cdot C\cdot B\cdot A.
$$

**Solution:**
All these matrices are **diagonal matrices**. Diagonal matrices commute with each other.
Let's verify the product:

$$
A = \operatorname{diag}(1, 2), \quad B = \operatorname{diag}(2, 4), \quad C = \operatorname{diag}(4, 8), \quad D = \operatorname{diag}(8, 16)
$$

The product of diagonal matrices is a diagonal matrix containing the products of diagonal elements.
Element $(1,1)$: $1 \cdot 2 \cdot 4 \cdot 8 = 64$
Element $(2,2)$: $2 \cdot 4 \cdot 8 \cdot 16 = 1024$

Since multiplication of scalars is commutative ($a\cdot b = b\cdot a$), the order of matrix multiplication for diagonal matrices does not matter.
Thus, **Yes**, the equality holds.

### Ex 3.

Given matrix

$$
C=\begin{pmatrix}1 & 0 & 2\\ -1 & 3 & 1\\ 0 & 2 & -1\end{pmatrix}.
$$

Determine the matrix obtained by rearranging rows: swap the 1st and 3rd row, then add twice the new 1st row to the 2nd row. Write down all steps.

**Solution:**

*   **Step 1: Swap Row 1 ($R_1$) and Row 3 ($R_3$)**:
    
    $$
    R_1 \leftrightarrow R_3 \implies \begin{pmatrix}0 & 2 & -1\\ -1 & 3 & 1\\ 1 & 0 & 2\end{pmatrix}
    $$

*   **Step 2: Add $2 \times$ (new $R_1$) to $R_2$**:
    $R_2' = R_2 + 2R_1$.
    Row 1 is $(0, 2, -1)$.
    Row 2 is $(-1, 3, 1)$.
    calculation:
    $(-1) + 2(0) = -1$
    $3 + 2(2) = 7$
    $1 + 2(-1) = -1$
    
    Resulting matrix:
    
    $$
    \begin{pmatrix}0 & 2 & -1\\ -1 & 7 & -1\\ 1 & 0 & 2\end{pmatrix}
    $$

### Ex 4.

For column vectors $u=(1,-2,3)^{\top}$ and $v=(2,0,-1)^{\top}$, write them as matrices and calculate $u+v$, $u-v$, and matrix products $u\,v^{\top}$ and $v\,u^{\top}$. What is the rank of matrix $u\,v^{\top}$?

**Solution:**

*   **Vectors**:
    
    $$
    u = \begin{pmatrix}1 \\ -2 \\ 3\end{pmatrix}, \quad v = \begin{pmatrix}2 \\ 0 \\ -1\end{pmatrix}
    $$

*   **$u+v$**:
    
    $$
    \begin{pmatrix}1+2 \\ -2+0 \\ 3-1\end{pmatrix} = \begin{pmatrix}3 \\ -2 \\ 2\end{pmatrix}
    $$
    
*   **$u-v$**:
    
    $$
    \begin{pmatrix}1-2 \\ -2-0 \\ 3-(-1)\end{pmatrix} = \begin{pmatrix}-1 \\ -2 \\ 4\end{pmatrix}
    $$
    
*   **$u\,v^{\top}$ (Outer product)**:
    
    $$
    \begin{pmatrix}1 \\ -2 \\ 3\end{pmatrix} \begin{pmatrix}2 & 0 & -1\end{pmatrix} = \begin{pmatrix}1\cdot2 & 1\cdot0 & 1\cdot(-1) \\ -2\cdot2 & -2\cdot0 & -2\cdot(-1) \\ 3\cdot2 & 3\cdot0 & 3\cdot(-1)\end{pmatrix} = \begin{pmatrix}2 & 0 & -1 \\ -4 & 0 & 2 \\ 6 & 0 & -3\end{pmatrix}
    $$
    
*   **$v\,u^{\top}$**:
    
    $$
    \begin{pmatrix}2 \\ 0 \\ -1\end{pmatrix} \begin{pmatrix}1 & -2 & 3\end{pmatrix} = \begin{pmatrix}2 & -4 & 6 \\ 0 & 0 & 0 \\ -1 & 2 & -3\end{pmatrix}
    $$
    
*   **Rank of $u\,v^{\top}$**:
    Since $u\,v^{\top}$ is an outer product of two non-zero vectors, each row is a scalar multiple of $v^{\top}$ (and each column a multiple of $u$). The rows are linearly dependent.
    Row 2 is $-2 \times$ Row 1. Row 3 is $3 \times$ Row 1.
    Thus, only 1 linearly independent row exists.
    **Rank = 1**.

### Ex 5.

Show that the diagonal matrix $D=\operatorname{diag}(2,-3,5)$ commits with any diagonal matrix $E=\operatorname{diag}(a,b,c)$. Additionally, calculate $D^{3}$ and, if it exists, $D^{-1}$.

**Solution:**

*   **commutativity**:
    $D = \begin{pmatrix}2 & 0 & 0 \\ 0 & -3 & 0 \\ 0 & 0 & 5\end{pmatrix}$, $E = \begin{pmatrix}a & 0 & 0 \\ 0 & b & 0 \\ 0 & 0 & c\end{pmatrix}$.
    $D \cdot E = \begin{pmatrix}2a & 0 & 0 \\ 0 & -3b & 0 \\ 0 & 0 & 5c\end{pmatrix}$.
    $E \cdot D = \begin{pmatrix}2a & 0 & 0 \\ 0 & -3b & 0 \\ 0 & 0 & 5c\end{pmatrix}$.
    Since scalar multiplication is commutative, $D \cdot E = E \cdot D$.

*   **$D^3$**:
    For diagonal matrices, powers are applied to diagonal elements.
    
    $$
    D^3 = \operatorname{diag}(2^3, (-3)^3, 5^3) = \begin{pmatrix}8 & 0 & 0 \\ 0 & -27 & 0 \\ 0 & 0 & 125\end{pmatrix}
    $$

*   **$D^{-1}$**:
    Exists if all diagonal elements are non-zero.
    
    $$
    D^{-1} = \operatorname{diag}(2^{-1}, (-3)^{-1}, 5^{-1}) = \begin{pmatrix}1/2 & 0 & 0 \\ 0 & -1/3 & 0 \\ 0 & 0 & 1/5\end{pmatrix}
    $$

### Ex 6.

$\star$ For matrix

$$
P=\begin{pmatrix}1 & 1 & 0\\ 0 & 1 & 1\\ 1 & 0 & 1\end{pmatrix}
$$

calculate $P^{2}$ and $P^{3}$. Does the sequence $P^{n}$ have a noticeable pattern for $n=1,2,3$?

**Solution:**

*   **$P^2$**:
    
    $$
    \begin{pmatrix}1 & 1 & 0\\ 0 & 1 & 1\\ 1 & 0 & 1\end{pmatrix}\begin{pmatrix}1 & 1 & 0\\ 0 & 1 & 1\\ 1 & 0 & 1\end{pmatrix} = \begin{pmatrix}1+0+0 & 1+1+0 & 0+1+0 \\ 1+0+1 & 0+1+0 & 1+1+1 \\ 1+0+1 & 1+0+0 & 0+0+1\end{pmatrix} = \begin{pmatrix}1 & 2 & 1 \\ 2 & 1 & 2 \\ 2 & 1 & 1\end{pmatrix}
    $$
    
*   **$P^3 = P^2 \cdot P$**:
    
    $$
    \begin{pmatrix}1 & 2 & 1 \\ 2 & 1 & 2 \\ 2 & 1 & 1\end{pmatrix}\begin{pmatrix}1 & 1 & 0\\ 0 & 1 & 1\\ 1 & 0 & 1\end{pmatrix} = \begin{pmatrix}1+0+1 & 1+2+0 & 2+1+1 \\ 2+0+2 & 2+1+0 & 1+2+2 \\ 2+0+1 & 2+1+0 & 1+1+1\end{pmatrix} = \begin{pmatrix}2 & 3 & 4 \\ 4 & 3 & 5 \\ 3 & 3 & 3\end{pmatrix}
    $$
    
*   **Pattern**:
    $P^1$: entries are 0 or 1.
    $P^2$: entries are 1 or 2.
    $P^3$: entries are 2, 3, 4, 5.
    The values are increasing, but there isn't a simple "cyclic" pattern like $P^k = I$. The matrix is becoming "fuller" and values are growing.

### Ex 7.

$\star$ Rotation coding example.
Calculate the product of rotation matrices by angle $\theta$ in 2D:

$$
R(\theta) = \begin{pmatrix}\cos\theta & -\sin\theta\\ \sin\theta & \cos\theta\end{pmatrix}
$$

Verify that $R(\theta_1)R(\theta_2) = R(\theta_1 + \theta_2)$.

**Solution:**

$$
R(\theta_1) \cdot R(\theta_2) = \begin{pmatrix}\cos\theta_1 & -\sin\theta_1\\ \sin\theta_1 & \cos\theta_1\end{pmatrix} \cdot \begin{pmatrix}\cos\theta_2 & -\sin\theta_2\\ \sin\theta_2 & \cos\theta_2\end{pmatrix}
$$

Element (1,1): $\cos\theta_1\cos\theta_2 - \sin\theta_1\sin\theta_2 = \cos(\theta_1+\theta_2)$
Element (1,2): $\cos\theta_1(-\sin\theta_2) - \sin\theta_1\cos\theta_2 = -(\sin\theta_2\cos\theta_1 + \cos\theta_2\sin\theta_1) = -\sin(\theta_1+\theta_2)$
Element (2,1): $\sin\theta_1\cos\theta_2 + \cos\theta_1\sin\theta_2 = \sin(\theta_1+\theta_2)$
Element (2,2): $\sin\theta_1(-\sin\theta_2) + \cos\theta_1\cos\theta_2 = \cos(\theta_1+\theta_2)$

Thus:

$$
R(\theta_1)R(\theta_2) = \begin{pmatrix}\cos(\theta_1+\theta_2) & -\sin(\theta_1+\theta_2)\\ \sin(\theta_1+\theta_2) & \cos(\theta_1+\theta_2)\end{pmatrix} = R(\theta_1+\theta_2)
$$

### Ex 8.

$\star$ Knowing that

$$
\begin{aligned}\sin(x)&=x-\frac{x^{3}}{3!}+\frac{x^{5}}{5!}-\ldots\\ \cos(x)&=1-\frac{x^{2}}{2!}+\frac{x^{4}}{4!}-\ldots\end{aligned}
$$

show to rotation matrix $R(\theta)$ can be written as

$$
R(\theta) = I +  A + \frac{1}{2!} A^{2} + \frac{1}{3!} A^{3} + \ldots
$$

where $A = \begin{pmatrix}0 & -\theta\\ \theta & 0\end{pmatrix}$.

**Solution:**
Calculate powers of $A$:
$A^1 = \theta \begin{pmatrix}0 & -1\\ 1 & 0\end{pmatrix} = \theta J$, where $J^2 = -I$.
$A^2 = \begin{pmatrix}0 & -\theta\\ \theta & 0\end{pmatrix} \begin{pmatrix}0 & -\theta\\ \theta & 0\end{pmatrix} = \begin{pmatrix}-\theta^2 & 0\\ 0 & -\theta^2\end{pmatrix} = -\theta^2 I$.
$A^3 = A^2 \cdot A = -\theta^2 I \cdot A = -\theta^2 A$.
$A^4 = -\theta^2 A \cdot A = -\theta^2 (-\theta^2 I) = \theta^4 I$.

The series expansion:
$e^A = I + A + \frac{1}{2!}A^2 + \frac{1}{3!}A^3 + \frac{1}{4!}A^4 + \ldots$
Separate terms with $I$ and terms with $A$:
$= I (1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} - \ldots) + \begin{pmatrix}0 & -1\\ 1 & 0\end{pmatrix} (\theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} - \ldots)$
(Note: in odd terms $A^k$, we factor out the matrix part structure. Specifically $A=\theta J$, $A^3 = -\theta^3 J$. So the coefficient of $J$ is $\theta - \theta^3/3! \dots$)

Using Taylor series for sin and cos:
$= I \cos\theta + \begin{pmatrix}0 & -1\\ 1 & 0\end{pmatrix} \sin\theta$
$= \begin{pmatrix}\cos\theta & 0\\ 0 & \cos\theta\end{pmatrix} + \begin{pmatrix}0 & -\sin\theta\\ \sin\theta & 0\end{pmatrix} = \begin{pmatrix}\cos\theta & -\sin\theta\\ \sin\theta & \cos\theta\end{pmatrix} = R(\theta)$.

### Ex 9.

$\star\star$ Pauli matrices are defined as:

$$
\sigma_x = \begin{pmatrix}0 & 1\\ 1 & 0\end{pmatrix}, \quad
\sigma_y = \begin{pmatrix}0 & -i\\ i & 0\end{pmatrix}, \quad
\sigma_z = \begin{pmatrix}1 & 0\\ 0 & -1\end{pmatrix}
$$

Check that:
- $\sigma_x^2 = \sigma_y^2 = \sigma_z^2 = I$
- $\sigma_x\sigma_y = i\sigma_z$, $\sigma_y\sigma_z = i\sigma_x$, $\sigma_z\sigma_x = i\sigma_y$
- $\{\sigma_i, \sigma_j\} = 2\delta_{ij}I$ (anti-commutator)

**Solution:**

*   **Squares**:
    $\sigma_x^2 = \begin{pmatrix}0 & 1\\ 1 & 0\end{pmatrix}\begin{pmatrix}0 & 1\\ 1 & 0\end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1\end{pmatrix} = I$.
    $\sigma_y^2 = \begin{pmatrix}0 & -i\\ i & 0\end{pmatrix}\begin{pmatrix}0 & -i\\ i & 0\end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1\end{pmatrix} = I$.
    $\sigma_z^2 = \begin{pmatrix}1 & 0\\ 0 & -1\end{pmatrix}\begin{pmatrix}1 & 0\\ 0 & -1\end{pmatrix} = \begin{pmatrix}1 & 0\\ 0 & 1\end{pmatrix} = I$.
    
*   **Products**:
    $\sigma_x\sigma_y = \begin{pmatrix}0 & 1\\ 1 & 0\end{pmatrix}\begin{pmatrix}0 & -i\\ i & 0\end{pmatrix} = \begin{pmatrix}i & 0\\ 0 & -i\end{pmatrix} = i\begin{pmatrix}1 & 0\\ 0 & -1\end{pmatrix} = i\sigma_z$.
    
*   **Anti-commutator**:
    $\{\sigma_x, \sigma_y\} = \sigma_x\sigma_y + \sigma_y\sigma_x = i\sigma_z + (-i\sigma_z) = 0$.
    For $i=j$, $\{\sigma_i, \sigma_i\} = 2\sigma_i^2 = 2I$.
    Thus $\{\sigma_i, \sigma_j\} = 2\delta_{ij}I$ holds.

## Determinants

### Ex 1.

Calculate determinant using Sarrus method:

$$
A=\begin{pmatrix}2 & 3 & 1\\ 0 & -1 & 4\\ 5 & 2 & 0\end{pmatrix}
$$

**Solution:**
Sarrus rule: sum of diagonals TL-BR minus sum of diagonals BL-TR.
$(2 \cdot (-1) \cdot 0) + (3 \cdot 4 \cdot 5) + (1 \cdot 0 \cdot 2) - (5 \cdot (-1) \cdot 1) - (2 \cdot 4 \cdot 2) - (0 \cdot 0 \cdot 3)$
$= 0 + 60 + 0 - (-5) - 16 - 0$
$= 60 + 5 - 16 = 49$.

### Ex 2.

Calculate determinants using Laplace expansion:
a) $A=(1)$ -> $\det = 1$.
b) $B=\begin{pmatrix}1 & 0 & 2\\ 3 & 1 & 0\\ 4 & 5 & 6\end{pmatrix}$.
Expand along row 1:
$= 1 \cdot \begin{vmatrix}1 & 0\\ 5 & 6\end{vmatrix} - 0 + 2 \cdot \begin{vmatrix}3 & 1\\ 4 & 5\end{vmatrix}$
$= 1(6-0) + 2(15-4) = 6 + 2(11) = 6 + 22 = 28$.

### Ex 3.

Show that if two rows are equal, determinant is zero.

**Solution:**
If we swap two equal rows, the determinant changes sign ($\det(A) = -\det(A')$). But since the rows are identical, the matrix remains the same ($\det(A) = \det(A')$).
So $\det(A) = -\det(A) \Rightarrow 2\det(A) = 0 \Rightarrow \det(A) = 0$.
Example: $\begin{vmatrix}1 & 2 & 3\\ 1 & 2 & 3\\ 4 & 5 & 6\end{vmatrix} = 0$.

### Ex 4.

Calculate determinant of triangle matrix $T$ with diagonal $(3,-2,5,1)$.

**Solution:**
Determinant of a triangular matrix is the product of diagonal entries.
$\det = 3 \cdot (-2) \cdot 5 \cdot 1 = -30$.

## Matrix Inversion

### Ex 1.

Find inverse for $2\times2$ matrices:
$A=\begin{pmatrix}2 & 1\\ 5 & 3\end{pmatrix}$.
$\det(A) = 6 - 5 = 1$.
$A^{-1} = \frac{1}{1} \begin{pmatrix}3 & -1\\ -5 & 2\end{pmatrix} = \begin{pmatrix}3 & -1\\ -5 & 2\end{pmatrix}$.

## Systems of Linear Equations

### Ex 1.

Solve:

$$
\begin{cases} 2x+3y=5 \\ x-4y=-2 \end{cases}
$$

**Solution:**
From eq 2: $x = 4y - 2$.
Substitute into eq 1: $2(4y-2) + 3y = 5 \Rightarrow 8y - 4 + 3y = 5 \Rightarrow 11y = 9 \Rightarrow y = 9/11$.
$x = 4(9/11) - 2 = 36/11 - 22/11 = 14/11$.
Answer: $x=14/11, y=9/11$.
