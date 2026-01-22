# Section 2 — Analytic Geometry: Exercises

## Vectors

### Ex 1.

For vectors in space

$$
\mathbf{u}=[1,2,-1]\quad\text{and}\quad\mathbf{v}=[2,-1,3]
$$

calculate $\mathbf{u}+\mathbf{v}$, $\mathbf{u}-\mathbf{v}$, dot product $\mathbf{u}\cdot\mathbf{v}$, and norms $\|\mathbf{u}\|$ and $\|\mathbf{v}\|$. Check if the vectors are orthogonal.

**Solution:**

*   **$\mathbf{u}+\mathbf{v}$**:
    $[1+2, 2+(-1), -1+3] = [3, 1, 2]$
    
*   **$\mathbf{u}-\mathbf{v}$**:
    $[1-2, 2-(-1), -1-3] = [-1, 3, -4]$
    
*   **$\mathbf{u}\cdot\mathbf{v}$ (Dot Product)**:
    $1\cdot2 + 2\cdot(-1) + (-1)\cdot3 = 2 - 2 - 3 = -3$
    
*   **Norms**:
    $\|\mathbf{u}\| = \sqrt{1^2 + 2^2 + (-1)^2} = \sqrt{1+4+1} = \sqrt{6}$
    $\|\mathbf{v}\| = \sqrt{2^2 + (-1)^2 + 3^2} = \sqrt{4+1+9} = \sqrt{14}$
    
*   **Orthogonality**:
    Vectors are orthogonal if their dot product is 0.
    Since $\mathbf{u}\cdot\mathbf{v} = -3 \neq 0$, they are **not orthogonal**.

### Ex 2.

For points $A(1,0,2)$, $B(3,-1,1)$ and $C(2,2,0)$, calculate vectors $\vec{AB}$ and $\vec{AC}$ and find the angle between them.

**Solution:**

*   **Vectors**:
    $\vec{AB} = B - A = [3-1, -1-0, 1-2] = [2, -1, -1]$
    $\vec{AC} = C - A = [2-1, 2-0, 0-2] = [1, 2, -2]$
    
*   **Angle**:
    $\cos \theta = \frac{\vec{AB} \cdot \vec{AC}}{\|\vec{AB}\| \|\vec{AC}\|}$
    $\vec{AB} \cdot \vec{AC} = 2\cdot1 + (-1)\cdot2 + (-1)\cdot(-2) = 2 - 2 + 2 = 2$
    $\|\vec{AB}\| = \sqrt{4+1+1} = \sqrt{6}$
    $\|\vec{AC}\| = \sqrt{1+4+4} = \sqrt{9} = 3$
    
    $\cos \theta = \frac{2}{3\sqrt{6}}$.
    $\theta = \arccos\left(\frac{2}{3\sqrt{6}}\right)$.

### Ex 3.

Calculate cross product $\mathbf{u}\times\mathbf{v}$ for vectors from problem 1 and check if it is orthogonal to both vectors.

**Solution:**
$\mathbf{u}=[1,2,-1]$, $\mathbf{v}=[2,-1,3]$.

$$
\mathbf{u}\times\mathbf{v} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 1 & 2 & -1 \\ 2 & -1 & 3 \end{vmatrix}
$$

$= \mathbf{i}(6 - 1) - \mathbf{j}(3 - (-2)) + \mathbf{k}(-1 - 4)$
$= 5\mathbf{i} - 5\mathbf{j} - 5\mathbf{k} = [5, -5, -5]$.

Check orthogonality:
$(\mathbf{u}\times\mathbf{v}) \cdot \mathbf{u} = 5(1) - 5(2) - 5(-1) = 5 - 10 + 5 = 0$. (Yes)
$(\mathbf{u}\times\mathbf{v}) \cdot \mathbf{v} = 5(2) - 5(-1) - 5(3) = 10 + 5 - 15 = 0$. (Yes)

### Ex 4.

For vectors in plane: $\mathbf{a}=[3,4]$ and $\mathbf{b}=[-4,3]$, calculate their dot product and check if they are perpendicular. Find projection of $\mathbf{a}$ on $\mathbf{b}$.

**Solution:**
*   **Dot product**:
    $\mathbf{a}\cdot\mathbf{b} = 3(-4) + 4(3) = -12 + 12 = 0$.
    Since the dot product is 0, they are **perpendicular**.
    
*   **Projection**:
    Since they are perpendicular, the projection of $\mathbf{a}$ on $\mathbf{b}$ is the **zero vector** $\mathbf{0}$.
    Formula: $\operatorname{proj}_{\mathbf{b}}\mathbf{a} = \frac{\mathbf{a}\cdot\mathbf{b}}{\|\mathbf{b}\|^2}\mathbf{b} = \frac{0}{25}\mathbf{b} = \mathbf{0}$.

### Ex 5.

Calculate length of vector $\mathbf{c} = [1, 1]$ and find its unit vector (versor).

**Solution:**
$\|\mathbf{c}\| = \sqrt{1^2+1^2} = \sqrt{2}$.
Unit vector $\hat{\mathbf{c}} = \frac{\mathbf{c}}{\|\mathbf{c}\|} = [\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}] = [\frac{\sqrt{2}}{2}, \frac{\sqrt{2}}{2}]$.

### Ex 6.

Calculate length of vector $\mathbf{c} = [1, 2, 3]$ and find its unit vector.

**Solution:**
$\|\mathbf{c}\| = \sqrt{1+4+9} = \sqrt{14}$.
Unit vector $\hat{\mathbf{c}} = [\frac{1}{\sqrt{14}}, \frac{2}{\sqrt{14}}, \frac{3}{\sqrt{14}}]$.

### Ex 7.

Calculate area of triangle spanned by vectors $[2, 1, 2]$ and $[-1, 1, 1]$.

**Solution:**
Area is $\frac{1}{2} \|\mathbf{a} \times \mathbf{b}\|$.
$\mathbf{a} \times \mathbf{b} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 1 & 2 \\ -1 & 1 & 1 \end{vmatrix} = \mathbf{i}(1-2) - \mathbf{j}(2-(-2)) + \mathbf{k}(2-(-1)) = [-1, -4, 3]$.
$\|\mathbf{a} \times \mathbf{b}\| = \sqrt{(-1)^2 + (-4)^2 + 3^2} = \sqrt{1 + 16 + 9} = \sqrt{26}$.
Area = $\frac{\sqrt{26}}{2}$.

### Ex 8.

Calculate angle in degrees between vectors $[4,2,1]$ and $[1,3,2]$.

**Solution:**
$\mathbf{u}\cdot\mathbf{v} = 4(1)+2(3)+1(2) = 4+6+2=12$.
$\|\mathbf{u}\| = \sqrt{16+4+1} = \sqrt{21}$.
$\|\mathbf{v}\| = \sqrt{1+9+4} = \sqrt{14}$.
$\cos \theta = \frac{12}{\sqrt{21}\sqrt{14}} = \frac{12}{\sqrt{294}} = \frac{12}{7\sqrt{6}}$.
$\theta = \arccos(\frac{12}{7\sqrt{6}}) \approx \arccos(0.69985) \approx 45.58^\circ$.

### Ex 9.

Find coordinates of the midpoint of segment with endpoints $A(-1, 2)$ and $B(3, -2)$.

**Solution:**
$M = \frac{A+B}{2} = (\frac{-1+3}{2}, \frac{2+(-2)}{2}) = (\frac{2}{2}, \frac{0}{2}) = (1, 0)$.

### Ex 10.

The BAC-CAB Identity. Prove:

$$
\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c}) \mathbf{b} - (\mathbf{a} \cdot \mathbf{b}) \mathbf{c}.
$$

**Solution:**
This is a standard vector identity.
Let $\mathbf{a}, \mathbf{b}, \mathbf{c}$ be defined by components.
Calculating the $x$-component of the LHS:
$(\mathbf{b} \times \mathbf{c})_x = b_yc_z - b_zc_y$.
$(\mathbf{b} \times \mathbf{c})_y = b_zc_x - b_xc_z$.
$(\mathbf{b} \times \mathbf{c})_z = b_xc_y - b_yc_x$.
$(\mathbf{a} \times (\mathbf{b} \times \mathbf{c}))_x = a_y(\mathbf{b} \times \mathbf{c})_z - a_z(\mathbf{b} \times \mathbf{c})_y$
$= a_y(b_xc_y - b_yc_x) - a_z(b_zc_x - b_xc_z)$
$= a_yb_xc_y - a_yb_yc_x - a_zb_zc_x + a_zb_xc_z$
$= b_x(a_y c_y + a_z c_z) - c_x(a_y b_y + a_z b_z)$.
Add and subtract $a_x b_x c_x$:
$= b_x(a_x c_x + a_y c_y + a_z c_z) - c_x(a_x b_x + a_y b_y + a_z b_z)$
$= b_x(\mathbf{a} \cdot \mathbf{c}) - c_x(\mathbf{a} \cdot \mathbf{b})$.
This matches the $x$-component of the RHS. Symmetry holds for $y$ and $z$.

### Ex 11.

Find the most general form of a vector simultaneously perpendicular to $\mathbf{v}=[-1,3,0]$ and $\mathbf{u}=[0,1,1]$.

**Solution:**
A vector perpendicular to both is parallel to their cross product.
$\mathbf{w} = \mathbf{v} \times \mathbf{u} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ -1 & 3 & 0 \\ 0 & 1 & 1 \end{vmatrix} = \mathbf{i}(3) - \mathbf{j}(-1) + \mathbf{k}(-1) = [3, 1, -1]$.
General form: $k [3, 1, -1]$ for any scalar $k \in \mathbb{R}$.

## Lines

### Ex 1.

Equation of line through $P(1,2)$ and $Q(3,-1)$.

**Solution:**
Slope $m = \frac{-1-2}{3-1} = \frac{-3}{2} = -1.5$.
Point-slope form: $y - 2 = -\frac{3}{2}(x - 1)$.
$y = -1.5x + 1.5 + 2 = -1.5x + 3.5$. (Slope-intercept form)
General form: $3x + 2y - 7 = 0$.

### Ex 2.

Parametric equation of line perpendicular to line from problem 1, passing through $R(0,1)$.

**Solution:**
Slope of original line: $-3/2$.
Slope of perpendicular line: $\frac{-1}{-3/2} = \frac{2}{3}$.
Direction vector: $[3, 2]$.
Parametric equation:

$$
\begin{cases} x = 0 + 3t \\ y = 1 + 2t \end{cases} \quad t \in \mathbb{R}
$$

### Ex 3.

Line through $A(1, 2)$ parallel to $y = 2x + 3$.

**Solution:**
Parallel slope $m=2$.
$y - 2 = 2(x - 1) \Rightarrow y = 2x - 2 + 2 \Rightarrow y = 2x$.

### Ex 4.

Relations between $l_1: 2x-3y+1=0$ and $l_2: 4x-6y-5=0$.

**Solution:**
Normal vectors: $\mathbf{n}_1 = [2, -3]$, $\mathbf{n}_2 = [4, -6]$.
Since $\mathbf{n}_2 = 2\mathbf{n}_1$, the lines are **parallel**.
Check if they are the same: $2(2x-3y+1) = 4x-6y+2 \neq 4x-6y-5$.
They are distinct parallel lines. No intersection.

### Ex 5.

Angle between $y = x + 3$ and $Ox$ axis.

**Solution:**
Slope $m=1$.
$\tan \alpha = 1 \Rightarrow \alpha = 45^\circ$.

### Ex 6.

Vector perpendicular to $x + y + 1 = 0$.

**Solution:**
The normal vector is coefficients of $x$ and $y$: $\mathbf{n} = [1, 1]$.

### Ex 7.

$\star$ Distance from $S(2,3)$ to $l: 3x-4y+5=0$.

**Solution:**
Formula: $d = \frac{|Ax_0 + By_0 + C|}{\sqrt{A^2+B^2}}$.
$d = \frac{|3(2) - 4(3) + 5|}{\sqrt{3^2+(-4)^2}} = \frac{|6 - 12 + 5|}{\sqrt{25}} = \frac{|-1|}{5} = 0.2$.

### Ex 8.

$\star$ Line through $T(1,1)$ with angle $\pi/6$ ($30^\circ$) to OX.

**Solution:**
Slope $m = \tan(30^\circ) = \frac{1}{\sqrt{3}} = \frac{\sqrt{3}}{3}$.
$y - 1 = \frac{\sqrt{3}}{3}(x - 1)$.
$y = \frac{\sqrt{3}}{3}x + (1 - \frac{\sqrt{3}}{3})$.
Intersection with OY (set $x=0$): Point $(0, 1 - \frac{\sqrt{3}}{3})$.

## Planes

### Ex 1.

Plane through $A(1,0,2)$ with normal $\mathbf{n}=[2,-1,1]$.

**Solution:**
$2(x-1) - 1(y-0) + 1(z-2) = 0$.
$2x - 2 - y + z - 2 = 0$.
General eq: $2x - y + z - 4 = 0$.

### Ex 2.

Plane through $A(1,0,0)$, $B(0,1,0)$, $C(0,0,1)$.

**Solution:**
Intercept form: $\frac{x}{1} + \frac{y}{1} + \frac{z}{1} = 1$.
$x + y + z - 1 = 0$.

### Ex 3.

Angle between $\pi_1: x+2y-2z+1=0$ and $\pi_2: 2x-y+z-3=0$.

**Solution:**
Normals: $\mathbf{n}_1 = [1, 2, -2]$, $\mathbf{n}_2 = [2, -1, 1]$.
$\cos \theta = \frac{|\mathbf{n}_1 \cdot \mathbf{n}_2|}{\|\mathbf{n}_1\| \|\mathbf{n}_2\|}$.
Dot prod: $1(2) + 2(-1) - 2(1) = 2 - 2 - 2 = -2$. Absolute value: 2.
$\|\mathbf{n}_1\| = \sqrt{1+4+4} = 3$.
$\|\mathbf{n}_2\| = \sqrt{4+1+1} = \sqrt{6}$.
$\cos \theta = \frac{2}{3\sqrt{6}}$.
$\theta = \arccos(\frac{2}{3\sqrt{6}})$.

### Ex 4.

Distance of $P(3,0,1)$ from $x-2y+2z-4=0$.

**Solution:**
$d = \frac{|1(3) - 2(0) + 2(1) - 4|}{\sqrt{1^2+(-2)^2+2^2}} = \frac{|3 + 0 + 2 - 4|}{\sqrt{9}} = \frac{|1|}{3} = \frac{1}{3}$.

### Ex 5.

Vector perpendicular to $x + y + z = 1$.

**Solution:**
Normal vector: $\mathbf{n} = [1, 1, 1]$.

### Ex 6.

Plane through $A(1, 2, 3)$ parallel to $2x + 3y + 4z = 5$.

**Solution:**
Same normal $[2, 3, 4]$.
$2(x-1) + 3(y-2) + 4(z-3) = 0$.
$2x + 3y + 4z - 2 - 6 - 12 = 0$.
$2x + 3y + 4z - 20 = 0$.

## Line and Plane in Space

### Ex 1.

Does line $\ell: x=1+2t, y=-1+t, z=3-t$ intersect plane $\pi: 2x-y+z-4=0$?

**Solution:**
Substitute line equations into plane equation:
$2(1+2t) - (-1+t) + (3-t) - 4 = 0$
$2 + 4t + 1 - t + 3 - t - 4 = 0$
$2t + 2 = 0 \Rightarrow 2t = -2 \Rightarrow t = -1$.

Intersection exists at $t=-1$.
$x = 1 + 2(-1) = -1$.
$y = -1 + (-1) = -2$.
$z = 3 - (-1) = 4$.
Point: $(-1, -2, 4)$.
