## Exercises

#### 1.

#### (a)

$$
s_a \times m_a + m_e + \sum_{m}^{lights} max(n\cdot{l_m},0)s_d \times m_d + (max(r_m \cdot {v},0))^{sh}s_s \times m_s
$$



#### (b) 

Diffuse and specular reflection terms should be modified using formula down below.
$$
l(p,p_0) = \frac{1}{\mid p - p_0 \mid ^2} l_{p0}
$$




#### 2.

Every vector used for lighting is assumed to be a unit vector.View vector may not remain normalized after going through rasterizer. 

#### 3.

When $\theta$ exceeds 90 degrees,  $n \cdot {l}$  becomes negative value and surface does not receive any lights. As the amount of light should be zero on the surface,  max function is required .

#### 4.

$$
r = 2n(n \cdot{l}) - l
$$

#### 5.

Smaller $sh$ leads to bigger cone, results in large range of speculated surface and vice versa 