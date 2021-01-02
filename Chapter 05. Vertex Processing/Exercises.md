## Exercises

#### 1. 

$$
\begin{pmatrix}
\frac{c}{a} & 0 \\\\
0 & \frac{d}{b}\\\\
\end{pmatrix}
$$



#### 2.

$$
\begin{pmatrix}
\frac{d}{a} & 0 & 0\\\\
0 & \frac{e}{b} & 0\\\\
0 & 0 & \frac{f}{c}
\end{pmatrix}
$$



#### 3.

#### 4.

#### 5.

$$
M_{view} =
\begin{pmatrix}
u_x & u_y & u_z & -u \cdot EYE \\\\
v_x & v_y & v_z & -v \cdot EYE\\\\
n_x & n_y & n_z & -n \cdot EYE\\\\
0 & 0 & 0 & 1
 \end{pmatrix} = 
\begin{pmatrix}
0 & 1 & 0 & 0\\\\
-1 & 0 & 0 & -5\\\\
0 & 0 & 1 & 0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$





#### 6.

#### (a)

Origin in camera space =  EYE
$$
n = (0,0,-1), u = (-1,0,0), v = (0,1,0)
$$
Answer:
$$
\{(-1,0,0), (0,1,0), (0,0,-1), (0,0,-\sqrt{3}) \}
$$


#### (b)

$$
M_{view} = RT = \begin{pmatrix}
u_x & u_y & u_z & -u \cdot EYE \\\\
v_x & v_y & v_z & -v \cdot EYE\\\\
n_x & n_y & n_z & -n \cdot EYE\\\\
0 & 0 & 0 & 1
 \end{pmatrix} = 
\begin{pmatrix}
-1 & 0 & 0 & \sqrt{3}\\\\
0 & 1 & 0 & 0\\\\
0 & 0 & -1 & 0\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$





#### 7.

#### (a)

Origin in camera space =  EYE
$$
n = (0,0,1), u = (1,0,0), v = (0,1,0)
$$

$$
\{(1,0,0), (0,1,0), (0,0,1), (0,0,3) \}
$$

#### (b)

$$
M_{view} = RT = \begin{pmatrix}
u_x & u_y & u_z & -u \cdot EYE \\\\
v_x & v_y & v_z & -v \cdot EYE\\\\
n_x & n_y & n_z & -n \cdot EYE\\\\
0 & 0 & 0 & 1
 \end{pmatrix} = 
\begin{pmatrix}
1 & 0 & 0 & 0\\\\
0 & 1 & 0 & 0\\\\
0 & 0 & 1 & 3\\\\
0 & 0 & 0 & 1
 \end{pmatrix}
$$



#### 8.

#### 9. 

Given that two view parameters share the same orthonormal basis, the resulting camera spaces are identical.

The camera space they share is:
$$
\{(0,0,1),(-\frac{3}{5},\frac{4}{5},0),(\frac{4}{5},\frac{3}{5},0),(18,8,0)\}
$$


#### 10.

#### 11.

#### 12.

$$
aspect = \frac{\tan(\frac{fovx}{2})}{\tan(\frac{fovy}{2})}
$$



#### 13.

#### 14.

