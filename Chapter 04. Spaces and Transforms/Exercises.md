# Exercises

1. 
(a)  

$$  
\begin{pmatrix}
 1 & 0 &  d_x \\\\
 0 & 1 &  d_y \\\\
 1 & 0 & 1   
 \end{pmatrix}
$$  

(b)
$$
\begin{pmatrix}
 cos\theta & -sin\theta & 0 \\\\
 sin\theta & cos\theta & 0 \\\\
 0 & 0 & 1   
 \end{pmatrix}
$$

(c)
$$
\begin{pmatrix}
 s_x & 0 & 0 \\\\
 0 & s_y & 0 \\\\
 0 & 0 & 1   
 \end{pmatrix}
$$

2. As $\{u,v,n\}$ is same as world-space basis, a matrix that went through Rotation Matrix would be:

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
 \begin{pmatrix} 
 0 & 0 & -1 \\\\
 -1 & 1 & 0 \\\\ 
 \sqrt2 & 0 & 0    
 \end{pmatrix}
$$


4. As Rotation Matrix doesn't tackle affine space (ignore last column and row), intuitively, the following matrix is rotated about the y axis, which results in: 

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

4.
5.