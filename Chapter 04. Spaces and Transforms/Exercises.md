## Exercises

#### 1.(a)

$$
\begin{pmatrix}
 1 & 0 &  d_x \\\\
 0 & 1 &  d_y \\\\
 1 & 0 & 1   
 \end{pmatrix}
$$

#### (b)

$$
\begin{pmatrix}
 cos\theta & -sin\theta & 0 \\\\
 sin\theta & cos\theta & 0 \\\\
 0 & 0 & 1   
 \end{pmatrix}
$$

#### (c)

$$
\begin{pmatrix}
 s_x & 0 & 0 \\\\
 0 & s_y & 0 \\\\
 0 & 0 & 1   
 \end{pmatrix}
$$

#### 2. 

As $\{u,v,n\}$ is same as world-space basis, a matrix that went through Rotation Matrix would be:
$$
R * \begin{pmatrix} 
1 & 0 & 0 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1    
\end{pmatrix} = \begin{pmatrix} 
0 & 0 & \frac{1}{\sqrt2} \\\\
0 & 1 & \frac{1}{\sqrt2} \\\\
-1 & 0 & 0    
\end{pmatrix}
$$

$$
R^T * R * \begin{pmatrix} 
1 & 0 & 0 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1    
\end{pmatrix} = R^T * \begin{pmatrix} 
0 & 0 & \frac{1}{\sqrt2} \\\\
0 & 1 & \frac{1}{\sqrt2} \\\\
-1 & 0 & 0    
\end{pmatrix}
$$


Answer: 
$$
R^T = \begin{pmatrix} 
 0 & 0 & -1 \\\\
 -1 & 1 & 0 \\\\
 \sqrt2 & 0 & 0    
 \end{pmatrix}
$$



#### 3. 

Rotation Matrix doesn't tackle affine space (ignore last column and row), intuitively, the following matrix is rotated about the y axis, which results in: 
$$
R = \begin{pmatrix}
 cos\pi & 0 & -sin\pi & 0\\\\
 0 & 1 & 0 & 0\\\\
 sin\pi & 0 & cos\pi & 0 \\\\
 0 & 0 & 0 & 1   
 \end{pmatrix}
$$

On the contrary, as Translation Matrix is all about affine space, the following translation matrix would be:
$$
T = \begin{pmatrix}
 1 & 0 & 0 & 3\\\\
 0 & 1 & 0 & -4\\\\
 0 & 0 & 1 & -1 \\\\
 0 & 0 & 0 & 1   
 \end{pmatrix}
$$

#### 4. 

(1) Rotation matrices of each principal axis which transforms to arbitrary axis are required. 

(2) Each principal axis act as a normal vector(result of cross product operation)  in rotation matrices. 

For comprehension, questions down below can help. Dull explanation :( sorry.



#### 5.  

#### (1) 

Following the hint, to transform arbitrary axis onto x-axis, the principal axis of its rotation is y-axis.
$$
R_1 * \begin{pmatrix} 
3 \\\\
0 \\\\
4    
\end{pmatrix} = \begin{pmatrix} 
1 \\\\
0\\\\
0   
\end{pmatrix}
$$

$$
R_1 =\begin{pmatrix} 
\frac{3}{25} & 0 & \frac{4}{25} \\\\
0 & 1 & 0 \\\\
-\frac{4}{25} & 0 & \frac{3}{25}    
\end{pmatrix}
$$

#### (2) 

$$
R_2 =\begin{pmatrix} 
1 & 0 & 0 \\\\
0 & 0 & 1 \\\\
0 & -1 & 0 
\end{pmatrix}
$$



#### (3)

The Inverse matrix of (1) is synonym for its transpose matrix
$$
R_3 =\begin{pmatrix} 
\frac{3}{25} & 0 & -\frac{4}{25} \\\\
0 & 1 & 0 \\\\
\frac{4}{25} & 0 & \frac{3}{25}    
\end{pmatrix}
$$
Computing all three matrices would be:
$$
R_3 R_2 R_1 =\begin{pmatrix} 
\frac{9}{625} & \frac{4}{25} & \frac{12}{625} \\\\
-\frac{4}{25} & 0 & \frac{3}{25} \\\\
\frac{12}{625} & -\frac{3}{25} & \frac{16}{625}    
\end{pmatrix}
$$




#### 6. 

#### (1)

$$
R_1 * \begin{pmatrix} 
3 \\\\4 \\\\0    
\end{pmatrix} = 
\begin{pmatrix} 1\\\\0\\\\0   
\end{pmatrix}
$$

$$
R_1 =\begin{pmatrix} 
\frac{3}{25} & \frac{4}{25} & 0\\\\
-\frac{4}{25} & \frac{3}{25} & 0  \\\\
0 & 0 & 1 
\end{pmatrix}
$$

#### (2)

$$
R_2 =\begin{pmatrix} 
1 & 0 & 0 \\\\
0 & 0 & 1 \\\\
0 & -1 & 0 
\end{pmatrix}
$$

#### (3)

The Inverse matrix of (1) is synonym for its transpose matrix
$$
R_3 =\begin{pmatrix} 
\frac{3}{25} & -\frac{4}{25} & 0\\\\
\frac{4}{25} & \frac{3}{25} & 0  \\\\
0 & 0 & 1 
\end{pmatrix}
$$
Computing all three matrices would be:
$$
R_3 R_2 R_1 =\begin{pmatrix} 
\frac{9}{625} & -\frac{12}{625} & \frac{4}{25} \\\\
-\frac{12}{625} & \frac{16}{625} & \frac{3}{25} \\\\
-\frac{4}{625} & -\frac{3}{25} & 0   
\end{pmatrix}
$$




