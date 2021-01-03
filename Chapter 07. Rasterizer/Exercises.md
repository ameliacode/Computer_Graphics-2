## Exercises

#### 1.

#### (a)

The triangle's winding order is CW

#### (b)

Assume that $v_1 = (0,0), v_2 = (0,1), v_3 = (1,0)$.  A vector connects to $v_1$ to $v_2$ would be $(0,1)$ and another vector that connects to $v_1$ to $v_3 is $(1,0)$ . Following the determinant results in: -1(negative).

#### 2.

#### (a)

$$
\begin{pmatrix}
\frac{w}{2} & 0 & 0 & 0  \\\\
0 & \frac{h}{2} & 0 & 0 \\\\
0 & 0 & \frac{maxZ - minZ}{2} &  0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
 = 
 \begin{pmatrix}
45 & 0 & 0 & 0 \\\\
0 & 90 & 0 & 0 \\\\
0 & 0 & \frac{1}{2} & 0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$



#### (b)

$$
\begin{pmatrix}
1 & 0 & 0 & minX + \frac{w}{2}  \\\\
0 & 1 & 0 & minY + \frac{h}{2} \\\\
0 & 0 & 1 & \frac{maxZ + minZ}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
 = 
 \begin{pmatrix}
1 & 0 & 0 & 55 \\\\
0 & 1 & 0 & 110 \\\\
0 & 0 & 1 &  \frac{3}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$

#### 3.

#### (a)

$$
\begin{pmatrix}
\frac{w}{2} & 0 & 0 & 0  \\\\
0 & \frac{h}{2} & 0 & 0 \\\\
0 & 0 & \frac{maxZ - minZ}{2} &  0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
 = 
 \begin{pmatrix}
100 & 0 & 0 & 0 \\\\
0 & 50 & 0 & 0 \\\\
0 & 0 & \frac{1}{2} & 0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$



#### (b)

$$
\begin{pmatrix}
1 & 0 & 0 & minX + \frac{w}{2}  \\\\
0 & 1 & 0 & minY + \frac{h}{2} \\\\
0 & 0 & 1 & \frac{maxZ + minZ}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
 = 
 \begin{pmatrix}
1 & 0 & 0 & 110 \\\\
0 & 1 & 0 & 70 \\\\
0 & 0 & 1 &  \frac{1}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$





#### 4.

$$
\begin{pmatrix}
\frac{w}{2} & 0 & 0 & minX + \frac{w}{2}  \\\\
0 & \frac{h}{2} & 0 & minY + \frac{h}{2} \\\\
0 & 0 & \frac{maxZ - minZ}{2} &  \frac{maxZ + minZ}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
 = 
 \begin{pmatrix}
50 & 0 & 0 & 80  \\\\
0 & 35 & 0 & 55 \\\\
0 & 0 & \frac{1}{2} &  \frac{1}{2}\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$



#### 5. R = 120,  z = 0.25

#### 6. (42,44,23),(0.45,0.35),0.25 

#### 7. 

No, the result does not remain in midpoint. As projection matrix is not an affine transform matrix, this, in fact, results in distorted distance ratio. 

#### 8.

#### (a) (0,0.66,0.33)

#### (b)

Basically, projection transform does not preserve the distance ratio. Given that $M_{view}$ is not an affine transform matrix, this results in non-linearity attributes. 

Hence, in order to avoid this unwanted result, perspective correction is given. 



